# Manipulation de listes en Python
#### 1. Création

Sous Python, on peut aussi définir une liste comme une collection d’éléments séparés par des virgules, l’ensemble étant enfermé dans des crochets `[ ]`. 

Les éléments de la liste peuvent être de n’importe quel type. Voici un exemple d’un liste en python :


```
# Créer une liste vide
liste = []

```

```
[]
```

```
jour_et_nombre = ['lundi', 'mardi', 'mercredi', 'jeudi', 'vendredi', 'samedi', 'dimanche', 0, 1, 5]
print(jour_et_nombre)
```
Affichage après exécution :

```
['lundi', 'mardi', 'mercredi', 'jeudi', 'vendredi', 'samedi', 'dimanche', 0, 1, 5]
```


Lorsqu’on dit que les éléments d’une liste peuvent contenir n’importe quel type, on ne rigole pas !! Voici une illustration :

```
# on peut avoir une liste contenant des listes comme des éléments
# une première liste
list1 = [1, 3, 'bonjour']

# une deuxième liste
list2 = [None, True, 3+2j, '']

# une troisième liste contenante list1 et list2 comme éléments
list3 = [list1, list2]

# une quatrième liste contenante list1, list2, et list3 comme éléments
list4 = [list1, list2, list3]

# afficher les listes
print(list1)
print(list2)
print(list3)
print(list4)
```

Affichage après exécution :
```
[1, 3, 'bonjour']
[None, True, (3+2j), '']
[[1, 3, 'bonjour'], [None, True, (3+2j), '']]
[[1, 3, 'bonjour'], [None, True, (3+2j), ''], [[1, 3, 'bonjour'], [None, True, (3+2j), '']]]
```


#### 2. Opérations sur les listes

L’opérateur `+` permet d’ajouter deux listes ensemble pour former une troisième liste :

```
ma_liste = [0, 1, 2] + [10, 20, 30]
print(ma_liste)
```
Pour savoir si un élément est présent dans une liste donnée, on peut utiliser le mot-clé `in` :
```
ma_liste = [0, 1, 2, 12, 0, 20, 30]
print(2 in ma_liste)
print(19 in ma_liste)
```

```
True
False
```

##### 2.1 La fonction len()

La fonction intégrée len(), que nous avons déjà rencontrée à propos des chaînes, s’applique aussi aux
listes. Elle renvoie le nombre d’éléments présents dans la liste :

```
list1 = [1, 3, 'bonjour']
print(len(list1))
```

##### 2.2 La fonction type()

```
#
jour_et_nombre = ['lundi', 'mardi', 'mercredi', 'jeudi', 'vendredi', 'samedi', 'dimanche', 0, 1, 5]

#
print(type(jour_et_nombre))
```
Affichage après exécution :
```
['lundi', 'mardi', 'mercredi', 'jeudi', 'vendredi', 'samedi', 'dimanche', 0, 1, 5]
<class 'list'>
```

##### 2.3 La fonction range()

Si vous avez besoin de créer sur une suite d’entiers, vous pouvez utiliser la fonction list(range()). Elle génère une suite arithmétique.

**syntaxe** = `list(range(valeur_initiale, borne_de_fin, pas))`



```python
a= list(range(10))
print(a)

```

Affichage après exécution :
```
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
```

Il ) noter qu'il est possible de faire commencer l’intervalle à un autre nombre, ou de spécifier un incrément différent (même négatif) :

```python
b= list(range(1, 100, 4))
print(b)

```
Affichage après exécution :

```
[1, 5, 9, 13, 17, 21, 25, 29, 33, 37, 41, 45, 49, 53, 57, 61, 65, 69, 73, 77, 81, 85, 89, 93, 97]
```

```{admonition} Exercice
:class: warning 
Créer une liste contenant les entiers allant de 1997 à 2024.
```

```{admonition} Exercice
:class: warning 
Créer une liste contenant les entiers impairs inférieur à 20.
```
```{admonition} Exercice
:class: warning 
Créer une liste contenant les entiers pairs inférieurs ou égale à 20.
```

##### 2.4  La fonction append()

Il est également possible d’ajouter un élément à une liste, à l'aide de la fonction append()
```
liste = ['samedi', 'dimanche', 0, 1, 5]
liste.append("lundi")
print(liste)
```

##### 2.5 La fonction insert()

Cette fonction insère une nouvelle valeur dans la liste courante, à la position spécifiée en paramètre

```
# Une liste initiale
data = [15, 20, 50, 19]    
print(data) 

# On y ajout des valeurs 
data.insert(1, 15)
data.insert(3, 25)
print(data)

```
Après exécution :
```
[15, 20, 50, 19]
[15, 15, 20, 25, 50, 19]
```

##### 2.6 La fonction del(), remove() \& pop()

Pour supprimer un élément d'une liste donnée on peut utiliser :

- `del()` : est une fonction intégrée permet de supprimer d’une liste un élément quelconque (à partir de son index).

- `pop()` : Enlève de la liste l’élément situé à la position indiquée et le renvoie en valeur de retour. Si aucune position n’est  spécifiée, pop() enlève et renvoie le dernier élément de la liste.

