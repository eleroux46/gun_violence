# gun_violence

Voici le projet réalisé par Matis Bruneau, Matthieu Grenier et Eloïse Leroux dans le cadre du cours Python pour la data science de deuxième année de l’ENSAE dispensé par Lino Galiana.
## Objectif du projet
Au cours de ce projet, nous essayons de fournir des éléments de réponse autour de la question de la violence par armes à feu aux Etats-Unis. Autrement dit, est-il possible d'identifier certains facteurs à l'origine de ces indicidents ? Deux questions majeures traversent cette analyse : 1) Peut-on prédire la fréquence de ces incidents ? 2) Peut-on prédire les conséquences humaines et matérielles de ces incidents ?
## Méthodologie suivie
### 1 – Récupération et traitement des données 
Dans le cadre de ce projet, nous collectons principalement des données en Open Data venant de sources variées : Gun Violence Archive (source des données récupérées sur le Github https://github.com/jamesqo/gun-violence-data), des données nationales américaines (FRED, Census Bureau, FBI) et d’autres sources en accès libre (Boston University School of Public Health, Github Fox News). 
Par la suite, il a fallu nettoyer les différentes bases de données, que ce soit pour convertir des données dans un format lisible (dictionnaire, liste) malgré les erreurs d’encodage ou pour pouvoir harmoniser des noms de comté afin de fusionner les différentes bases.
### 2 et 3 - Visualisation et analyse descriptive 
Dans cette partie, nous nous attachons à faire des statistiques descriptives pour décrire au mieux les données disponibles, que ce soit au niveau des caractéristiques des incidents par arme à feu ou au niveau des variables socio-démographiques, économiques et politiques des comtés ou Etats correspondant à ces incidents. 
Notre visualisation s’intéresse donc d’abord à la distribution fréquentiste de nos variables puis ensuite à une visualisation cartographique. 
Nous nous intéressons également à l’analyse de corrélation entre nos variables principales, que ce soit pour justifier du choix de l’utilisation d’une variable quelle que soit l’année ou pour commencer à essayer de prédire la fréquence ou les conséquences des incidents par arme à feu.
### 4 – Modélisation 
Nous proposons ici un modèle linéaire ayant pour objectif de prédire le nombre d'incidents par armes à feu allant survenir dans chaque comté, ainsi que le nombre de morts et le nombre de blessés à la suite d’un incident.
Nous effectuons également une analyse par Lasso pour vérifier que toutes les variables contribuent à la baisse de l'erreur quadratique moyenne.
### 5 – Conclusion 

## Fonctionnement 
Le notebook principal est le main.ipynb qui permet de visualiser les résultats des autres notebooks à l’aide de la commande %run.