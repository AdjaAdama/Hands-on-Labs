# Hands-on Labs & Infrastructure Engineering

Ce dépôt centralise mes travaux pratiques, laboratoires personnels et expérimentations techniques axés sur l'administration systèmes, la virtualisation, l'automatisation et la sécurité des infrastructures.

L'objectif est de valider par la pratique les concepts théoriques et d'industrialiser le déploiement d'environnements de test.

---

## 📂 Organisation
L'arborescence est structurée par objectifs opérationnels :

* **`architectures-cloud/`** : Projets liés au Cloud computing, infrastructures hybrides, orchestration d'infrastructures à grande échelle.

* **`offensive-security/`** : Laboratoires d'analyse de vulnérabilités, simulations d'attaques, tests de pénétration et exercices de type Red Team.

* **`defensive-security/`** : Mise en place de contre-mesures, durcissement de systèmes, configuration de pare-feu et détection d'intrusions (Blue Team).

* **`infrastructure-services/`** : Déploiement de services réseaux fondamentaux (DNS sécurisés, PKI, annuaires d'entreprise, routage virtuel) combinant VM et conteneurs.

* **`observability-operations/`** : Cas centrés sur la supervision globale, l'analyse de logs et la haute disponibilité d'une infrastructure complète.

---

## 🚀 Principes Directeurs de mes Labs

Pour chaque laboratoire présent dans ce dépôt, je m'impose les standards suivants :
1. **Infrastructure as Code (IaC) :** Privilégier au maximum le déploiement scripté plutôt que les configurations manuelles.
2. **Security by Design :** Application du principe du moindre privilège, interdiction des secrets en clair et durcissement des configurations par défaut.
3. **Reproductibilité :** Chaque sous-dossier contient ses propres instructions spécifiques pour être exécuté en un clic ou une commande.

---

## 🛠️ Outils & Technologies

* ![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black) **Linux** : Système d'exploitation cible pour le déploiement des infrastructures.
* ![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=flat-square&logo=ansible&logoColor=white) **Ansible** : Automatisation, gestion de configuration et Infrastructure as Code (IaC).
* ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) **Docker** : Conteneurisation, isolation des services et durcissement des environnements.
* ![Vagrant](https://img.shields.io/badge/Vagrant-1868F2?style=flat-square&logo=vagrant&logoColor=white) **Vagrant** : Provisionnement et orchestration locale de machines virtuelles de test.
* ![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat-square&logo=figma&logoColor=white) **Figma** : Modélisation des architectures réseaux et maquettage visuel des infrastructures.

---

## 🛠️ Prérequis Globaux

Pour exécuter la majorité de ces labs, mon environnement de contrôle local utilise :
* **Hyperviseur :** Un gestionnaire de machines virtuelles fonctionnel (comme VMware ou VirtualBox) pour accueillir les environnements isolés.
* **Ressources :** Un processeur multi-cœur et un minimum de 8 Go de RAM (16 Go recommandés pour les architectures multi-VM).
