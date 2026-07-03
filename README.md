# Hands-on Labs & Infrastructure Engineering

Ce dépôt centralise mes travaux pratiques, laboratoires personnels et expérimentations techniques axés sur l'administration systèmes, la virtualisation, l'automatisation et la sécurité des infrastructures.

L'objectif est de valider par la pratique les concepts théoriques et d'industrialiser le déploiement d'environnements de test.

---

## 📂 Organisation
L'arborescence est structurée par piliers technologiques :

*   **`virtualization/`** : Configurations de machines virtuelles, gestion d'hyperviseurs et isolation (Vagrant, QEMU/KVM).
*   **`automation/`** : Scripts de configuration et d'Infrastructure as Code (Ansible, Terraform local).
*   **`containers/`** : Durcissement, orchestration légère et sécurité des environnements conteneurisés (Docker, Podman).
*   **`monitoring/`** : Collecte de métriques, centralisation des logs et observabilité (Prometheus, Grafana).

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
* Un système de type UNIX / Linux
* **Ansible** `>= 2.15`
* **Docker** / **Docker Compose**