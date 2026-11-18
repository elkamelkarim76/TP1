
# TP1 – Comparaison des méthodes de comptage de mots

## Description

Ce TP porte sur le comptage des occurrences de mots dans des fichiers texte de tailles croissantes. Il permet de comprendre le modèle MapReduce et de comparer différentes approches de traitement, de Python classique aux frameworks distribués.

## Objectifs

- Comprendre le principe de MapReduce.
- Implémenter le comptage de mots en Python.
- Simuler les étapes Map, Shuffle et Reduce.
- Utiliser Hadoop MapReduce.
- Découvrir Apache Spark avec PySpark.
- Comparer les performances des différentes méthodes.

## Méthodes étudiées

Les travaux présentent les méthodes suivantes :

1. **Python simple** : comptage à l'aide d'un dictionnaire et d'une boucle.
2. **Pseudo-MapReduce Python** : simulation locale des étapes Map, Shuffle et Reduce.
3. **Hadoop MapReduce** : utilisation de Hadoop pour effectuer le comptage.
4. **PySpark** : utilisation d'Apache Spark avec les opérations RDD `flatMap`, `map` et `reduceByKey`.

## Expérimentations

Les méthodes sont étudiées sur des fichiers de tailles croissantes :
- 10 000 lignes
- 100 000 lignes
- 500 000 lignes
- 1 000 000 lignes

Les résultats sont vérifiés afin de garantir la cohérence des comptages. Les temps d'exécution sont mesurés et comparés à l'aide de tableaux et de graphiques.

## Organisation des fichiers

Le dépôt contient les deux fichiers du TP1 :
- Le premier présente la comparaison entre Python simple, pseudo-MapReduce et Hadoop MapReduce.
- Le deuxième ajoute PySpark à la comparaison et présente une étude des quatre méthodes.

## Exécution

Ouvrir les fichiers dans Jupyter Notebook et exécuter les cellules dans l'ordre.

Les parties Hadoop et PySpark nécessitent un environnement compatible avec leurs dépendances respectives.

## Conclusion

Ce TP permet de comparer plusieurs approches de comptage de mots et de mettre en évidence leurs différences en matière de performances et de mise en œuvre.

Il montre notamment que les outils distribués ont des coûts de démarrage qui peuvent être importants sur de petits fichiers, mais qu'ils sont conçus pour traiter des volumes de données plus importants.
