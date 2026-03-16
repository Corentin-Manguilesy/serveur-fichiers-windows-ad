# Serveur de fichiers sécurisé (SMB + Active Directory)

## Contexte du projet

Ce projet a été réalisé dans le cadre de ma formation **BTS SIO option SISR**.

L'objectif était de mettre en place un serveur de fichiers centralisé dans un environnement Active Directory afin de permettre aux utilisateurs d’accéder aux ressources de leur service via des partages réseau sécurisés.

Ce type d'infrastructure est couramment utilisé dans les systèmes d'information d'entreprise.

---

## Technologies utilisées

- Windows Server 2019
- Active Directory
- SMB
- NTFS
- PowerShell

---

## Fonctionnement

Le projet repose sur les éléments suivants :

- création de groupes Active Directory par service
- création des utilisateurs
- mise en place d'une arborescence de dossiers
- attribution des permissions NTFS
- configuration de partages SMB sécurisés

Chaque service dispose de ses propres ressources accessibles selon les permissions définies.

---

## Automatisation

Des scripts **PowerShell** ont été utilisés pour automatiser certaines tâches :

- création d'utilisateurs
- ajout des utilisateurs aux groupes
- gestion des accès aux dossiers partagés

---

## Tests réalisés

Afin de valider le bon fonctionnement du serveur de fichiers :

- un poste client a été intégré au domaine Active Directory
- des tests d’accès aux partages réseau ont été réalisés selon les groupes utilisateurs