```
liste = ['samedi', 'dimanche', 0, 1, 5]
del(liste[2])
print(liste)
liste.pop(2)
print(liste)
```

- Il aussi est possible de supprimer une entrée d'une liste avec sa valeur avec la fonction `remove` .

```
liste.remove('dimanche')
```

##### 2.7 La fonction count

Pour compter le nombre d'occurences d'une valeur, on peut utiliser la fonction `count`
```
liste2=["o","Ali","O",1,3,0,"o", 7,10]
liste2.count('o')
```

Affichage après exécution :

```
2
```

##### 2.8 La fonction index

La fonction `index` vous permet de connaitre la position de l'item cherché.

Pour compter le nombre d'occurences d'une valeur, on peut utiliser la fonction `index`
```
liste2=["o","Ali","O",1,3,0,"o", 7,10]
liste2.index('Ali')
```
Affichage après exécution :

```
1
```
##### 2.9 La fonction sort

Elle permet d'ordonner les éléments dans la liste.

```
liste2= [2,8,9,0,5,8,9]
liste2.sort()
```
Affichage après exécution :

```
[0, 2, 5, 8, 8, 9, 9]
```

##### 2.10 La fonction reverse
Elle permet d'inverser l'ordre des éléments dans la liste.

```
liste2= [2,8,9,0,5,8,9]
liste2.reverse()
```
Affichage après exécution :

```
[9, 8, 5, 0, 9, 8, 2]
```

##### 2.11 La fonction copy

Pour copier une liste de cette manière adéquate, il est recommandé d'utiliser la fonction `copy()`
```
liste2= [2,8,9,0,5,8,9]
x=liste2.copy()
x
```
Affichage après exécution :

```
[2, 8, 9, 0, 5, 8, 9]
```

##### 2.12 Minimum, maximum et somme

Les fonctions suivantes : `min()`, `max()` et `sum()` renvoient respectivement le minimum, le maximum et la somme d'une liste passée en argument.

- Pour connaître le plus grand élément d’une liste : `max()`

- Pour connaître le plus petit élément d’une liste : `min()`

- Pour sommer les éléments d’une liste : `sum()`

```
liste = [0, 1, 5,3,88,10,3, 2,0,8]
print(max(liste))
print(min(liste))
print(sum(liste))
```

Affichage après exécution :

```
88
0
120
```







#### 3. Slicing \& Indexing

Une `slice` permet de découper des structures de données séquentielles, telles que  :

- les chaînes de caractères

- les listes.

Les `slices` sont des expressions en Python qui permettent d'extraire des éléments d'une liste ou d'une chaîne en une seule ligne de code


##### 3.1 Indiçage

Une liste peut être indexée avec des nombres positifs et/ou négatifs.

- Pour les indices positifs, on commence par 0.

- Pour les indices négatifs, on commeence par -1. Les indices négatifs reviennent à compter à partir de la fin


![Drag Racing](indices.JPG)

##### 3.2. Slices 

###### 3.2.1 Slices avec deux indices


**syntaxe** : Object `[start:end]`

```
chaine = "Université"
print(chaine[0])
print(chaine[2])
print(chaine[0:2])
#Indices négatifs
print(chaine[-1])
print(chaine[-2:-9])
```

```
U
i
Un
é
```

```
list2 = [3,4,5,6,7,8,9,10]
print(list2[0])
print(list2[2])
print(list2[3:9])
#Indices négatifs
print(list2[-1])
print(list2[-3])
print(list2[-1:-5])
```

```
3
5
[6, 7, 8, 9, 10]
10
8
[]
```

###### 3.2.2 Slices étendus

**syntaxe** : Object `[start:end:step]`



```
chaine = "Université"
print(chaine[0:9:1])
print(chaine[:4:]) # les quatre premiers élements
print(chaine[0:9:2])
#Indices négatifs
print(chaine[-2:-9:-1])
# Copie superficielle
print(chaine[::])
# Copie à l’envers
print(chaine[::-1])
```

```
Universit
Univ
Uiest
tisrevi
Université
étisrevinU
```

```
list2 = [3,4,5,6,7,8,9,10]
print(list2[3:9:2])
#Indices négatifs
print(list2[-1:-5:-2])
# Tous sauf les 4 premiers
print(list2[4::])
#Tous sauf les 4 derniers
print(list2[:-4:])

```

```
[6, 8, 10]
[10, 8]
[7, 8, 9, 10]
[3, 4, 5, 6]
```

```{admonition} Exercice
:class: warning 
Constituez une liste année contenant les 12 mois de l'année.
1. À partir de cette liste, comment récupérez-vous seulement les 3 premiers mois de l'année d’une part, et le reste d’autre part ? Utilisez pour cela l’indiçage.
2. Cherchez un autre moyen pour arriver au même résultat (en utilisant un autre indiçage).
3. Trouvez deux manières pour accéder au dernier mois de l'année.
4. Inversez les mois de l'année en une commande.
```

```
```