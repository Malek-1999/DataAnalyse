## *Analyze Your Runkeeper Fitness Data* 🚴

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Malek-1999/DataAnalyse/main?labpath=notebook.ipynb)

### :file_folder: Introduction :
Avec l'explosion de la popularité des trackers de fitness, les coureurs du monde entier collectent des données avec des gadgets (smartphones, montres, etc.) pour rester motivés. Ils cherchent des réponses à des questions telles que :

* Quelle a été la vitesse, la durée et l'intensité de ma course aujourd'hui ?
* Ai-je atteint mes objectifs d'entraînement ?
* Est-ce que je progresse ?
* Quelles ont été mes meilleures réalisations ?
* Comment est-ce que je performe par rapport aux autres ?
  
Ce projet analyse les données d'un coureur sur sept ans collectées à partir du dispositif de suivi Runkeeper. Les données sont un fichier CSV où chaque ligne est une seule activité de formation. Dans ce projet, nous allons créer, importer, nettoyer et analyser les données pour répondre aux questions précedents.
![img](./img/image.png)
***
### :clipboard: Les Tâches du projet :
- Obtenir et examiner les données brutes
- Prétraitement des données
- Traiter des valeurs manquantes
- Tracer les données en cours d'exécution
- Statistiques de course
- Préparez les données et créez un graphique.
- Créez un tracé avec la distance observée des pistes et la tendance décomposée.
- Créer un histogramme personnalisé pour la distribution de la fréquence cardiaque
- Créer un rapport de synthèse
***
### :woman_technologist: Analyse des données :
##### :memo: Chargez les données des activités d'entraînement du dataset :
> runkeeper_file = 'datasets/cardioActivities.csv'

![img](./img/tab.png)
##### 📈 Visualisation des données liées à chaque type de course :

![img](./img/4.png)

![img](./img/4.2.png)

##### 📊 Visualisation des moyennes de chaque séance d'entrainement :
Traçons les moyennes à long terme de la distance parcourue et de la fréquence cardiaque avec leurs données brutes pour comparer visuellement les moyennes de chaque séance d'entraînement en utilisant les données de 2015 à 2018.

![img](./img/6.png)

##### 📈 Visualisation de la distance de course annuelle (km) de 2013 à 2018:
Pour se motiver à courir régulièrement, cet utilisateur a fixé comme objectif de courir 1000 km par an:

![img](./img/7.png)
On remarque alors qu'il a atteint son objectif de 1000 km deux fois en 2015 et en 2017.

#####  Est-ce que il est entrain de progresser? 
Pour répondre à cette question, nous allons décomposer la course de distance hebdomadaire et la comparer visuellement aux données brutes. Une ligne de tendance rouge représentera la distance hebdomadaire parcourue
![img](./img/8.png)

##### 📊 Intensité d'entraînement :
La fréquence cardiaque est généralement utilisée pour mesurer l'intensité de l'entraînement. Selon l'âge et le niveau de forme physique, les fréquences cardiaques sont regroupées en différentes zones que les gens peuvent cibler en fonction des objectifs d'entraînement.
Une fréquence cardiaque,lors d'activités d'intensité modérée est d'environ 50 à 70 % de la fréquence cardiaque maximale, tandis que lors d'une activité physique vigoureuse, elle est d'environ 70 à 85 % de la fréquence maximale.
On a eu recourt alors à la création d'un diagramme de distribution des données de fréquence cardiaque par l'intensité d'entraînement.

![img](./img/9.png)

##### :clipboard: Rapport de synthèse détaillé :
Pour ce faire, nous allons créer deux tables :
- Le premier tableau sera un résumé des variables de distance (km) et de dénivelé (m) pour chaque activité d'entraînement. 
- Le deuxième tableau répertorie les statistiques récapitulatives pour les variables de vitesse moyenne (km/h), de montée (m) et de distance (km) pour chaque activité d'entraînement.
###### Table 1 : La distance et la dénivelé pour chaque activité :
![img](./img/10.1.PNG) 
###### Table 2 : Tableau récapitulatif des differentes activités 
![img](./img/10.2.PNG) 
***