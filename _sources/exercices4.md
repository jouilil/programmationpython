# Python pour la Data Mining 

![Drag Racing](datamining.png)


Dans ce quatrième chapitre, nous allons explorer les possibilités d'exploration de données (data mining)

- Découvrir les objets Pandas DataFrame

- Calculer avec la bibliothèque Pandas

- Manipuler des données et les valeurs particulières

- Concaténer différentes sources de données

- Fusionner différentes sources de données

- Visualisation graphique des données grâce à la librairie Matplotlib

##### 1. Introduction à la Data Mining avec Python

##### 2.  Manipulation et Exploration de Données

###### 2.1 Lecture et manipulation de DataFrames avec Pandas.

```{admonition} <font color='blue'>Pandas</font>
:class: tip

La bibliothèque Pandas dispose d’outils pour lire et écrire dans des fichiers de différents formats (.csv, .txt, .xlsx, .sql, .hdf5, etc…).

Une fois Pandas est installé et pour commencer à l’utiliser, vous devez l’importer dans votre script comme suit :

```
import pandas as pd
```
```

```
import pandas as pd

# Specify the path to your CSV file
csv_file_path = 'path/to/your/file.csv'

# Read the CSV file into a pandas DataFrame
df = pd.read_csv(csv_file_path)


```

```{admonition} Exemple
:class: tip
path= "C:/Users/LENOVO/Desktop/youness/Classeur1.csv"

data=pd.read_csv(path, sep=';')
```

###### 2.2 Prétraitement des Données


```{admonition} Sélection des données
:class: tip
Pour sélectionner des variables (colonnes) spécifiques dans un DataFrame Pandas, vous pouvez utiliser l'accès par nom de colonne:

- Sélection d'une seule colonne :
data = data['Age']

- Sélection de plusieurs colonnes par nom
data = data[['Nom', 'Salaire']]

- Utilisation de loc ou iloc pour la sélection basée sur des conditions ou des indices

data = data.loc[:, ['Nom', 'Salaire']]

data = data.iloc[:, [0, 2]] # permet de sélectionner toutes les lignes (:), mais uniquement les colonnes d'indice 0 et 2.

```


statistiques descriptives, tendances, distribution

##### 3.  Analyse exploratoire des données 

##### 4. Visualisation de données avec Matplotlib et Seaborn

##### 5. Régression avec Python

###### 5.1 Régression linéaire simple

###### 5.2 Régression linéaire multiple

##### 6. Exercices

##### 7. Projets pratques




