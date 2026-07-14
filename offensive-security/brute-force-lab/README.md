# Lab: Attaque par Force Brute (Itération, Dictionnaire & Hybride)

## 📝 Présentation du Laboratoire
* **Domaine** : Sécurité Offensive (Offensive Security)
* **Objectif** : Comprendre les mécanismes des attaques par force brute, analyser l'impact de la complexité des mots de passe et étudier les méthodes de remédiation.
* **Outils pressentis** : `Hydra`, `John the Ripper` ou outils équivalents selon les phases du TP.

---

## 🏗️ Architecture & Environnement
* **Machine Cible** : (À compléter lors de la mise en place, ex: VM cible / Conteneur)
* **Machine Attaquante** : (À compléter, ex: Kali Linux)

---

## 🛡️ Réalisation des Manipulations

### Phase 1 : Attaque par itération (Force brute pure)
#### 1. Préparation de la cible
Pour simuler un scénario d'audit réel, une archive RAR chiffrée a été générée depuis un environnement Windows 10, contenant des documents fictifs mais structurellement valides (`Informations bancaires.xlsx` et `Secrets.txt.docx`).

* **Caractéristiques de l'archive :**
  * **Algorithme cible** : RAR5 / WinRAR
  * **Mot de passe appliqué** : `1234` (faible, propice à la force brute pure)
  * **Option activée** : Chiffrement des noms de fichiers (masquage des métadonnées)

L'archive a ensuite été transférée sur le bureau de la machine attaquante Kali Linux pour la suite des manipulations.

![Archive cible sur Kali Linux](img/archive.png)
### Phase 2 : Attaque par dictionnaire
*En attente des premières manipulations.*

### Phase 3 : Attaque hybride
*En attente des premières manipulations.*

---

## 🔍 Conclusion & Remédiation
*En attente des conclusions du laboratoire.*