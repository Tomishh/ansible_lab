# Ansible LAB - Autoformation
---
## Contexte
Afin de prendre la main sur l'outil Ansible et la gestion d'une infrastructure sur une plateforme cloud, une multitudes d'exercices m'ont été fournis par un ami. La liste des énoncés ci-dessous me permetterons de me faire la main sur différents outils.
## Liste des outils
  - Git
  - Ansible
  - Google Cloud
  - Networking divers
---
## Liste des exercices

### 🧱 Projet 1 : Rôle base – Configuration système de base
#### 📁 roles/base/
Un rôle système à appliquer à tout serveur dès le départ.

**&ensp;✅ Fonctionnalités :**

- Création de plusieurs utilisateurs avec clé SSH
- Ajout à sudo sans mot de passe
- Configuration de la bannière SSH (/etc/issue.net)
- Sécurisation SSH (PasswordAuthentication no, etc.)
- UFW :
  - Ports ouverts : 22, personnalisable via variable
  - Règles par défaut : deny incoming / allow outgoing
---
### 🚀 Projet 2 : Rôle app_web – Déploiement d’une app React via Docker
#### 📁 roles/app_web/
Ce rôle déploie une app web statique (comme un build React) dans un conteneur Docker Nginx.
#### ✅ Fonctionnalités :
- Prérequis : docker et docker-compose
- Déploie une app React (ou autre statique) via une image personnalisée
- Utilise un docker-compose.yml généré par template
- Configuration via variables.
---
### ⚙️ Projet 3 : Playbook complet – 2 apps + Apache en load balancer
Ce projet final orchestre le tout : configuration des serveurs, déploiement de 2 apps web avec Docker, et mise en place d’un Apache HTTPD agissant comme reverse proxy/load balancer.
#### 🎯 Objectif :

1 serveur avec Apache qui load-balance vers 2 instances de la même app React (ou 2 apps différentes)
#### ✅ Fonctionnalités :
- Déploiement automatisé sur 3 hôtes (balancer, app1, app2)

