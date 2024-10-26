### Série 1 : Espace vectoriel

#### Prof. Jouilil Youness

###### 1. Sous-espace vectoriel

```{admonition} Exercice 1
**Montrer que les sous-ensembles suivants des sous-espaces vectoriels**

- $A_1$ =$ \left\{ (x,y,z) \in \mathbb{R}^3 / x+y+z = 0 \right\}$

- $A_2$ = $ \left\{ (x,y,z) \in \mathbb{R}^3 / x-y = 0 \right\}$

- $A_3$ = $ \left\{ (x,y,z) \in \mathbb{R}^3 / x =3z \right\}$

```

```{admonition} <font color='blue'>Réponse de l'exercice 1</font>
:class: attention, dropdown

- $A_1$ =$ \left\{ (x,y,z) \in \mathbb{R}^3 / x+y+z = 0 \right\}$

$(0,0,0) ~\in$ $A_1 ~~ \Rightarrow A_1 \neq  \emptyset$

Soit :  $X=(x,y,z) ~ et~ X'= (x',y',z') ~ \in ~A_1$

On a :

$X+ X' = (x,y,z) + (x',y',z') = (x+x',y+y',z+z')$

tel que : $x+y+z = 0 ~et~ x'+y'+z' = 0 \Rightarrow x+x'+y'+ y+ z +z' = 0 $

$X=(x,y,z) ~ et~ X'= (x',y',z') ~ \in ~A_1 \Rightarrow X+ X'~ \in ~A_1$

$\lambda X = (\lambda x, \lambda y,\lambda z)$

tel que : 
$\lambda x+ \lambda y+ \lambda z = 0 \Rightarrow \lambda (x+y+z) = 0$

Ainsi, $\lambda X \in ~A_1$
 
- $A_2$ = $ \left\{ (x,y,z) \in \mathbb{R}^3 / x-y = 0 \right\}$

- $A_3$ = $ \left\{ (x,y,z) \in \mathbb{R}^3 / x =3z \right\}$

```

```{admonition} Exercice 2
Les sous-ensembles suivants sont-ils des sous-espaces vectoriels ?

- $A_1$ =$ \left\{ (x,y,z) \in \mathbb{R}^3 / x+y-3z = 2 \right\}$

- $A_2$ =  $\left\{ (x,y,z) \in \mathbb{R}^3 / x+y > z \right\}$

- $A_3$ = $ \left\{ (x,y,z) \in \mathbb{R}^3 / xyz = 0 \right\}$

- $A_4$ = $ \left\{ (x,y,z, t) \in \mathbb{R}^4 / x = 2y= -z=3t \right\}$

- $A_5$ = $ \left\{ (x,y,z) \in \mathbb{R}^3 / y(x^2+z) = 0 \right\}$

```

```{admonition} <font color='blue'>Réponse de l'exercice 2</font>
:class: attention, dropdown
Pour  
- $A_1$ =$ \left\{ (x,y,z) \in \mathbb{R}^3 / x+y-3z = 2 \right\}$

- $A_2$ =  $\left\{ (x,y,z) \in \mathbb{R}^3 / x+y > z \right\}$

- $A_3$ = $ \left\{ (x,y,z) \in \mathbb{R}^3 / xyz = 0 \right\}$

- $A_4$ = $ \left\{ (x,y,z, t) \in \mathbb{R}^4 / x = 2y= -z=3t \right\}$

- $A_5$ = $ \left\{ (x,y,z) \in \mathbb{R}^3 / y(x^2+z) = 0 \right\}$

```

