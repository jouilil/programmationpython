# Variables et opérations

##### 1.  Variable
###### 1.1. Variable et assignation
Une variable est concept fondamental en programmation. Elle permet de stocker une valeur (par exemple la valeur 2) ou un objet (par exemple une fonction, liste, tableau, vecteur, …). Cela permet de l’utiliser ultérieurement pour accéder facilement à la valeur ou à l’objet qui est stocké dans cette variable.

On affecte une valeur a une variable en utilisant le symbole `=`. Si vous voulez stocker la valeur 4 dans une variable nommée `ma_valeur` on peut faire comme suit :



```python
# affecter la valeur 4 a la variable ma_valeur
ma_valeur = 4
# afficher le contenu de la variable ma_valeur
print(ma_valeur)

```

Affichage après exécution :

```
4
```

On peut faire toutes les opérations susmentionnées avec les variables à la place de valeurs. Voici un exemple : Dans une classe, le nombre des hommes est 10 le nombre des femmes est 18.

```
# Affecter le nombre des étudiants de sexe masculin à la variable hommes
hommes = 10
# Affecter le nombre des étudiants de sexe féminin à la variable femmes
femmes = 18

# Affecter le nombre total des étudiants à la variable total_etudiant
total_etudiant = hommes + femmes

# Afficher le nombre total d'étudiants
print(total_etudiant)
```

Affichage après exécution :

```python
28
```

Python supporte les opérateurs d’affectation suivants : `=`, `+ =`, `– =`, `*=`, `/=`, `%=`, `**=` et `//=`

Hormis le premier opérateur `=`, les autres opérateurs ont la même logique. Nous allons illustrer cette logique avec `+=` et vous alles comprendre l’utilisation des autres.


Imaginons une variable (appelons-la `var`) contenant une valeur (par exemple, `2`). Pour une raison particulière, nous souhaitons que cette variable conserve son ancienne valeur (2) tout en ajoutant une nouvelle valeur (par exemple, `1`). Cela peut être réalisé en utilisant l'opérateur `=` de la manière suivante :

```
# la variable var contient la valeur 2
var = 2
# la variable var reçoit l'ancienne valeur plus 1
var = var +1
# afficher le contenu de la variable var
print(var)
```

Affichage après exécution :

```
3
```
On peut faire la même instruction avec l’opérateur `+=` comme suit :

```
# la variable var contient la valeur 2
var = 2
# la variable var reçoit l'ancienne valeur plus 1
var += 1
# afficher le contenu de la variable var
print(var)
```

Affichage après exécution :
```
3
```

```{admonition} Avertissement
:class: attention
Sous Python, les noms de variables doivent en outre obéir à quelques règles simples :

- Un nom de variable est une séquence de lettres (`a → z`, `A → Z`) et de chiffres (`0 → 9`), qui doit toujours commencer par une lettre.

- Seules les lettres ordinaires sont autorisées. Les lettres accentuées, les cédilles, les espaces, les caractères spéciaux tels que `$`, `#`, `@`, etc. sont interdits, à l’exception du caractère `_` (souligné).

- Python est `case sensitive` (les caractères majuscules et minuscules sont distingués). Par exemple : Var1, var1, VAR1 sont donc des variables différentes.

- il est interdit d’utiliser comme nom de variables les mots réservés a python. Ils sont : `and`, `as`, `assert`, `break`, `class`, `continue`, `def`, `del`, `elif`, `else`, `except`, `False`, `finally`, `for`, `from`, `global`, `if`, `import`, `in`, `is`, `lambda`, `None`, `nonlocal`, `not`, `or`, `return`, `True`, `try`, `while`, `with`

