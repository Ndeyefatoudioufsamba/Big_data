# Programmation fonctionnelle avancée (Scala, Apache Spark)

**Author** : Djibril MBOUP, PhD
**Role** : Data Scientist at Atos Senegal
**E-mail** : mboupdjibril.m2itic@gmail.com

## Objectifs

Dans ce cours nous allons :

* Voir les bases de la programmation fonctionnelle en Scala,
* Apprendre à manipuler les concepts avancées de collections, classes, higher-order functions, pattern matching, mapReduce etc.
* Developper des programmes paralleles avec Apache Spark pour le pré-traitement des données dans un cluster Hadoop
* Etudier comment assurer le chargement, l'extraction et la transformation des données avec Spark Dataframe, SQL et Datasets.
* Traiter de données en Streaming
* Developper des modèles Machine Learning en utilisant la Spark MLlib

## Installation de Scala

Vous pouvez installer Scala à partir de :

* Créer une machine virtual Ubuntu dans Virtualbox
* Installer Java JDK 11 (https://adoptopenjdk.net/)
* Installer SDKMAN (https://sdkman.io/usage)
  * `curl -s "https://get.sdkman.io" | bash`
  * `source "$HOME/.sdkman/bin/sdkman-init.sh"`
  * `sdk version`
* 
* Installer avec SDK
  * `sdk install java` # Si vous n'avez pas installé java avec adoptopenjdk
    * `sdk install sbt`
  * `sdk install scala`

## Installation de Apache Spark

* Installer Spark avec SDKMAN

  * `sdk install spark 3.3.1`
* Installer Anaconda ou Miniconda (https://www.anaconda.com/products/individual)
* Copier le dossier apache_spark_data_processing dans votre $HOME ubuntu

  * `cd $HOME/apache_spark_data_processing`
* créer un environnement virtual python dans conda

  * `conda env create -f environment.yml`
  * `conda activate pySpark`
* Installer spylon-kernel pour connecter jupyter avec Spark-shell

  * `cd `
  * `python -m spylon_kernel install --user`
* Créer une variable d'environnement SPARK_HOME dans .bashrc ou bash_profile

  * copier `export SPARK_HOME=$HOME/.sdkman/candidates/spark/3.3.1` dans .bashrc et enregistrer
  * taper la command `source .bashrc`
* Démarrer jupyter notebook ou jupyter lab pour tester

  * `cd $HOME/apache_spark_data_processing`
  * `jupyter lab` ou `jupyter notebook`
  
* Vous pouvez aussi créer un compte Databricks (https://databricks.com) pour travailler dans un cluster Spark en mode Try.
  #   t e s t    
 