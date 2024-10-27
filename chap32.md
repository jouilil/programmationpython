# Les modules en Python

Les modules, également connus sous le nom de bibliothèques ou de librairies en programmation Python, sont des ensembles de programmes qui renferment des fonctions destinées à être fréquemment réutilisées



#### 1.  Création de vos propres modules
Pour créer un module en Python, il vous suffit de créer un fichier avec l'extension .py et d'y écrire votre code Python. Par exemple, si vous voulez créer un module pour le calcul de la surface des formes géométriques, vous pouvez créer un fichier mes_surfaces.py et y définir vos fonctions.


##### 1.1. Création d'un Module pour le Calcul de Surface
Supposons que vous souhaitiez créer un module pour calculer la surface de différentes formes géométriques telles que le carré, le rectangle, le cercle et le triangle.

Créez un nouveau fichier Python appelé surface.py.

Dans ce script, nous définissons les fonctions pour calculer la surface de certaines formes géométriques :

```
import math

def surface_carre(cote):
    return cote ** 2

def surface_rectangle(longueur, largeur):
    return longueur * largeur

def surface_cercle(rayon):
    return math.pi * rayon ** 2

def surface_triangle(base, hauteur):
    return (base * hauteur) / 2

```

##### 1.2. Utilisation du Module dans un Programme Principal

Maintenant que vous avez créé votre module `mes_surface.py`, vous pouvez l'importer et l'utiliser dans un autre programme Python.

Créons un nouveau fichier Python appelé `main.py`.

Dans ce fichier, nous importons le module `mes_surface` et utilisons ses fonctions pour calculer la surface de différentes formes géométriques :

```
import mes_surface

# Calcul de la surface d'un carré
surface_carre = mes_surface.surface_carre(5)
print("Surface du carré :", surface_carre)

# Calcul de la surface d'un rectangle
surface_rectangle = mes_surface.surface_rectangle(4, 6)
print("Surface du rectangle :", surface_rectangle)

# Calcul de la surface d'un cercle
surface_cercle = mes_surface.surface_cercle(3)
print("Surface du cercle :", surface_cercle)

# Calcul de la surface d'un triangle
surface_triangle = mes_surface.surface_triangle(4, 3)
print("Surface du triangle :", surface_triangle)
```

### 2. Modules prédéfinis 

Les modules prédéfinis sont des modules intégrés à Python et disponibles par défaut lors de l'installation de Python. Ils comprennent des modules tels que Numpy, math, random, os, sys, datetime, etc. Ces modules fournissent des fonctionnalités prêtes à l'emploi pour effectuer des opérations mathématiques, générer des nombres aléatoires, manipuler des fichiers et des répertoires, interagir avec le système d'exploitation, gérer la date et l'heure, et bien plus encore.



#### 2.1. math
le module math nous a donné accès aux fonctions trigonométriques sinus et cosinus, et à la constante :

```
import math
math.cos(math.pi / 3)
```

```
import math
math.sin(math.pi / 2)
```


#### 2.2.  Numpy

NumPy introduit un nouveau type l'array qui est semblable à une liste, mais tous les éléments doivent être du même type (entier, flottant, booléen ou encore chaîne de caractères).


NumPy utilisée pour :

- Effectuer des calculs mathématiques et scientifiques

- calculs numériques autour des tableaux multidimensionnels

- Algèbre lnéaire

NumPy est la bibliothèque Python la plus utilisée en Data Science


```python
import numpy as np

# Construction du tableau de type float
tab = np.array([0,1, 2, 3, 4])

# Affichage du tableau
print(tab)
```

```
[0 1 2 3 4]
```
