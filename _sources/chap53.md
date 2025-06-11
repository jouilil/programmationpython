### La dataviz avec Python

##### 1. Vue d’ensemble des bibliothèques Python

Python offre plusieurs bibliothèques puissantes pour la visualisation de données.

```{admonition} Bibliothèques de la visualisation

*Matplotlib*: Base pour la création de visualisations statiques, animées et interactives. Hautement personnalisable avec une documentation complète.

*Seaborn* : Construit sur Matplotlib, il simplifie les visualisations complexes. Se concentre sur la visualisation de données statistiques avec des styles par défaut attrayants.

*Pandas* : Principalement une bibliothèque de manipulation de données, mais fournit également des capacités de traçage intégrées.

```
Ces librairies sont des outils indispensables pour une visualisation efficace des données en Python.


##### 2. Chargement de la base 

```
*Importer un fichier CSV* :

data = pd.read\_csv('chemin\_du\_fichier.csv')

*Importer un fichier Excel*:

data = pd.read\_excel('chemin\_du\_fichier.xlsx', sheet\_name='NomFeuille')

```

```
import pandas as pd

import matplotlib.pyplot as plt

data = pd.read_excel("C:\\Users\LENOVO\Desktop\DZ\change_CE.xlsx")

print(data.head())

data.info()

data.describe()

effectifs = data['PAYS'].value_counts()

frequences= data['PAYS'].value_counts(normalize=True) * 100

tableau_statistique = pd.DataFrame({
        'Effectifs': effectifs,
        'Fréquences (%)': frequences
    })

print(tableau_statistique)
```

```{admonition} Utilité d'un tableaux et un graphique

Pour résumer une information statistique, nous utilisons les tableaux statistiques et/ou les représentations graphiques.
```
```{admonition} Remarque
:class: attention
Le choix du type de l'illustration à mobiliser graphique dépend de la nature des variables étudiées.
```

##### 3. Types de graphiques 

###### Scatter Plot

```
import pandas as pd
import matplotlib.pyplot as plt
 
 
# reading the database
data = pd.read_csv("tips.csv")
 
# Scatter plot with day against tip
plt.scatter(data['day'], data['tip'])
 
# Adding Title to the Plot
plt.title("Scatter Plot")
 
# Setting the X and Y labels
plt.xlabel('Day')
plt.ylabel('Tip')

 
plt.show()

```

######  Line Chart


```
import pandas as pd
import matplotlib.pyplot as plt
 
 
# reading the database
data = pd.read_csv("tips.csv")
 
# Scatter plot with day against tip
plt.plot(data['tip'])
plt.plot(data['size'])
 
# Adding Title to the Plot
plt.title("Scatter Plot")
 
# Setting the X and Y labels
plt.xlabel('Day')
plt.ylabel('Tip')
 
plt.show()
```

######  Bar Chart
```
import pandas as pd
import matplotlib.pyplot as plt
 
 
# reading the database
data = pd.read_csv("tips.csv")
 
# Bar chart with day against tip
plt.bar(data['day'], data['tip'])
 
plt.title("Bar Chart")
 
# Setting the X and Y labels
plt.xlabel('Day')
plt.ylabel('Tip')
 
# Adding the legends
plt.show()
```

######  Histogram
```
import pandas as pd
import matplotlib.pyplot as plt
 
 
# reading the database
data = pd.read_csv("tips.csv")
 
# histogram of total_bills
plt.hist(data['total_bill'])
 
plt.title("Histogram")
 
# Adding the legends
plt.show()
```
