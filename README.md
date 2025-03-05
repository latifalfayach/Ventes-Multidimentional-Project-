# Entrepôt de Données pour un Laboratoire Médical

Ce projet consiste en la création d'un entrepôt de données pour un laboratoire médical, utilisant **Wamp**, **Microsoft SQL Server**, et **Power BI** pour la Business Intelligence (BI). L'objectif est de centraliser, organiser et analyser les données médicales pour faciliter la prise de décision et améliorer l'efficacité opérationnelle.

## Fonctionnalités

- **Centralisation des données** : Collecte et stockage des données provenant de différentes sources du laboratoire médical.
- **Nettoyage et transformation des données** : Préparation des données pour l'analyse en utilisant des scripts SQL et des outils ETL.
- **Visualisation des données** : Création de tableaux de bord interactifs avec Power BI pour suivre les indicateurs clés de performance (KPI).
- **Rapports automatisés** : Génération de rapports périodiques pour les équipes de gestion et les médecins.

## Installation

1. **Installer Wamp** :
   - Téléchargez et installez WampServer depuis [le site officiel](http://www.wampserver.com/).
   - Assurez-vous que les services Apache et MySQL sont en cours d'exécution.

2. **Installer Microsoft SQL Server** :
   - Téléchargez et installez Microsoft SQL Server depuis [le site officiel](https://www.microsoft.com/en-us/sql-server/sql-server-downloads).
   - Configurez une nouvelle instance de base de données pour le projet.

3. **Importer les scripts SQL** :
   - Exécutez les scripts SQL situés dans le dossier `/scripts/` pour créer les tables et insérer les données.

4. **Configurer Power BI** :
   - Ouvrez le fichier `dashboard.pbix` dans Power BI.
   - Configurez la connexion à la base de données SQL Server pour actualiser les données.

## Utilisation

1. **Accéder au tableau de bord** :
   - Ouvrez le fichier `dashboard.pbix` dans Power BI pour visualiser les données.

2. **Gérer les données** :
   - Utilisez les scripts SQL pour ajouter, modifier ou supprimer des données dans la base de données.

3. **Analyser les données** :
   - Utilisez les tableaux de bord Power BI pour suivre les KPI et générer des rapports.

## Structure du Projet

### Explanation of the Structure

- **`VentesMultidimentionalProject.sln`** : Fichier de solution Visual Studio pour gérer le projet.
- **`VentesMultidimentionalProject/`** : Dossier principal contenant tous les fichiers du projet.
  - **`VentesMultidimentionalProject.dwproj.user`** : Fichier contenant les options spécifiques à l'utilisateur.
  - **`VentesMultidimentionalProject`** : Fichier de projet principal.
  - **`Data Warehouse DB`** : Source de données utilisée pour l'analyse.
  - **`Ventes`** : Cube d'analyse pour les données de ventes.
  - **`Dim Time`** : Dimension pour l'analyse temporelle.
  - **`Dim Region`** : Dimension pour l'analyse géographique.
  - **`Dim Produit`** : Dimension pour l'analyse des produits.
  - **`/bin/`** : Dossier contenant les fichiers de déploiement.
  - **`/obj/Development/`** : Dossier contenant les fichiers temporaires de développement.
- **`README.md`** : Ce fichier, contenant la documentation du projet.