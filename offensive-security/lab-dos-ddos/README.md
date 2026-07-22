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
