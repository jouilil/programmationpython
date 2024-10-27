# Les Boucles

Supposons que vous souhaitiez afficher les éléments d’une liste les uns après les autres. Dans l’état actuel de
vos connaissances, il faudrait taper quelque chose du style :

```
Nom = [" Hamid " , " Said", " Karima ", " Aya ", "Aboubakar"]
print ( Nom[0])
print ( Nom[1])
print ( Nom[2])
print ( Nom[3])
print ( Nom[4])
```
```
Hamid
Said
Karima
Aya
Aboubakar
```
Si notre liste contient plus ce que 100000 éléments! Pour remédier à ce défi, il faut utiliser les boucles
```
Nom = [" Hamid " , " Said", " Karima ", " Aya ", "Aboubakar"]
for nom in Nom :
     print ( nom )
```

```
Hamid
Said
Karima
Aya
Aboubakar
```

Lorsqu’on voulait répéter plusieurs fois l’exécution d’une partie du programme, on utilise les boucles. Il en existe deux types :

-  Les boucles bornées 

-  Les boucles non bornées

###### 2.1. Les boucles bornées
Elles sont utilisées lorsqu’on a une idée a priori sur le nombre de répétition. Il s’agit de la boucle `for` ; la syntaxe de la boucle `for` est la suivante :

```
for var in valeurs_possibles:
    instructions
```

* `var` est le nom d'une variable locale à la fonction `for()` 
* `valeurs_possibles` un objet comprenant des éléments définissant les valeurs que prendra objet pour chaque itération, 
*  `instructions` est le bloc d'instructions qui seront exécutées à chaque itération.

Voici deux exemples simples de l’utilisation de la boucle `for` :

- Calculer le carrée de chaque nombre 1, 2, 3 et 4;

- Calculer la somme des nombres 1, 2, 3 et 4.

```
for i in [1, 2, 3, 4]:
    print("le carré de", i, "est:", i**2)
```


Affichage après exécution :

```
le carré de 1 est: 1
le carré de 2 est: 4
le carré de 3 est: 9
le carré de 4 est: 16
```
```
somme = 0
for i in [1, 2, 3, 4]:
    somme += i
print(somme)
```

```
10
```

Une fonction très importante qui est souvent utilisée en Python pour la boucle for est la fonction `range()`. Cette fonction prend les arguments suivants :

- start : (optionnel, par défaut, 0) valeur de début pour la séquence (inclue) ;

- stop : valeur de fin de la séquence (non inclue) ;

- step : (optionnel, par défaut 1) le pas.

On peut refaire les exemples suivants comme suit :

```
for i in range(1, 5):
    print("le carré de", i, "est:", i**2)
```

```
le carré de 1 est: 1
le carré de 2 est: 4
le carré de 3 est: 9
le carré de 4 est: 16
```

```
somme = 0
for i in range(5):
    somme += i
print(somme)
```
Affichage après exécution :
```
10
```
Rien n’empêche avoir une boucle for dans un bloc d’instructions d’une autre boucle `for`. Ou encore une instruction conditionnelle dans un bloc de la boucle `for` (vice versa). Par exemple si on veut calculer le produit de chaque élément de la liste `[1, 5, 9, 10]` par chaque élément de la liste `[2, 3, 5]`:

```
for i in [1, 5, 9, 10]:
    for j in [2, 3, 5]:
        print("Le produit de", i, "fois", j, "est:", i*j)
```

Affichage après exécution :

```
Le produit de 1 fois 2 est: 2
Le produit de 1 fois 3 est: 3
Le produit de 1 fois 5 est: 5
Le produit de 5 fois 2 est: 10
Le produit de 5 fois 3 est: 15
Le produit de 5 fois 5 est: 25
Le produit de 9 fois 2 est: 18
Le produit de 9 fois 3 est: 27
Le produit de 9 fois 5 est: 45
Le produit de 10 fois 2 est: 20
Le produit de 10 fois 3 est: 30
Le produit de 10 fois 5 est: 50

```
Ou si l’on veut tester la parité de chaque élément entre 3, et 14 (`range(3,15)`);


```
for i in range(3, 15):
    if i%2==0:
        print("Le nombre", i, "est pair")
    else:
        print("Le nombre", i, "est impair")
```

Affichage après exécution :

```
Le nombre 3 est impair
Le nombre 4 est pair
Le nombre 5 est impair
Le nombre 6 est pair
Le nombre 7 est impair
Le nombre 8 est pair
Le nombre 9 est impair
Le nombre 10 est pair
Le nombre 11 est impair
Le nombre 12 est pair
Le nombre 13 est impair
Le nombre 14 est pair
```


```{admonition} Exercice
:class: warning
Demandez à l'utilisateur de saisir un nombre, puis utilisez une boucle for pour afficher la table de multiplication de ce nombre de 1 à 10.
```

```{admonition} Exercice
:class: warning
Demandez à l'utilisateur de saisir un nombre, puis utilisez une boucle for pour calculer la somme des carrés des nombres de 1 à ce nombre.
```
```{admonition} Exercice
:class: warning 
Codez un programme qui donne la factorielle d’un nombre.

Pour rappel, la factorielle est le réssultat de la multiplication de tous les nombres inférieurs ou égaux à un nombre donné.
```

```{admonition} Exercice
:class: warning 
Écrire un algorithme permettant d'afficher les nombres paires compris entre 0 et N, où N saisi par l'utilisateur.
```

###### 2.2. Les boucles non bornées

Elles sont utilisées si on ne connait pas à l’avance le nombre de répétitions. Il s’agit de la boucle `while`. Le principe d’une boucle `while()` est que les instructions à l’intérieur de la boucle seront répétées tant qu’une condition est respectée. L’idée est de faire dépendre cette condition d’un ou plusieurs objets qui seront modifiés au cours des itérations (sans cela, la boucle tournerait à l’infini).

La syntaxe est la suivante 

```
while condition:
    instructions
```
Nous allons illustrer le rôle de chaque boucle dans l’exemple suivant. Supposons que nous voulons calculer le factoriel d’un nombre (soit 10), voici le code pour le calculer :

```
i = 1
fact = 1
while i<=10:
    fact *= i
    i+=1

print(fact)
```

Affichage après exécution :

```    
3628800
```

Reprenons l’exemple précédant dont on veut tester la parité de chaque élément entre 3, et 14 avec la boucle while:

```
i = 3
while i<15:
    if i%2==0:
        print("Le nombre", i, "est pair")
    else:
        print("Le nombre", i, "est impair")
    i+=1
```

Affichage après exécution :

```
Le nombre 3 est impair
Le nombre 4 est pair
Le nombre 5 est impair
Le nombre 6 est pair
Le nombre 7 est impair
Le nombre 8 est pair
Le nombre 9 est impair
Le nombre 10 est pair
Le nombre 11 est impair
Le nombre 12 est pair
Le nombre 13 est impair
Le nombre 14 est pair

```

```{admonition} Remarque
:class: tip

- Si on connaît avant de démarrer la boucle le nombre d’itérations à exécuter, on choisit une boucle for. Au contraire, si la décision d’arrêter la boucle ne peut se faire que par un test, on choisit une boucle while.

- Il est toujours possible de remplacer une boucle for par une boucle while.


```