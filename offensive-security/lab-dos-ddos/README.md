# SECURITE DES RESEAUX : ATTAQUES PAR DENIS SERVICE : DoS/DDoS

## Informations Générales
* **Machine Attaquante :** Kali Linux (`192.168.232.142`)
* **Machine Cible :** Metasploitable 2 (`192.168.232.128`)

---

## Étape 1 : Phase de Reconnaissance et Scan de Ports

Avant de mener toute action, il est indispensable de cartographier la cible pour identifier les services actifs. Nous effectuons un scan ciblé à l'aide de l'outil **Nmap** afin de vérifier si le serveur Web (port 80) est accessible et opérationnel.

```bash
nmap -p 80 [VOTRE_IP_CIBLE]
```
![cartographie de la cible](img/nmap.png)
## Étape 2 : Configuration de la Résolution de Noms (`/etc/hosts`)

Afin d'accéder à la cible via son nom de domaine dédié, nous éditons le fichier `/etc/hosts` de la machine Kali Linux (`192.168.232.142`) pour associer l'adresse IP de Metasploitable 2 (`192.168.232.128`) au domaine `www.mentorat.com`.

```bash
sudo nano /etc/hosts
```
Nous vérifions ensuite la bonne prise en compte de la résolution de nom en accédant au serveur Web cible depuis le navigateur Web de la machine Kali à l'adresse `http://www.mentorat.com`.

![Vérification de l'accès au serveur Web via le domaine www.mentorat.com](img/verif_domain-name.png)

## Étape 3 : Installation de l'Outil Slowloris

Afin de réaliser la simulation d'attaque par déni de service (DoS), nous clonons le dépôt officiel de l'outil [Slowloris sur GitHub](https://github.com/gkbrk/slowloris.git). Cet outil permet d'envoyer des requêtes HTTP incomplètes et de maintenir de nombreuses connexions ouvertes pour saturer la table de connexions du serveur Web.

```bash
sudo git clone https://github.com/gkbrk/slowloris.git
```
## Étape 4 : Installation des Dépendances et Lancement de Slowloris

### 4.1. Installation de la dépendance `socketpool`

Avant d'exécuter le script, nous installons le paquet Python `socketpool` nécessaire à la gestion des sockets de connexion.

```bash
pip install socketpool
```
Nous nous déplaçons ensuite dans le dossier cloné slowloris afin d'accéder au script principal.
![deplacement vers le dossier slowloris](img/slowloris-repertoire.png)

### 4.2. Exécution du test de déni de service (DoS)
Nous lançons l'attaque Slowloris en ciblant l'adresse IP de notre machine Metasploitable 2 (192.168.232.128) sur le port HTTP (80).
```bash
python slowloris.py 192.168.232.128 -p 80
```