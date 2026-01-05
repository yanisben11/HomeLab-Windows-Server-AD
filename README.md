# 🏢 Projet Home Lab : Infrastructure Windows Server & Active Directory

## 📄 Description
Ce projet documente la mise en place d'une infrastructure réseau d'entreprise simulée dans un environnement virtuel. L'objectif était de construire un domaine Active Directory fonctionnel, de la configuration du serveur jusqu'à l'expérience utilisateur finale.

## 🛠️ Technologies utilisées
* **Hyperviseur :** VMware Workstation
* **Serveur :** Windows Server 2022 (Contrôleur de Domaine)
* **Client :** Windows 10 Pro
* **Services :** AD DS (Active Directory Domain Services), DNS, DHCP (Statique)

## ⚙️ Implémentations réalisées

### 1. Configuration Réseau & Serveur
* Installation de Windows Server 2022.
* Configuration d'adressage IP statique pour la stabilité du serveur.
* Déploiement du rôle **AD DS** et promotion en Contrôleur de Domaine.
* Création du domaine racine : `entrepriseyanis.ca`.

### 2. Gestion des Utilisateurs & OUs
* Création d'une structure d'Unités d'Organisation (OU).
* Création de comptes utilisateurs tests (`yanis.test`) pour valider les accès.

### 3. Stratégies de Groupe (GPO)
Mise en place d'automatisations pour standardiser le parc informatique :
* **GPO_Fondecran :** Déploiement automatique de l'identité visuelle de l'entreprise sur tous les postes.
* **GPO_LecteurZ :** Mappage automatique d'un lecteur réseau partagé (Disque Z:) connectant l'utilisateur à son dossier personnel sur le serveur.

## 📸 Captures d'écran
<img width="956" height="663" alt="photos 2" src="https://github.com/user-attachments/assets/60ecc98e-9d66-4dc8-8d8c-f8132b3aeb3d" />
<img width="1919" height="912" alt="photos 3" src="https://github.com/user-attachments/assets/2d10a7fc-6f97-431d-8d70-b62786ee2a60" />
<img width="1919" height="884" alt="photos 1" src="https://github.com/user-attachments/assets/8b46cba2-90a9-4fd8-aa63-f7570229fcd7" />


## 🚀 Prochaines étapes
Le lab évoluera prochainement vers un projet de **Blue Team / Cybersécurité** avec l'intégration d'un SIEM (Wazuh) pour la surveillance des logs et la détection d'intrusions.
