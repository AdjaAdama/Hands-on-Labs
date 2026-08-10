# Compte Rendu - TP : Persistance Windows & Linux

## 1. Introduction
Ce laboratoire porte sur la mise en place de mécanismes de persistance sur des environnements Windows et Linux. L'objectif est de maintenir un accès discret et continu à un système compromis après une réinitialisation ou une déconnexion.

## 2. Persistance sur Windows
- **Génération du payload** : Utilisation de `msfvenom` pour créer un exécutable malveillant.
- **Transfert et exécution** : Mise en place d'un serveur HTTP temporaire et contournement des mesures de sécurité pour exécuter le payload.
- **Établissement du listener** : Configuration d'un écouteur Metasploit pour intercepter la connexion.
- **Module de persistance** : Utilisation du module `exploit/windows/local/persistence` pour inscrire le payload dans les clés de registre de démarrage automatique.

## 3. Persistance sur Linux
- **Exploitation initiale** : Exploitation de la vulnérabilité du service FTP (`vsftpd 2.3.4`) sur la cible.
- **Élévation du shell** : Obtention d'un shell TTY interactif via Python.
- **Script de reverse shell** : Développement et transfert d'un script Python malveillant.
- **Planification des tâches (Cron)** : Ajout d'une tâche planifiée (`crontab`) pour automatiser l'exécution du reverse shell à intervalles réguliers.

## 4. Conclusion
Résumé des compétences acquises et des mesures de remédiation/défense pour contrer ces vecteurs de persistance.