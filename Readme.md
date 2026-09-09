# 🎮 **PokemonMonster**  
**Un projet WPF en C# inspiré du système de combat Pokemon**  

## 📜 **Description du projet**  
**PokemonMonster** est une application développée en **C#** avec **WPF** (Windows Presentation Foundation). L'objectif est de recréer, dans une version simplifiée, le **système de combat Pokemon**, avec des fonctionnalités clés pour rendre l'expérience interactive et agréable.  

---

## 🎥 **Démonstration du projet**

Vous pouvez voir une vidéo de démonstration du projet ici :
[![Watch the video](https://img.youtube.com/vi/05NEGC9uOxA/0.jpg)](https://www.youtube.com/embed/05NEGC9uOxA)

--- 

### 🚪 **Fonctionnalités principales**  

1. **Authentification**  
   - Le projet démarre par une **page de connexion** où les utilisateurs peuvent s'authentifier ou s'inscrire.  

2. **Catalogue de Pokemon**  
   - Accédez à une liste des **151 premiers Pokemon**.  
   - Chaque Pokemon est jouable !  
   - Consultez leurs statistiques et capacités associées.  

3. **Catalogue de capacités**  
   - Parcourez une liste des **attaques (ou capacités)** disponibles.  
   - Consultez le détail de chaque capacité et les Pokemon pouvant l'utiliser.  

4. **Système de combat**  
   - Choisissez un Pokemon en cliquant sur **« Play »**.  
   - Affrontez des adversaires sélectionnés aléatoirement.  
   - **Progression dynamique** : après trois victoires, les adversaires reçoivent un **bonus de dégâts ou de vie**, rendant le jeu plus difficile.  

5. **Navigation simple et intuitive**  
   - Une **barre de navigation** en haut de l'écran permet de basculer facilement entre les pages :  
     - Liste des Pokemon  
     - Liste des capacités  
     - Page de combat  

---  

### 🧩 **Architecture et modèle MVVM**  
Le projet suit le patron **MVVM (Model-View-ViewModel)** dans la plupart des cas. Cependant, certaines exceptions, comme la **logique de navigation**, sont directement intégrées dans les vues par souci de simplicité.  

---  

## 🚀 **Installation et mise en route**  

### **Prérequis**  
- **Git** (pour cloner le dépôt)  
- **C#**  
- **SQL Server** (pour la base de données)  
- Un **IDE compatible avec C#**, comme **Visual Studio**  

---  

### **Étapes d'installation**  

1. **Créer la base de données**  
   - Créer une base de données locale nommée **`ExerciceMonster`**.  
   - Les **tables et données** seront générées automatiquement au lancement du projet, aucune configuration manuelle n'est nécessaire.  

2. **Cloner le dépôt**  
   - Cloner le projet sur votre machine via un terminal :  
     ```bash
     git clone https://github.com/fl-hugo/PokemonMonster
     ```  

3. **Configurer la connexion à la base de données**  
   - Ouvrir le projet dans **Visual Studio** ou un IDE équivalent.  
   - Modifier le fichier `RepositoryBase.cs` situé dans le dossier **Repositories**.  
   - Mettre à jour la valeur **`_connectionString`** pour qu'elle corresponde à votre base locale. Exemple pour **SQLEXPRESS** :  
     ```csharp
     _connectionString = "Server=localhost\\SQLEXPRESS; Database=ExerciceMonster; Trusted_Connection=True; TrustServerCertificate=True;";
     ```  

4. **Lancer le projet**  
   - Compiler et lancer le projet depuis votre IDE.  
   - Attendre l'apparition de la **page d'accueil**. Vous êtes prêt à jouer ! 🎉  

---  

### **Remarque**  
J'ai tenté de mettre en place une page de configuration dynamique (`DatabaseConnectionView.xaml`) pour faciliter la configuration de la connexion à la base de données sans modifier le code source. Cependant, cette fonctionnalité n'est pas encore opérationnelle dans la version actuelle du projet.  

---  

## 🛠️ **Technologies utilisées**  
- **Langage** : C#  
- **Framework** : WPF  
- **Base de données** : SQL Server  
- **Architecture** : MVVM  

---  

## 🎯 **Améliorations futures**  
- Finaliser la configuration dynamique de la connexion à la base de données.  
- Mettre en place un système de sauvegarde de la progression.  
- Optimiser l'interface utilisateur pour une meilleure expérience.  
- Ajouter davantage de complexité au système de combat (effets de sorts comme la brûlure, types de Pokemon et de capacités, statistiques des monstres).  
- Améliorer le design de l'application en ajoutant fluidité et animations.  

---  

## 🧑‍💻 **Auteur**  
Développé par **Flandrin Hugo** dans le cadre d'un projet pédagogique à **Ynov Lyon**.  

---  

### 🚀 **Profitez bien du jeu !**  
