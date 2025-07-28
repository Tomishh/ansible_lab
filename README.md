# Ansible LAB - Autoformation
---
## Contexte
Afin de prendre la main sur l'outil Ansible et la gestion d'une infrastructure sur une plateforme cloud, une multitudes d'exercices m'ont été fournis par un ami. La liste des énoncés ci-dessous me permetterons de me faire la main sur différents outils.
## Liste des outils
  - Git
  - Ansible
  - Google Cloud
  - Networking divers

## Liste des exercices

### 🧱 Projet 1 : Rôle base – Configuration système de base
**&ensp;📁 roles/base/**

Un rôle système à appliquer à tout serveur dès le départ.

**&ensp;✅ Fonctionnalités :**

- Création de plusieurs utilisateurs avec clé SSH
- Ajout à sudo sans mot de passe
- Configuration de la bannière SSH (/etc/issue.net)
- Sécurisation SSH (PasswordAuthentication no, etc.)
- UFW :
  - Ports ouverts : 22, personnalisable via variable
  - Règles par défaut : deny incoming / allow outgoing

