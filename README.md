# Projet-fouille-sommeil

Données : https://www.kaggle.com/datasets/rxnach/student-stress-factors-a-comprehensive-analysis

# Description des données
​Le jeu de données intitulé "Student Stress Factors: A Comprehensive Analysis" disponible sur Kaggle comprend 1 100 entrées et 21 variables, explorant divers facteurs influençant le stress chez les étudiants. Ces variables sont regroupées en cinq catégories principales :​

Facteurs psychologiques :

- Niveau d'anxiété : Avec des scores de 0 à 21 (variable quantitative) indiquant des niveaux d'anxiété de minimal à sévère.​


- Estime de soi : Avec des scores de 0 à 30 (variable quantitative) reflétant une estime de soi de faible à élevée.​


- Antécédents de santé mentale : Indique si l'étudiant a des antécédents en santé mentale (0 pour non, 1 pour oui), c’est une variable qualitative (binaire :1/0).​


- Dépression : Avec des scores de 0 à 27 (variable quantitative) représentant des niveaux de dépression de minimal à sévère.​


Facteurs physiologiques :

- Maux de tête : Fréquence des maux de tête, notée de 0 (rarement) à 5 (fréquemment) variable quantitative.​


- Pression artérielle : Classée de 1 (trop basse) à 3 (trop élevée), c’est une variable quantitative.​


- Qualité du sommeil : Auto-évaluation de la qualité du sommeil, de 0 (très mauvaise) à 5 (excellente) est une variable quantitative.​


- Problèmes respiratoires : Notés de 0 (aucun) à 5 (graves) est variable quantitative.​


Facteurs sociaux :

- Soutien social : Niveau de soutien perçu, évalué sur une échelle de 0 à 5 (variable quantitative).​


- Pression des pairs : Degré de pression ressenti de la part des pairs, noté de 0 à 5 (variable quantitative).​


- Activités extrascolaires : Participation à des activités en dehors du cadre académique, évaluée de 0 (aucune) à 5 (très active) est une variable quantitative.​


- Harcèlement : Expérience du harcèlement, notée de 0 (jamais) à 5 (très fréquent) est une variable quantitative.​


Facteurs environnementaux :

- Niveau de bruit : Perception du niveau de bruit dans l'environnement de vie, de 0 (très calme) à 5 (très bruyant), est une variable quantitative.​


- Conditions de vie : Satisfaction concernant les conditions de vie, notée de 0 (très insatisfaisant) à 5 (très satisfaisant), est une variable quantitative.​


- Sécurité : Sentiment de sécurité dans l'environnement de vie, évalué de 0 (très dangereux) à 5 (très sûr), est une variable quantitative.​


- Besoins fondamentaux : Degré de satisfaction des besoins fondamentaux, noté de 0 (pas du tout satisfait) à 5 (entièrement satisfait), est une variable quantitative.​


Facteurs académiques :

- Performance académique : Auto-évaluation des résultats scolaires, de 0 (très mauvais) à 5 (excellent), est une variable quantitative.​


- Charge d'étude : Perception de la charge de travail académique, notée de 0 (très légère) à 5 (très lourde), est une variable quantitative.​


- Relation enseignant-étudiant : Qualité perçue de la relation avec les enseignants, évaluée de 0 (très mauvaise) à 5 (très bonne), est une variable quantitative.​


Préoccupations concernant la carrière future : Niveau d'inquiétude concernant les perspectives de carrière, noté de 0 (pas du tout inquiet) à 5 (très inquiet), est une variable quantitative.

Stress_Level: C’est notre variable cible de type quantitative, (0 = Faible, 1 = Modéré, 2 = Élevé. Elle représente le niveau global de stress de l’étudiant. 

 



# Objectif du projet

Nous voulons réaliser une classification automatique du niveau de stress chez les étudiants. Pour avoir une classification optimale, nous comparerons les paramètres et les performances de la méthode “arbre de décision” pour trouver les paramètres qui nous permettent d’avoir la meilleure classification pour le niveau de stress des étudiants. 

Pour cela, nous ferons tout d’abord une analyse préliminaire des données, nous regarderons si des variables doivent être exclus de l’analyse, car peu pertinente (par exemple : trop de valeurs différentes ne permettant pas de séparer nos données en groupes suffisants, ou bien aucune corrélation avec notre variable d’intérêt). Pour ce faire, nous ferons un test de corrélation, afin de voir si certaines variables sont faiblement corrélées à notre variable “stress_level”. Nous ferons également un summary pour savoir le nombre de valeurs différentes par variables

Puis, nous regarderons si nos variables ont besoin d’être transformés (par exemple : transformer nos données quantitatives en qualitative, ou normaliser nos données). Nous devrons transformer notre variable “stress_level” en classe afin de pouvoir réaliser la classification. 

Ces étapes nous permettront d’avoir un tableau d’individus-variables. 
Puis, nous construirons notre modèle sur Knime, nous réaliserons donc un modèle de type arbre de décision. Nous évaluerons ce premier modèle en regardant son taux d’erreur. Puis, nous modifierons les paramètres de ce modèle et à chaque changement, nous déterminerons le taux d’erreur du modèle (avec donc les nouveaux paramètres). Le meilleur modèle sera celui avec les paramètres donnant le taux d’erreur le plus faible. 
