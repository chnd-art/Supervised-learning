# Détection de fraude
## Introduction
La détection de la fraude est le processus consistant à identifier des enregistrements financiers anormaux au sein d’un ensemble plus large de transactions normales.
Les ensembles de données pour la détection de fraude sont notoirement difficiles d’accès en raison des problématiques liées à la confidentialité des données. Il existe cependant quelques ensembles de données populaires disponibles en ligne, dont celui du ULB Machine Learning Group sur la fraude à la carte bancaire, disponible sur Kaggle, que nous utiliserons tout au long de ce projet.
## Entrainer un modèle d'apprentissage supervisé
### Logistic Regression Model
La régression logistique est un modèle de prédiction qui utilise une fonction logistique pour modéliser la probabilité d'un événement binaire. Contrairement à la régression linéaire qui prédit une variable continue, la régression logistique prédit une variable catégorielle avec deux résultats possibles.

La fonction logistique, également connue sous le nom de fonction sigmoïde, est une fonction mathématique en forme de S qui transforme une valeur réelle en une probabilité comprise entre 0 et 1.
### XGBoost Model
XGBoost (eXtreme Gradient Boosting) est une bibliothèque de machine learning distribuée et open source qui utilise des arbres de décision auxquels est appliqué le boosting de gradient, ce dernier étant un algorithme de boosting d’apprentissage supervisé qui utilise la descente de gradient. Il est connu pour sa vitesse, son efficacité et sa capacité à s’adapter à de grands jeux de données.
## Analyse approfondie
### Ajustement des hyperparamètres
XGBoost possède plusieurs hyperparamètres qui peuvent être ajustés pour améliorer la performance du modèle. Des techniques comme la recherche par grille (Grid Search) ou la recherche aléatoire (Random Search) peuvent aider à trouver le meilleur ensemble d'hyperparamètres.

Hyperparamètres clés :
n_estimators : Nombre de tours de boosting.
learning_rate : Taille du pas utilisée pour éviter le surapprentissage.
subsample : Fraction des échantillons utilisés pour ajuster les apprenants de base individuels.
colsample_bytree : Fraction des caractéristiques utilisées pour ajuster les apprenants de base individuels.
### Autre Modèles potentiels pour comparaison 
Forêt aléatoire (Random Forest) : Une méthode d'ensemble qui peut traiter des données déséquilibrées et fournir l'importance des caractéristiques.

Réseaux de neurones : Des modèles d'apprentissage profond qui peuvent capturer des motifs complexes dans les données.

En suivant ces stratégies et en améliorant continuellement le modèle, nous pouvons obtenir un système de détection de fraude plus robuste et précis, contribuant ainsi à prévenir les pertes financières dues aux transactions frauduleuses.













