#### Numpy pour les Tableaux et calcul matriciel

NumPy utilisée pour :

- Effectuer des calculs mathématiques et scientifiques

- calculs numériques autour des tableaux multidimensionnels

- Algèbre lnéaire

NumPy est la bibliothèque Python la plus utilisée en Data Science

##### Tableaux numpy.array()

NumPy introduit un nouveau type l'array qui est semblable à une liste, mais tous les éléments doivent être du même type (entier, flottant, booléen ou encore chaîne de caractères).

###### Tableaux unidimensionnels

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
####### le type

```python
type(tab)
```
```
<class 'numpy.ndarray'>
```
####### Accès aux éléments d’un tableau
```python
# Affichage de l'élément d'indice 2
print("Element d'incide 2 :", tab[2])
```

```
Element d'incide 2 : 2
```

```{admonition} Remarque
:class: warning 
Comme pour les listes, les indices des éléments commencent à zéro.
```

###### Tableaux multidimensionnels

Il est important de noter que pour un tableau multidimensionnel, on sépare chaque dimension par une virgule

```python
tab2 = np.array([[0, 1, 2], [3,4, 5]])
print(tab2)
```

```
[[0 1 2]
 [3 4 5]]
```

####### Accès aux éléments d’un tableau 2D
```python
# Affichage de la 1ère ligne
print(tab2[0])
# Affichage du premier élement
print(tab2[0,0])
```
###### Sélection de données

```{admonition} Remarque
:class: warning 
Sélection de données dans un tableau ou `slicing` permet de sélectionner une portion de données dans un tableau
```

La syntaxe est la suivante :

- `array[début:fin:pas]`

```python
tab2= np.array([0,1,2,3,4,5,6,7,8,9,10])
print(tab2)
# Une valeur sur deux en commençant à l'indice 0 jusqu'à l'indice 7 exclu
print(tab2[0:7:2])
# Une valeur sur trois en commençant à l'indice 1 jusqu'à la fin
print(tab2[1::3])
print(tab2[0::])
```
```
[ 0  1  2  3  4  5  6  7  8  9 10]
[0 2 4 6]
[ 1  4  7 10]
[0 3 6 9]
```

```python
print(tab2[1:7])  # Les valeurs comprises entre l'indice 1 et 7 exclue
print(tab2[:7])  # Les 7 premières valeurs
```
```
[1 2 3 4 5 6]
[0 1 2 3 4 5 6]
```

```python
print(tab2[-1])  # Affichage de la dernière valeur d'un tableau
```
```
10
```
###### Quelques fonctions usuelles
```python
print(np.shape(tab2)) # renvoie la taille du tableau.
print(np.arange(10)) #Équivalent à la fonction range.
print(np.arange(1,10,2))

```
Affichage
```
[0 1 2 3 4 5 6 7 8 9]
[1 3 5 7 9]
```

###### calcul matriciel avec NumPy

$$
  A = \left[ \begin{array}{ccc}
      1 & 2 & 3 \\
      0 & 5 & 6 \\
      7 & 8 & 9 \\
  \end{array} \right]
$$

- Matrice \( B \) :
 
$$
  B = \left[ \begin{array}{ccc}
      0 & 8 & 7 \\
      6 & 5 & 4 \\
      3 & 2 & 1 \\
  \end{array} \right]
$$


```python
A = np.array([[1, 2, 3],
              [0, 5, 6],
              [7, 8, 9]])

B = np.array([[0, 8, 7],
              [6, 5, 4],
              [3, 2, 1]])

print(A+B)
print(A-B)
#Multiplication de matrices (A * B):
print(A@B)
print(np.dot(A,B))
#Transposition d'une matrice (A transposée)
print(A.T)
#Inverse d'une matrice (si elle est inversible) :
print(np.linalg.inv(A))
# Determinant d'une matrice
print(np.linalg.det(A))
# Trace
print(np.trace(A))
# 
numpy.linalg.solve(A,b)

```
**Résolution du système Ax=b**

Supposons que nous ayons les matrices suivantes :

- Matrice \( A \) :
  
$$
  A = \left[ \begin{array}{ccc}
      1 & 2 & 3 \\
      0 & 5 & 6 \\
      7 & 8 & 9 \\
  \end{array} \right]
$$

- Le vecteur \( b \) :
 
$$
  b = \left[ \begin{array}{c}
      1 \\
      0 \\
      2 \\
  \end{array} \right]
$$

Nous cherchons à résoudre :

$$
 Ax=b \implies  \left[ \begin{array}{ccc}
      1 & 2 & 3 \\
      0 & 5 & 6 \\
      7 & 8 & 9 \\
  \end{array} \right] \left[ \begin{array}{c}
      x_1 \\
      x_2 \\
      x_3 \\
  \end{array} \right] = \left[ \begin{array}{c}
      1 \\
      0 \\
      2 \\
  \end{array} \right]
 $$


```python
b = np.array([1, 0, 2])
# Résoudre le système d'équations linéaires
x = np.linalg.solve(A, b)

# Afficher la solution
print("La solution du système Ax = b est :", x)
```

```{admonition} Exercice
:class: warning

Soit A et B deux matrices de $M_{2,2}(\mathbb{R})$ telles que :

$$
  A = \left[ \begin{array}{cc}
      1 & 2  \\
      0 & -5
  \end{array} \right]
$$

$$
  B = \left[ \begin{array}{cc}
      -1 & 1  \\
      2 & -3
  \end{array} \right]
$$

- Calculer $A+B$, $A-B$

- Calculer $2B$, $-A$, $A+3I_2$, $B-2I_2$

- Calculer $AB$ et $BA$

- Comparer les deux matrices  $(A+B)^2$ et $A^2+2AB+B^2$.

- comparer les deux matrices $(A+B)^2$ et $A^2+AB+BA+B^2$.


```

```{admonition} Exercice
:class: warning

On considère, dans  $M_{2,2}(\mathbb{R})$,  les matrices suivantes : 

$$
  A = \left[ \begin{array}{cc}
      1 & -1  \\
      -1 & 1
  \end{array} \right]
$$

$$
  B = \left[ \begin{array}{cc}
      1 & 1  \\
      0 & 2
  \end{array} \right]
$$

- Calculer $A^2$, $A^3$ et $A^4$ 

- En déduire la valeur de $A^n$  $~~,~~ \forall ~~n ~~ \geq ~~1$.

-  Répondre aux mêmes questions pour la matrice B.

```