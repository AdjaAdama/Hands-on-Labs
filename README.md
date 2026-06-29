# Hands-on Labs & Infrastructure Engineering

Ce dépôt centralise mes travaux pratiques, laboratoires personnels et expérimentations techniques axés sur l'administration systèmes, la virtualisation, l'automatisation et la sécurité des infrastructures.

L'objectif est de valider par la pratique les concepts théoriques et d'industrialiser le déploiement d'environnements de test.

---

## 📂 Organisation du Dépôt

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

## 🛠️ Prérequis Globaux

Pour exécuter la majorité de ces labs, mon environnement de contrôle local utilise :
* Un système de type UNIX / Linux
* **Ansible** `>= 2.15`
* **Docker** / **Docker Compose**