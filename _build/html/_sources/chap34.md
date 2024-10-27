#### Exercices d’application


##### Exercice 01

```{admonition} Exercice
:class: warning
Écrire une fonction en Python appelée calculer_factorielle qui prend un nombre entier positif en paramètre et renvoie sa factorielle. La factorielle d'un nombre n est le produit de tous les entiers de 1 à n.

Ensuite, écrivez un programme principal qui demande à l'utilisateur d'entrer un nombre entier, appelle la fonction calculer_factorielle pour calculer sa factorielle, puis affiche le résultat.
```

##### Exercice 02

```{admonition} Exercice
:class: warning
Écrivez une fonction Python appelée somme_carres_pairs qui prend en entrée un entier n et retourne la somme des carrés des nombres pairs de 1 à n.

```
##### Exercice 03

```{admonition} Exercice
:class: warning 
On considère la matrice $M_{(3,3)}(\mathbb{R})$ définie par :

$$
A =
\left[ \begin{array}{ccc}
1 & 2 & 3 \\
-1 & 0 & -1 \\
9 & -7 & 3 \\
\end{array} \right]
$$

a. Définir la matrice \( A \) comme un tableau NumPy à l'aide de la fonction `np.array()`.

b. Modifier la matrice \( A \) pour que ses deux premières lignes soient multipliées par 1/2 et que sa dernière colonne soit divisée par 5.

```

##### Exercice 04

```{admonition} Exercice
:class: warning 
On donne :

$$
A =
\left[ \begin{array}{ccc}
1 & 2 & 3 \\
-1 & 0 & -1 \\
9 & -7 & 3 \\
\end{array} \right]
$$
$$
B =
\left[ \begin{array}{ccc}
2 & 2 & 4 \\
0 & 0 & -1 \\
1 & 2 & 0 \\
\end{array} \right]
$$
$$
C =
\left[ \begin{array}{ccc}
-5 & 2 & 7 \\
-7 & 2 & -1 \\
1 & 3 & 0 \\
\end{array} \right]

$$

a. Calculer A+B, B+C, A+2B, B-4C

b. Modifier la matrice \( A \) pour que ses deux premières lignes soient multipliées par 1/2 et que sa dernière colonne soit divisée par 5.

c. Ecrire la matrice transposée $A^{'}$ de A et donner son format 

d. Calculer, puis comparer les produits AB et BA. Commenter

e. Calculer, puis comparer les produits A(BC) et A(BC). Commenter


```

##### Exercice 05

```{admonition} Exercice
:class: warning 
Soit \( A \) une matrice carrée de dimensions $M_{(3,3)(\mathbb{R})}$, définie comme suit :

$$
A =
\left[ \begin{array}{ccc}
2 & -2 & 2/3 \\
-2 & 4 & 1 \\
0 & -1 & 1 \\
\end{array} \right]
$$

- Déterminez le rang de la matrice \( A \) en utilisant la fonction `np.linalg.matrix_rank` de NumPy. Indiquez également si la matrice est inversible.

- En utilisant la matrice \( A \) et le vecteur \( b \) défini comme suit :

$$
b = 
\left[ \begin{array}{c}
3 \\
-7 \\
1 \\
\end{array} \right]
$$
résolvez le système d'équations linéaires \( Ax = b \) en utilisant la fonction `np.linalg.solve()`. 

```

##### Exercice 06

```{admonition} Exercice
:class: warning 

Résoudre les systèmes d'équations linéaire suivants :

a. Système de 2 inconnues :

$$
\begin{cases}
2x + 3y &= 5 \\
x - y &= 3 \\
\end{cases}

$$

b. Système de 3 inconnues :

$$
\begin{cases}
3x - 2y + z &= 6 \\
2x + 4y - 3z &= 10 \\
x - y + 2z &= 4 \\
\end{cases}

$$

c. Système de 4 inconnues :

$$
\begin{cases}
x + 2y - z + 3w &= 7 \\
2x - y + 3z - 2w &= 5 \\
3x + y - 2z + w &= 3 \\
x - 3y + z + 2w &= -1 \\
\end{cases}

$$

d. Système de 5 inconnues :

$$
\begin{cases}
2x + y - z + 3w - 2v &= 7 \\
x - 2y + z - w + 4v &= 5 \\
3x + y + z - w - v &= 3 \\
x - y + 2z + w + v &= 2 \\
2x + 3y - z - 2w + v &= -4 \\
\end{cases}

$$

