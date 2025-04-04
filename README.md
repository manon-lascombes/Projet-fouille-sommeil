# Projet-fouille-sommeil

Données : https://www.kaggle.com/datasets/rxnach/student-stress-factors-a-comprehensive-analysis

# Description des données



# Objectif du projet

Nous voulons réaliser une classification automatique du niveau d’anxiété chez les étudiants. Pour avoir une classification optimale, nous comparerons les paramètres et les performances de la méthode “arbre de décision” pour trouver les paramètres qui nous permettent d’avoir la meilleure classification pour le niveau d’anxiété des étudiants. 

Pour cela, nous ferons tout d’abord une analyse préliminaire des données, nous regarderons si des variables doivent être exclu de l’analyse, car peu pertinente (ex : trop de valeurs différentes ne permettant pas de séparer nos données en groupes suffisants). Pour ce faire, nous ferons un test de corrélation, afin de voir si certaines variables sont faiblement corrélées à notre variable “anxiety_level”. Nous ferons également un summary pour savoir le nombre de valeurs différentes par variables

Puis, nous regarderons si nos variables ont besoin d’être transformé (ex : transformer nos données quantitatives en qualitative, ou normaliser nos données). Nous devrons transformer notre variable “anxiety_level” en classe afin de pouvoir réaliser la classification. 

Ces étapes nous permettront d’avoir un tableau d’individu variable. 
Puis nous construirons notre modèle sur Knime, nous réaliserons donc un modèle de type arbre de décision. Nous évaluerons ce premier modèle en regardant son taux d’erreur. Puis, nous modifierons les paramètres de ce modèle et à chaque changement, nous déterminerons le taux d’erreur du modèle (avec donc les nouveaux paramètres). Le meilleur modèle sera celui avec les paramètres donnant le taux d’erreur le plus faible. 
