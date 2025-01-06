# NBA STATS

## Projet qui transforme des données en CSV de basket en table SQL 


### **Pré-requis :**


####
* Connaissance en requête SQL
* Connaissance de Databricks
    * Créer des clusters
    * Lancer des scripts

 
### Je vais vous donner maintenant toutes les étapes à suivre afin de pouvoir manipuler les données


## Etape 1 :

Vous importez le fichier **.dbc** dans votre espace de travail sur Databricks

Ensuite, vous créez un cluster avec cette configuration dans la partie compute sur la sidebar de gauche 

![Compute image](/image/Compute.png)

## Etape 2 :

Sur votre espace de travail, allez sur le notebook **part bronze**, choississez le cluster que vous avez crée précedemment et appuyez sur **Run all**

![Part bronze](/image/PartBronze.png)

Dans cette partie, on recupère nos data depuis Azure afin d'en faire des tables qui seront nettoyés et transformés par la suite.

## Etape 3 : 

Vous allez maintenant dans le dossier **Part_Silver** puis **Init Part Silver**, vous choississez toujours le cluster que vous ave crée puis appuyez sur **Run all**

Ce qui est fait dans le silver est le nettoyage des données, la transformations afin d'avoir des données claires (arrondir les données, les multiplier par 100 etc...) et enfin la fusion de chaque tables d'une même catégorie en 1 seule : Match, Joueur, Equipe
