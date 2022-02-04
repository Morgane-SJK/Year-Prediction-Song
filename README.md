# Year-Prediction-Song

**Date de réalisation :** Janvier 2021

**Cadre du projet :** Cours "Python for Data Analysis" en 4ème année à l’ESILV (2ème année du cycle ingénieur), réalisé en groupe avec Nicolas et Louis-Raphael

**Langage utilisé :** Python

## Présentation du projet

Il s’agit de l’étude du dataset YearPredictionMSD, qui est un sous-dataset de Million Song Dataset. 
Celui-ci contient des caractéristiques audios de musiques avec leur année de sortie. 

Voici le lien pour télécharger les données : https://archive.ics.uci.edu/ml/datasets/YearPredictionMSD

Le projet est divisé en 3 parties : 
-	Tout d’abord une analyse des données avec différents types de visualisation.
-	L’implémentation et la comparaison de plusieurs modèles de prédiction pour la date de sortie des musiques.  Pour cela nous avons considéré que notre problème pouvait se résoudre avec des modèles de classification : nous souhaitons prédire la décennie de sortie de la musique et non pas l’année, afin d’avoir moins de classes et obtenir des modèles plus performants.

Les deux premières parties du projet sont accessibles via le Notebook *Python_Project_VF.ipynb*.

-	La dernière partie est la transformation du meilleur modèle que nous avons trouvé en API Flask. Celle-ci permet d’afficher la décennie de sortie d’une musique pour laquelle nous devons renseigner toutes les caractéristiques audios nécessaires. 

Le fichier *Rapport_final.pdf* contient la présentation détaillée du projet : des explications sur les visualisations de données obtenues, le choix du modèle sélectionné pour nos prévisions ainsi qu’une brève présentation du fonctionnement de l’API. 

 
## Lancement de l’API Flask

Dans le dossier API_Part, le fichier *requirements.txt* contient toutes les bibliothèques nécessaires au lancement de l’API.

Pour les installer il vous suffit de lancer la commande `pip install -r requirements.txt` dans votre terminal.

Ensuite vous pouvez exécuter le fichier `app.py` et accéder à l’interface : http://127.0.0.1:5000/
