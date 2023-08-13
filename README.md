# Presentation d'un projet sur les_NLPs
#### *Mon premier Projet sur les NLPs, pour mon mémoire de fin d'année  master 1 (2022-2023)*


## Mise en œuvre et Github :

Pour rendre ma stratégie et mes codes accessibles à tous, j'ai créé cette page Github. 

Sur cette page vous trouverez :
la description  de ma stratégie et un lien vers mon mémoire pour plus de détails, expliquant les raisons derrière chaque choix méthodologique.
dans le mémoire on y trouve la préparation des données, la modélisation avec les méthodes classiques, ainsi que l'utilisation de Tensorflow et Bert. Les résultats obtenus à chaque étape, y compris les performances des différents modèles.
Dans cette page il y'a aussi les liens vers des notebooks Jupyter pour chaque méthode, les liens vers les données d'apprentissage, de test et vers les résultats de prédiction générés par mon modèle final.
Je suis engagé à maintenir et mettre à jour cette page pour assurer sa pertinence et son utilité à la fois pour le challenge et pour ceux qui souhaitent en apprendre davantage sur les méthodes d'analyse de données et de traitement du langage naturel.

Je remercie mes professeurs pour cette opportunité passionnante et j'attends avec impatience vos commentaires et suggestions.

Cordialement,
Nasseme Ahamed

## MÉMOIRE
[LIEN VERS LE MÉMOIRE ](memoireupdate.pdf)

## INTRODUCTION
le sujet de notre de notre exercice est tiré d'un challenge Kaggle: [Natural Language Processing with Disaster Tweets 
(Traitement automatique du langage naturel avec des tweets de catastrophe)](https://www.kaggle.com/competitions/nlp-getting-started).
on est amené à présenter un algorithme de classification de tweets en catégories "urgent" et "normal". Nous proposerons plusieurs approches de classification afin de résoudre cette problématique.

Le plan de developement de notre projet peu ce diviser en 3 grandes parties:
 - l'observation des données
 - l'utilisation des méthodes dites classiques: RandomForestClassifier, SVM,et MultinomialNB.
 - l'utilisation de Tensorflow et Bert
   
En effet les premiers algorithmes qu'on va utiliser, nous permetterons d'avoir une première vision globale des problématique et solutions des NLPs.
À travers Bert et tensorflow on va pouvoir utiliser l'approche du problème avec le Deep Learning. c'est les résultats de Tensorflow et Bert qu'on va retenir pour la réponse final du problème, du fait de la robustesse des algorithmes de Tensorflow et Bert Par rapport aux premiers algorithmes.

## DÉVELOPPEMENT 
#### Observation des données:
Nos données, comme on va le voir dans l'image suivante, sont composées d'identifiant(id) pour chaque tweet, d' un mot clé (keyword) et du lieu d'émission (location), aussi du texte (text) qui est le tweet lui même et enfin un target (0 ou 1). les target donne la nature du tweet( urgent==1 et normal==0). Cette étape m'a permis de comprendre la nature du problème et les caractéristiques des données
![](/images/text.png)

#### utilisation des méthodes dites classiques: RandomForestClassifier, SVM, et MultinomialNB:
RandomForestClassifier, SVM et MultinomialNB, sont pratiques pour l'initiation et l'application de la classification sur les NLPs. 
Les algorithmes RandomForestClassifier, SVM (Support Vector Machine) et MultinomialNB (Naive Bayes multinomial) sont des techniques d'apprentissage automatique largement utilisées pour résoudre des problèmes de classification et d'analyse de données. Chacun de ces algorithmes possède ses propres caractéristiques et avantages, les rendant pertinents dans divers contextes. Nous examinerons individuellement chaque algorithme dans le contexte de l'analyse de texte et du traitement du langage naturel.

Dans le graphique suivant, on peut observer l'efficacité de chaque modèle et identifier celui qui se rapproche le plus de la réalité :
![](/images/rfc.png)
![](/images/svm.png)


[ LIEN DU CODE DE LA PARTIE: RFC,SVM ET MULTINOMIALNB  ](/codes/CLASSIC.ipynb) 



#### utilisation de Tensorflow et Bert:
Les trois algorithmes précédents sont particulièrement utiles et pratiques pour les introductions aux NLP. En revanche, Tensorflow et BERT se révèlent particulièrement utiles pour saisir les rouages des réseaux de neurones profonds, ce qui les rend essentiels à la quête de performances optimales. 
Les résultats obtenus à l'issue de cette phase alimenteront nos prédictions finales.

Tensorflow et BERT se distinguent en tant qu'outils avancés dans le domaine de l'apprentissage en profondeur (deep learning) et sont adaptés aux tâches complexes. Cependant, leur exploitation requiert une expertise plus poussée pour être véritablement efficace. Ces outils sont fréquemment mobilisés pour des tâches de classification textuelle et d'autres défis liés au traitement du langage naturel.

Le graphique suivant illustre une nette amélioration, avec l'accent mis sur la pertinence de la prédiction (le graphe de la prédiction finale est symbolisé par la courbe prédiction_75) :


![](/images/tensorflow.png)


[ LIEN DU CODE DE LA PARTIE: TENSORFLOW ET BERT ](/codes/TENSORFLOW.ipynb) 


## CONCLUSION
L'utilisation d'algorithmes de classification classiques tels que RandomForestClassifier, SVM et MultinomialNB, ainsi que les algorithmes de deep learning avec Tensorflow et BERT, a démontré leur potentiel étendu, notamment dans la classification que nous avons entreprise. En particulier, la composante de deep learning s'est avérée particulièrement efficace. 
Cependant, dans des domaines exigeants tels que le nucléaire et la santé, où une classification précise est cruciale, il est souvent nécessaire d'atteindre un niveau supérieur d'efficacité.
Dans de tels cas, l'amélioration des modèles présentés ci-dessus peut être entreprise selon plusieurs axes : en affinant l'ingénierie des fonctionnalités futures(features ingeneering), en ajustant les méta-paramètres etc.. . ou en explorant davantage d'algorithmes récents. Ces approches offrent des opportunités pour améliorer encore davantage la précision et la pertinence des classifications, tout en ouvrant la voie à une application plus étendue dans des domaines sensibles et exigeants.



### Ci-dessous se trouvent les données utilisées pour l'apprentissage et la validation du modèle.

[-données d'entrainnement ](/donnees/train.csv) <br>
[-données de test ](/donnees/test.csv) <br>
[-données résultat(sample_submission) ](/donnees/sample_submission.csv)  <br>


### çi dessous se trouvent les données résultant de notre modèle

[-données prédiction par mon modèle final  ](/donnees/submission_final.csv)

