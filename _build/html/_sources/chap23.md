# Listes en compréhension

##### Définition

```{admonition} Définition \& utilité
:class: tips
Les listes en compréhension offrent une méthode concise pour créer des listes. Elles permettent notamment de générer une liste où chaque élément est le résultat d'une opération appliquée à chaque élément d'une séquence existante. Elles sont également utiles pour filtrer une séquence en ne conservant que les éléments répondant à une condition spécifique
```

Les avantages des listes en compréhension :

- Concision : Les listes en compréhension permettent d'écrire du code de manière plus concise par rapport à l'utilisation de boucles classiques.

- Lisibilité : Les listes en compréhension rendent souvent le code plus lisible et plus compréhensible.

- Performance : Les listes en compréhension sont plus performantes que l'utilisation de boucles for traditionnelles.

##### Syntaxe générale 

La syntaxe générale d'une liste en compréhension est la suivante :

```
[expr for val in collection]
[expr for val in collection if <test>]
[expr for val in collection if <test1> and <test2>]
[expr for val in collection if <test1> or <test2>]
[expr for val1 in collection1 and val2 in collection2]

```
##### Exemples

###### Exemple 1
```
nums=[6,7,9,10,12,17,18,19,20,24,35,44,65,88, 99,102,112]
# Méthode classique
even_num=[]
for num in nums :
    if num%2==0 :
        even_num.append(num)

print(even_num)

# listes en compréhension 
even_num2=[num for num in nums if num%2==0]
print(even_num2)

```
###### Exemple 2
```
# Méthode classique
squares=[]
for i in range(50):
    squares.append(i**2)
print(squares)
```
```
[0, 1, 4, 9, 16, 25, 36, 49, 64, 81, 100, 121, 144, 169, 196, 225, 256, 289, 324, 361, 400, 441, 484, 529, 576, 625, 676, 729, 784, 841, 900, 961, 1024, 1089, 1156, 1225, 1296, 1369, 1444, 1521, 1600, 1681, 1764, 1849, 1936, 2025, 2116, 2209, 2304, 2401]
```
```
# listes en compréhension 
squares=[num*num for num in range(50)]
print(squares)
```

```{admonition} Exercice
:class: warning
Écrivez un programme Python qui prend un nombre entier positif en entrée et renvoie une liste contenant tous ses diviseurs.
```

```
# Méthode classique
def diviseurs(n):
    my_list=[]
    for i in range(1,n+1):
        if n%i==0:
            my_list.append(i)
    return my_list

# Méthode des listes en compréhension 
def diviseurs2(n):
    my_list2=[divis for divis in range(1,n+1) if n%divis==0]
    return my_list2

print(diviseurs(42))
print(diviseurs2(42))
```

```{admonition} Exercice
:class: warning
Écrivez un programme Python qui prend deux ensembles en entrée et renvoie une liste de tuples représentant le produit cartésien de ces deux ensembles. Par exemple, si l'entrée est {a, b} et {3, 4}, le programme devrait renvoyer [(a, 3), (a, 4), (b, 3), (b, 4)].
```

