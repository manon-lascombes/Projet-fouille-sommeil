# **Documentation d’utilisation du script *Script\_stress\_level.Rmd***

**1\. Prérequis**

Les prérequis permettant d’utiliser le fichier Script\_stress\_level.Rmd dans le but d’un pré-traitement des données contenu dans le fichier StressLevelDataset.csv sont : 

* Avoir au minimum la version 4.2.0 de R   
* Avoir la version 2023.12 de Rstudio (optionnel)  
* Posséder les librairies : corrplot et tidymodels et les activer à l’aide de ces commandes : library(tidymodels) et library(corrplot)  
* Avoir le fichier de donnée : StressLevelDataset.csv

  

## **3\. Étapes pas‑à‑pas**

1. Cloner ou copier le script dans votre projet R ou RStudio.

2. Placer StressLevelDataset.csv à la racine du projet ou ajuster le chemin dans la ligne data ← read.csv(...).

3. Ouvrir Script\_stress\_level.Rmd puis cliquer sur Run puis Run All ou bien exécuter chaque bloc de code ou utiliser tricoter (Knit) pour générer le rapport HTML.

4. Vérifier la sortie de chaque cellule. 

## **4\. Résultats attendus**

Ce script permet de fournir la matrice individus-variables pré-traiter du fichier StressLevelDataset.csv. Nous obtenons donc à la fin de ce script un tableau prêt à traiter. 

 

