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
#### Observation des données:
Nos données, comme on va le voit dans l'image suivant, est composé d'identifiant(id) pour chaque tweet, de mot clé (keyword) du tweet, de texte (text) qui est le tweet et enfin un target (0 ou 1). les target donne la nature du tweet( urgent==1 et normal==0).
![](/images/text.png)

#### utilisation des méthodes dites classiques: RandomForestClassifier, SVM, et MultinomialNB:
les trois algorithmes cités précedement, sont pratiques pour l'initiation et l'application de la classification sur les NLPs. 
Les algorithmes RandomForestClassifier, SVM (Support Vector Machine) et MultinomialNB (Naive Bayes multinomial) sont des techniques d'apprentissage automatique largement utilisées pour résoudre des problèmes de classification et d'analyse de données. Chacun de ces algorithmes possède ses propres caractéristiques et avantages, les rendant pertinents dans divers contextes. Nous explorerons  chaque algorithme pour le domaine de l'analyse de texte et du traitement du langage naturel.

dans le graphes suivant on peut voir l'éfficacité de chaque modèle(celui qui se rapproche le plus de la réalité):
![](/images/1er%20parti.png)
![](/images/2eme%20partie.png)


[ LIEN DU CODE LA PARTIE: RFC,SVM ET MULTINOMIALNB  ](/codes/CLASSIC.ipynb) 



#### utilisation de Tensorflow et Bert:
autant les trois algorithmes précedement sont sont utiles et pratiques pour un introduction aux NLPs. autant Tensorflow et Bert sont utiles pour comprendre les résaux de neurones profond (deep learning). par conséquent Tensorflow et Bert, nous permetterons d'avoir de meilleurs résultats.
On ne va pas aller trop en profondeur sur Tensorflow et Bert.

les résultats de cette partie, seront les résultats utilisé pour la prédictions finale.

Tensorflow et BERT sont des outils avancés pour l’apprentissage en profondeur (deep learning) et peuvent être utilisés pour des tâches plus complexes. Bien que ces outils puissent offrir de meilleurs résultats, ils nécessitent également une expertise plus avancée pour être utilisés efficacement. Ils sont souvent utilisés pour la classification de texte et d’autres tâches de traitement du langage nature

le graphe suivant montre une amélioration net ( le graphes important est celle de la prédiction prediction_75):


![](/images/tensorflow.png)


[ LIEN DU CODE DE LA PARTIE: TENSORFLOW ET BERT ](/codes/TENSORFLOW.ipynb) 


## CONCLUSION
l'utilisation d'algorithme de classification classic comme RandomForestClassifier, SVM et MultinomialNB, ou les algorithmes du deep learning avec tensorflow et Bert. permet de faire beaucoups de chose comme la classification qu'on a fait et c'est efficace, surtout la partie Deep learning. Mais souvent il faut avoir plus d'efficacité, il y a des domaines comme le nucléaire, la santé  etc.. qui peuvent necessiter une classification plus précise. dans ce cas on peut améliorer les modèles vu plus hauts, sur plusieurs point: travailler sur le futuring ingenering, manipuler les metaparamètres etc... ou encore utiliser plus d'algorithmes récent .



### çi dessous ce trouves les données pour l'apprentissages et la validation du modèle

[-données d'entrainnement ](/DONN%C3%89ES/train.csv) <br>
[-données de test ](/DONN%C3%89ES/test.csv) <br>
[-données résultat(sample_submission) ](/DONN%C3%89ES/sample_submission.csv) <br>


### çi dessous ce trouves les données résultant de notre modèle

[-données prédiction par mon modèle final  ](/DONN%C3%89ES/submission_final.csv)

