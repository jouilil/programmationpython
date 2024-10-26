# Les fonctions en Python

Une fonction correspond à un ensemble d’instructions créées pour effectuer une tâche précise. Autrement dit, une fonction (ou function ) est une suite d'instructions que l'on peut appeler avec un nom. On distingue entre deux types :

- Les fonctions prédéfinies 

- Les fonction définies par l’utilisateur



#### Les fonctions prédéfinies Python

Les fonction prédéfinies sont des fonctions déjà créées et mises à la disposition de l'utilisateur par Python par exemple :

- `dict()`

- `print()`

- `len()`

- `type()`

- ...etc.


#### Les fonctions définies par l’utilisateur


La syntaxe Python pour la définition d’une fonction est la suivante :

```
def nom_fonction(liste de paramètres):
      bloc d'instructions
```

Commençons par voir un exemple d'une fonction qui calcule le carrée d'un nombre

``` 
def carree(x):
    return x**2
```

```
carree(2)
4
```

La fonction carree admet donc un paramètre x. Elle calcule ensuite le carrée qui est le résultat que doit produire la fonction. Pour signaler cela, on utilise le mot réservé `return` qui permet de définir la valeur de retour d'une fonction.

Il est d'ailleurs possible d'utiliser plusieurs paramètres:


```
def somme_deux(x, y):
    return x+y
```

```
somme_deux(10, 9)
19
```

#### Exercices d'application

```{admonition} Exercice
:class: warning
Écrire une fonction en Python appelée calculer_produit qui prend deux paramètres, a et b, et renvoie le produit de ces deux nombres. 

Ensuite, écrivez un programme principal qui demande à l'utilisateur d'entrer deux nombres, appelle la fonction calculer_produit avec ces nombres, puis affiche le résultat.
```


```{admonition} Exercice
:class: warning

Écrire une fonction appelée calculer_surface_triangle qui prend la longueur de la base et la hauteur d'un triangle en paramètres et renvoie la surface du triangle.

Ensuite, écrivez un programme principal qui demande à l'utilisateur d'entrer la longueur de la base et la hauteur d'un triangle, appelle la fonction calculer_surface_triangle avec ces valeurs, puis affiche la surface résultante.
```