```{admonition} Exercice 3

* On considère l'ensemble suivant:

$$
A = \left\{ X \in \mathbb{R}^4 ; X= (x+2y,y-z, -x+3z,-z)~~ x,y,z \in \mathbb{R} \right\}
$$
1. Montrer que A est un sous espace vectoriel de $\mathbb{R}^4$
2. Donner une base de A
3. Le vecteur suivant (0,1,-4,0) appartient-il à A ? _Justifier votre réponse !_

```
```{admonition} <font color='blue'>Réponse de l'exercice 3</font>
:class: attention, dropdown
On a : 

$$
A = \left\{ X \in \mathbb{R}^4 ; X= (x+2y,y-z, -x+3z,-z)~~ x,y,z \in \mathbb{R} \right\}
$$

1. Montrons que A est un un sous espace vectoriel de $\mathbb{R}^4$
2. Cherchons une base de A.
3. Le vecteur (0,1,-4,0) appartient-il à A ?
```


###### 2. Combinaison linéaire

```{admonition} Exercice 3
On considère les vecteurs de $\mathbb{R}^3$ suivants :
$
E_1(1,0,1) ; E_2(0,1,1) ; E_3(1,1,0)
$

- Est-ce que le vecteur $E$$(2,3,0)$ est combinaison linéaire des vecteurs $E_1$, $E_2$ et $E_3$ ?
```



```{admonition} Exercice 3
On considère les ensembles suivants

$ 
E_1 = \left\{  A = \begin{pmatrix}
a& -b\\
b&c \\
\end{pmatrix} \in M(2) ~;~ 
a,b,c \in \mathbb{R} \right\}
$

$ 
E_2 = \left\{  A = \begin{pmatrix}
a& c\\
b& d\\
\end{pmatrix} \in M(2) ~;~
a,b,c, d \in \mathbb{R} \right\}
$

$ 
E_3 = \left\{  A = \begin{pmatrix}
a& a & c\\
b& d & a\\
b& d & a
\end{pmatrix} \in M(3) ~;~
a,b,c, d \in \mathbb{R} \right\}
$
$ 
E_5 = \left\{  A = \begin{pmatrix}
a& 0 & 0\\
b& 0 & -a\\
b& 0 & a
\end{pmatrix} \in M(3) ~;~
a,b \in \mathbb{R} \right\}
$

$ 
E_5 = \left\{  A \in M(2) ~;~
A' = -A \right\}
$

$ 
E_6 = \left\{  A \in M(3) ~;~
A' = A \right\}
$


tels que $M(2)$, $M(3)$ sont resp. les espaces vectoriels des matrices carrées d’ordre 2 et 3.

1. Parmi ces ensembles, quels sont ceux qui sont des sous-espaces vectoriels ?
2. Donner, _en justifiant vos réponses_, une famille génératrice pour chaque sous-espace vectoriel.

```

```{admonition} <font color='blue'>Réponse de l'exercice 3</font>
:class: attention, dropdown
On a : 


1. Parmi ces ensembles, quels sont ceux qui sont des sous-espaces vectoriels ?

A est-il un sous-espace vectoriel !?
```

###### 3. Famille libre
```{admonition} Exercice 4
Les familles de vecteurs suivantes sont-elles libres ?

1. $e_1(0,1,3)$, $e_2(-1,1,0)$ et $e_3(-2,0,5)$ dans $\mathbb{R}^3$.

2. $e_1(0,1,1)$, $e_2(1,1,0)$ et $e_3(1,1,1)$ dans $\mathbb{R}^3$.

3. $e_1(5,1,-1,0)$, $e_2(0,-1,3,7)$ et $e_3(8,1,-1,7)$ dans $\mathbb{R}^4$.
```
```{admonition} <font color='blue'>Réponse de l'exercice 4</font>
:class: attention, dropdown

Les familles de vecteurs suivantes sont-elles libres ?

```

###### 4. Famille génératrice
```{admonition} Exercice 5
- La famille de vecteurs $E = \left\{(1; 1; 0); (1;-1; 0); (1; 0; -1)\right\}$ est-elle une famille génératrice de $\mathbb{R}^3$ ? _Justifier_
```
```{admonition} <font color='blue'>Réponse de l'exercice 5</font>
:class: attention, dropdown

$E = \left\{(1; 1; 0); (1;-1; 0); (1; 0; -1)\right\}$ est-elle une famille génératrice de $\mathbb{R}^3$ ?

```

```