```




###### 1.2.   Types de variables
Il existe de nombreux types de données dans Python. Voici quelques-uns les plus basiques :

- `float`: Les valeurs décimales (ou en virgule flottante) telles que 10,15 (attention en utilise `.` comme décimal au lieu de `,`).

- `int` (les nombres entiers) : les valeurs comme 8; 4; 10 sont des entiers (`int`). Les entiers font aussi partie des valeurs numériques.

- `bool` (les valeurs booléennes) : `True` ou `False` sont dites valeurs logiques.

- `str` (les caractères, ou chaînes de caractères). Les guillemets "texte" (ou encore les apostrophes 'texte') indiquent que texte est de type `str`.

- `complex` (les nombre complexes): sont les nombres contenant une partie réelle et une partie imaginaire. En mathématiques, on note  le nombre complexe dans le carrée est égale à 1. Cependant, en Python, on utilise la lettre `j` (ou `J`) pour indiquer ce nombre. Par exemple, si on voulait écrire le nombre 3+1.5`i` (le nombre complexe dont la partie réelle est 3 et la partie imaginaire est 1.5) en python on écrit 3 + 1.5`j`.

- `None`: type Le mot-clé None est utilisé pour définir une valeur nulle (pas 0), ou aucune valeur du tout. None n’est pas la même chose que 0, `False` ou une chaîne vide ''. None est un type de données en soi (NoneType) et la seule valeur qui peut être de type `None` est le mot-clé None.

si nous avons un variable (ou même une valeur) et nous voulons savoir son type de données, on utilise la fonction type. Il faut être prudent lorsqu’on voulait faire des opérations sur des variables si leur type n’est le même!


```
# cette instruction va afficher int
print(type(1))
# cette instruction va afficher float
print(type(1.5))

# cette instruction va afficher  bool
print(type(True))
# cette instruction va afficher str
print(type("bonjour"))

# cette instruction va afficher complex
print(type(5+17.89j))

# cette instruction va afficher NoneType
print(type(None))

```
Affichage après exécution :

```
<class 'int'>
<class 'float'>
<class 'bool'>
<class 'str'>
<class 'complex'>
<class 'NoneType'>
```

###### 1.3. Minimum et maximum
Python propose les fonctions min() et max() qui renvoient respectivement le minimum et le maximum de plusieurs entiers
et /ou floats :

```
a = 6
b = 7
c= -5
d =min(a,b,c)
print(d)
```
```
a = 6
pi = 3.14
c =max(pi,a)
print(c)
```

###### 1.4. Convertir les types de données
    
Il existe plusieurs raisons pour lesquelles nous somme devant l’obligation de convertir les types de données (une raison est celle de `input` que nous avons vu). Les fonctions qui servent à la conversion entre les types de données sont les suivantes :

- `int()`: pour convertir un type de données en entier;

- `float()`: pour convertir un type de données en virgule flottante.

- `str()`: pour convertir un types de donnes en chaine de caractères;

- et `bool()`: pour convertir les types de donnes en valeurs booléennes.

Les types de données `int` et `float` peuvent être convertis en tous autre type de données. La seule remarque est que la conversion d’une valeur de type `float` en `int` rend les chiffres avant la virgule (1.9 devient 1 après conversion). Pour avoir l’entier le plus proche au nombre que nous voulons convertir, nous devons utiliser la fonction `round()`.

#### 2.   Opérateurs logiques et relationnels 

##### 2.1.   Opérateurs logiques

En python, il existe trois opérateurs logiques : `or` qui signifie ou, `and` qui signifie et, et `not` qui signifie non.

Pour mieux illustrer ces opérations, soient `var1= True` et `var2 = False`. Quel serait le résultat des instructions suivantes :

- `var1 or var2`

- `var1 and var2`

- `not var1`

- `(var1 and var2) or (not var2)`

```python
# initialiser les deux variables
var1 = True; var2 = False # remarquer qu'on peut faire plusieurs instructions dans une même linge. Cependant, il est déconseillé
#
print(var1 or var2)

#
print(var1 and var2)

#
print(not var1)

# 
print((var1 and var2) or (not var2))
```
Affichage après exécution :
```
True
False
False
True
```

##### 2.2.   Opérateurs relationnels (tests)


En python, il existe six opérateurs relationnels :

- `<` qui permet de tester si une valeur et strictement inférieure à une autre ;

- `<=` qui permet de tester si une valeur et inférieure ou égale à une autre ;

- `>` qui permet de tester si une valeur et strictement supérieure à une autre ;

- `>=` qui permet de tester si une valeur et supérieure ou égale à une autre ;

- `!=` ou `<>` qui permet de tester si une valeur est égale a une autre;

- et `==` qui permet de tester l’égalité de deux valeurs.

Soient `var1 = 5`, `var2 = 2+3`, `var3 = 6`, `var4 = "bonjour"`, `var5 = True`. Quel serait le résultat des instructions suivantes :

- `var1 == var2`;

- `var2 != var4`;

- `var3 > var1+ var2`;

- `var3< var1 + var2`;

```python
#
var1 = 5; var2 = 2+3; var3 = 6; var4 = "bonjour"; var5 = True

