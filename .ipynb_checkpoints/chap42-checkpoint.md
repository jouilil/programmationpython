# Préparation des données pour data mining

##### 1 Lecture et manipulation de DataFrames avec Pandas.

```{admonition} <font color='blue'>Pandas</font>
:class: tip

La bibliothèque Pandas dispose d’outils pour lire et écrire dans des fichiers de différents formats (.csv, .txt, .xlsx, .sql, .hdf5, etc…).

Une fois Pandas est installé et pour commencer à l’utiliser, vous devez l’importer dans votre script comme suit :

```

```
import pandas as pd
```

###### 1.1 pour les Csv File


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
###### 1.2 pour les Excels File


```
import pandas as pd
# 1ere méthode
path = "C:/Users/LENOVO/Desktop/youness/data1.xlsx"
df= pd.read_excel(path)
# 2ème méthode
df= pd.read_excel("C:/Users/LENOVO/Desktop/youness/data1.xlsx")
```
###### 2.2 Prétraitement des Données







statistiques descriptives, tendances, distribution

##### 3.  Sélection des données dans les dataframes

Pour sélectionner des variables (colonnes) spécifiques dans un DataFrame Pandas, vous pouvez utiliser l'accès par nom de colonne:

- Sélection d'une seule colonne :
```
data = data['Age']
```

- Sélection de plusieurs colonnes par nom
```
data = data[['Nom', 'Salaire']]
```

- Utilisation de loc ou iloc pour la sélection basée sur des conditions ou des indices

```
data = data.loc[:, ['Nom', 'Salaire']]
```
```
data = data.iloc[:, [0, 2]] # permet de sélectionner toutes les lignes (:), mais uniquement les colonnes d'indice 0 et 2.
```

###### 3.1 Par crochets

###### 3.2 Par .iloc

Lorsqu’on veut effectuer une extraction avec les attributs `iloc()`, nous utilisons la syntaxe est la suivante :

**df.iloc[selection_lignes, selection_colonnes]**

`iloc()` repose sur l'utilisation de l'index numérique

```
df= pd.read_excel(path)
print(df.head())
df2=df.iloc[:, [1,4,5]]
print(df2.head())
```

###### 3.3 Par .loc

Lorsqu’on veut effectuer une extraction avec les attributs `loc()`, nous utilisons la syntaxe est la suivante :

**df.loc[selection_lignes, selection_colonnes]**

```
df= pd.read_excel(path)
print(df.head())
df2=df.loc[:, ["Age","Sexe"]]
print(df2.head())
```

`loc()` repose sur l'utilisation de l'index textuel






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



