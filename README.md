# Presentation de l'exercice sur les_NLP
#### *Mon premier Projet sur les NLPs, pour mon mémoire de fin d'année  master 1 (2022-2023)*

## INTRODUCTION
le sujet de notre de notre exercice est tiré d un challenge Kaggle: [Natural Language Processing with Disaster Tweets 
(Traitement automatique du langage naturel avec des tweets de catastrophe)](https://www.kaggle.com/competitions/nlp-getting-started/overview).
on est amené à donner un algorithme de classification de tweet, en tweet urgent et  normal. On va donner plusieurs algorithmes de classification pour la résolution du problème.

Le plan de developement de notre projet peu ce diviser en 3 grandes parties:
 - l'observation des données
 - l'utilisation des méthodes dites classiques: RandomForestClassifier, SVM,et MultinomialNB.
 - l'utilisation de Tensorflow et Bert
   
en effet les premiers algorithmes qu'on va utiliser, nous permetterons d'avoir une première vision globale des problématique et solutions des NLPs.
la deuxième partie, qui va être d'une importance capitale, car c'est celle qu'on va rétenir les résultat, du fait de la robustesse des algorithmes de Tensorflow et Bert.

## DÉVELOPPEMENT 
#### Observation:
Nos données, comme on va le voit dans l'image suivant, est composé d'identifiant(id) pour chaque tweet, de mot clé (keyword) du tweet, de texte (text) qui est le tweet et enfin un target (0 ou 1). les target donne la nature du tweet( urgent==1 et normal==0).