#
print(var1 == var2)

#
print(var1 != var4)

#
print(var3 > var1 + var2)

#
print(var3 < var1 + var2)
```
Affichage après exécution :

```
True
True
False
True
```

#### 3. Lecture d’informations au clavier
Parfois, on est amené a ce que notre programme dépend d’intervention de l’utilisateur (entrée d’un paramètre, clic de souris sur un bouton, etc.). Dans un programme simple, on utilise la fonction `input`. Cette fonction invite l’utilisateur à entrer des données au clavier puis taper `<entrer>`. Lorsque le programme est exécuté, une case apparait à l’utilisateur pour entrer ces donner. Puis le programme continue à s’exécuter pour rendre un output. Les données entrées par l’utilisateur peuvent être stockées dans une variable. Il est à noter que cette variable sera de type `str`. Donc, si l’on veut des données numériques par exemple, on doit convertir cette variable au type de donne que nous souhaitons. Enfin, on peut y mettre comme argument un texte qui oriente à l’utilisateur lors de l’entrée des données. Voici un exemple dont on demande à l’utilisateur d’entrer son nom.

```python
x = input()
print(x)
```
Le type de la variable qui stocke le contenu de `input` est toujours `str`:

```python
x = input("merci d'entrer un chiffre: ")
print(type(x))
```

```python
<class 'str'>
```

```{admonition} Exercice
:class: warning
Veuillez créer un script qui demande deux valeurs entières à l'utilisateur et calculer la somme de ces deux valeurs.
```

```
x = 5
y = 10
z = 8

y -= 3
z += 1

resultat = x * (y + z)

print(f"Le résultat est : {resultat}")
```



```
a = 7
b = 3
c = 5

a += 2
b -= 1
c *= 3
a, b = b, a

resultat = a + (b * c)

print(f"Le résultat est : {resultat}")
```


```{admonition} Remarque
:class: tips
L'expression `a, b = b, a` en Python est une manière élégante d'échanger les valeurs de deux variables sans avoir besoin d'une variable auxiliaire.
```


```python
x = 10
y = 5
z = 2

x, y, z = z, x, y
x += 3
y *= 2
z -= 1
x, y = y, x

res = x / (y - z)

print(f"Le résultat est : {res}")
```

#### 4. Retour sur les éléments de base de l'algorithmique
##### 4.1. Notions d’algorithmique

```{admonition} Définition
:class: notice

Un algorithme est une suite  d'instructions qui décrivent la solution d'un problème informatique posé. Il s'agit du plan ou la structure d'un programme informatique. 

```

Un algorithme se trouve détaché de tout langage de programmation, tout en étant intimement lié à celui-ci, puisqu'il définit la logique qui sous-tend sa mise en œuvre.

##### 4.2. Structure d’un algorithme
Un algorithme doit être lisible et compréhensible par plusieurs personnes.

**Algorithme** : Nom d’Algorithme

**Déclarations : Variables, constantes…**

**Début**

$~~~~~$ Ensemble d’instructions ;

**Fin**

##### 4.3. Exemples

```{admonition} Exemple 1
:class: tip
Écrire un algorithme qui demande à l'utilisateur de saisir un nombre entier, puis qui calcule et affiche le carré de ce nombre.
```



**Algorithme Calculecarree**

**Variables** Nombre, carree: entiers

**Début**

$~~~~~$ Ecrire('Quel nombre voulez-vous élever au carré?')
    
$~~~~~$ Lire(Nombre)
    
$~~~~~$ carree ←Nombre*Nombre
    
$~~~~~$ Ecrire('Le carrée de', Nombre,'c'est ', carree)

**Fin**



```{admonition} Exemple 2
:class: tip
Écrire un algorithme qui demande à l'utilisateur de saisir un nombre entier, puis qui calcule et affiche l'inverse de ce nombre.
```