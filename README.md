# Projet-fouille-sommeil

Données : https://www.kaggle.com/datasets/rxnach/student-stress-factors-a-comprehensive-analysis

# Description des données
​Le jeu de données intitulé "Student Stress Factors: A Comprehensive Analysis" disponible sur Kaggle comprend 1 100 entrées et 20 variables, explorant divers facteurs influençant le stress chez les étudiants. Ces variables sont regroupées en cinq catégories principales :​

Facteurs psychologiques :

  Niveau d'anxiété : Évalué selon l'échelle GAD-7, avec des scores de 0 à 21 ( variable quantitatif ) indiquant des niveaux d'anxiété de minimal à sévère.​


  Estime de soi : Mesurée par l'échelle de Rosenberg, avec des scores de 0 à 30 ( variable quantitatif ) reflétant une estime de soi de faible à élevée.​


  Antécédents de santé mentale : Indique si l'étudiant a des antécédents en santé mentale (0 pour non, 1 pour oui), est un variable Qualitative (binaire : Oui/Non).​


  Dépression : Évaluée via le PHQ-9, avec des scores de 0 à 27 ( variable quantitatif ) représentant des niveaux de dépression de minimal à sévère.​


Facteurs physiologiques :

  Maux de tête : Fréquence des maux de tête, notée de 0 (rarement) à 5 (fréquemment)  variable quantitatif.​


  Pression artérielle : Classée de 1 (trop basse) à 3 (trop élevée), est un variable Qualitatif ordinale (Basse, Normale, Haute).​


  Qualité du sommeil : Auto-évaluation de la qualité du sommeil, de 0 (très mauvaise) à 5 (excellente) est un variable quantitatif.​


  Problèmes respiratoires : Notés de 0 (aucun) à 5 (graves) est variable quantitatif.​


Facteurs sociaux :

  Soutien social : Niveau de soutien perçu, évalué sur une échelle de 0 à 5 ( variable quantitatif ).​


  Pression des pairs : Degré de pression ressenti de la part des pairs, noté de 0 à 5 ( variable quantitatif ).​


  Activités extrascolaires : Participation à des activités en dehors du cadre académique, évaluée de 0 (aucune) à 5 (très active) est un variable quantitatif.​


  Harcèlement : Expérience du harcèlement, notée de 0 (jamais) à 5 (très fréquent) est un variable quantitatif .​


Facteurs environnementaux :

  Niveau de bruit : Perception du niveau de bruit dans l'environnement de vie, de 0 (très calme) à 5 (très bruyant), est un variable quantitatif.​


  Conditions de vie : Satisfaction concernant les conditions de vie, notée de 0 (très insatisfaisant) à 5 (très satisfaisant), est un variable quantitatif.​


  Sécurité : Sentiment de sécurité dans l'environnement de vie, évalué de 0 (très dangereux) à 5 (très sûr), est un variable quantitatif.​


  Besoins fondamentaux : Degré de satisfaction des besoins fondamentaux, noté de 0 (pas du tout satisfait) à 5 (entièrement satisfait), est un variable quantitatif.​


Facteurs académiques :

  Performance académique : Auto-évaluation des résultats scolaires, de 0 (très mauvais) à 5 (excellent).​


  Charge d'étude : Perception de la charge de travail académique, notée de 0 (très légère) à 5 (très lourde), est un variable quantitatif.​


  Relation enseignant-étudiant : Qualité perçue de la relation avec les enseignants, évaluée de 0 (très mauvaise) à 5 (très bonne), est un variable quantitatif.​


  Préoccupations concernant la carrière future : Niveau d'inquiétude concernant les perspectives de carrière, noté de 0 (pas du tout inquiet) à 5 (très inquiet), est un variable quantitatif.



# Objectif du projet

Nous voulons réaliser une classification automatique du niveau d’anxiété chez les étudiants. Pour avoir une classification optimale, nous comparerons les paramètres et les performances de la méthode “arbre de décision” pour trouver les paramètres qui nous permettent d’avoir la meilleure classification pour le niveau d’anxiété des étudiants. 

Pour cela, nous ferons tout d’abord une analyse préliminaire des données, nous regarderons si des variables doivent être exclus de l’analyse, car peu pertinente (par exemple : trop de valeurs différentes ne permettant pas de séparer nos données en groupes suffisants, ou bien aucune corrélation avec notre variable d’intérêt). Pour ce faire, nous ferons un test de corrélation, afin de voir si certaines variables sont faiblement corrélées à notre variable “anxiety_level”. Nous ferons également un summary pour savoir le nombre de valeurs différentes par variables

Puis, nous regarderons si nos variables ont besoin d’être transformés (par exemple : transformer nos données quantitatives en qualitative, ou normaliser nos données). Nous devrons transformer notre variable “anxiety_level” en classe afin de pouvoir réaliser la classification. 

Ces étapes nous permettront d’avoir un tableau d’individus-variables. 
Puis, nous construirons notre modèle sur Knime, nous réaliserons donc un modèle de type arbre de décision. Nous évaluerons ce premier modèle en regardant son taux d’erreur. Puis, nous modifierons les paramètres de ce modèle et à chaque changement, nous déterminerons le taux d’erreur du modèle (avec donc les nouveaux paramètres). Le meilleur modèle sera celui avec les paramètres donnant le taux d’erreur le plus faible. 
