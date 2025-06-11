#### Caractéristiques de Tendance Centrale


Les représentations graphiques ont permis une première synthèse visuelle de la distribution des observations.

Un paramètre statistique permet de résumer par une seule quantité numérique une information contenue dans une distribution d’observations.!

```{admonition} Avertissement

Les paramètres statistiques ne concernent que les variables quantitatives

```

##### Le mode (m)


```{admonition} Définition

Le mode d'une distribution statistique est la valeur du caractère la plus fréquentée

On note généralement le mode d'une série donnée par m .

Une distribution est unimodale si elle présente un maximum marqué, et pas d'autres maxima relatifs.

La lecture s'effectue sur le diagramme en bâtons ou l'histogramme.

Le mode correspond à l'abscisse du maximum, c.à.d. la valeur la plus fréquente

```

```{admonition} Le mode (m)

1. *Cas d'une var. quant. Discrète*

$ f_{i}(x_{i}) $ $\leq$ $ f_{i_{0}}(x_{i_{0}}) $ ; $\forall$ i ={1, 2, ..., N} $\Rightarrow$ m = $x_{i_{0}}$


On parle dans ce cas de la valeur modale.

2. *Cas d'une var. quant. cont.*


$ f^c_{i}(x_{i}) $ $\leq$ $ f^c_{i_{0}}(x_{i_{0}}) $ ; $\forall$  i ={1, 2, ..., N} $\Rightarrow$ m $\in$ $[x_{i_{0}-1}, x_{i_{0}}[$


On parle dans ce cas de classe modale.

La valeur exacte du mode peut être retrouvée graphiquement à l'aide de l'histogramme ou un développement mathématiquement (Voir TD)



- Si la distribution présente 2 ou plus maxima relatifs, on dit qu'elle est bimodale ou plurimodale.

- La population est composée de plusieurs sous-populations ayant des caractéristiques de tendance centrale différentes.


<center>

![Drag Racing](image_2.JPG)

</center>


```

#####  Les différentes types de moyennes

###### La moyenne arithmétique simple ($\overline{x}$)


```{admonition} La moyenne arithmétique simple $\overline{x}$

La moyenne arithmétique simple est une caractéristique de tendance centrale qui est proche (au centre) de toutes les observations

On note la moyenne arithmétique simple d'une série statistique par le symbole $\overline{x}$

Pour calculer une moyenne, on effectue le calcul suivant :

**Série brute**: $\overline{x} = \frac{1}{N} \sum^{N}_{i=1} x_{i}$

```

```{admonition} La moyenne arithmétique simple $\overline{x}$

*Série groupée (var. quant. discrète):*

$$
\overline{x} = \frac{1}{N} \sum^{k}_{i=1} n_{i}x_{i}= \sum^{k}_{i=1} f_{i}x_{i} 
$$

*Série groupée (var. quant. continue)*

$$
\overline{x} = \frac{1}{N} \sum^{k}_{i=1} n_{i}c_{i}= \sum^{k}_{i=1} f_{i}c_{i} 
$$

ou $c_{i}$ est le centre de la classe [$x_{i-1}$,$x_{i}$[
```

```{admonition} Les différentes types de moyennes

- *Moyenne géométrique (G)*

Utilisée dans le cas de phénomènes multiplicatifs

$$
G = \sqrt[N]{\prod^{N}_{i=1} x_{i}}
$$

La moyenne géométrique s'utilise, par exemple, quand on veut calculer la moyenne de taux d’intérêt, taux de croissance moyen ...etc.


- *Moyenne harmonique (H)*

Utilisée dans le cas où l’on combine deux variables sous forme de rapport (pièces/heure, km/litre,…)

$$
H = \frac{N}{\sum^{N}_{i=1} \frac{1}{x_{i}}}
$$


- *Moyenne quadratique (Q)*

Une moyenne qui trouve des applications lorsque l'on a affaire à des phénomène présentant un caractère sinusoïdal avec alternance de valeurs positives et de valeurs négatives (très utilisée en physique, électricité, ...etc).

$$
Q = \sqrt{\sum^{N}_{i=1} x^{2}_{i}}
$$


```


##### La médiane M

```{admonition} La médiane M
La médiane d'une série statistique notée généralement par M est la valeur du caractère qui répartie la population en deux sous-parties égales.


- Var. quant. discrète

Médiane pour le cas d'une var. quant. discrète.

a. Observations non groupées
 
$$
M = \left\{ 
\begin{array}{l l}
  X(\frac{N}{2}) & ~~~~ N ~~ pair
\\
  X(\frac{N+1}{2}) & \quad N ~~ impair\\  
  \end{array} \right.
$$

b. Observations groupées


$F_{i-1}(x_{i_{0}-1})$ $\leq$ 0.5 $<$ $F_{i}(x_{i_{0}})$ $\Rightarrow$ M = $x_{i_{0}}$


- Var. quant. continue


$F_{i-1}$ $\leq$ 0.5 $<$ $F_{i}(x_{i_{0}})$ $\Rightarrow$ M $\in$ $ [x_{i_{0}-1}, x_{i_{0}}[$

On parle dans ce cas de *la classe médiane* $ [x_{i_{0}-1}, x_{i_{0}}[$.

La valeur exacte peut être retrouvée graphiquement à l'aide de l'histogramme ou mathématiquement par interpolation linéaire ou encore par l'intersection des courbes des fréquences cumulées croissantes (F) et celles des fréquences cumulées décroissantes (G) (Pour plus de détails, voir TD).

```

```{admonition} Exercice 4: CTC

Les notes d’une classe à un contrôle en économie contemporaine a donné lieu à la  répartition suivante :

<center>

![Drag Racing](exo_4.JPG)

</center>

a) Calculer la moyenne arithmétique simple. Commenter

b) Calculer le mode. Commenter

c) Calculer la médiane. Commenter.
```




##### Exercices d'applications

##### Exercice 01

```{admonition} Exercice
:class: warning 
Vous avez les données suivantes concernant les notes d’un groupe d’étudiants :

- Notes : 3, 8, 12, 15, 17, 19, 20

- Effectifs : 6, 4, 6, 10, 8, 2, 1

1. Identifier la variable étudiée et son type.

2. Récapituler ces données dans un tableau statistique

3. Calculez manuellement et sous python les fréquences et les fréquences cumulées croissantes

4. Calculer  manuellement et sous python la moyenne arithmétique simple $\overline{x}$

5. Calculer manuellement et sous python le mode.

6. Calculer manuellement et sous python la médiane.

```


##### Exercice 02

```{admonition} Exercice
:class: warning 
Vous disposez des données suivantes concernant les températures maximales mensuelles dans une ville :

- Températures (°C) : 18, 22, 25, 27, 30

- Effectifs (mois correspondants) : 3, 4, 5, 2, 3

1. Calculez les fréquences des différentes températures.

2. Calculez manuellement et sous python les fréquences cumulées croissantes

3. Calculer  manuellement et sous python la moyenne arithmétique simple $\overline{x}$

4. Calculer manuellement et sous python le mode.

5. Calculer manuellement et sous python la médiane.

```

##### Exercice 03
```{admonition} Exercice
:class: warning 
Vous avez les données suivantes concernant les tailles des individus dans une population :

- Tailles (en cm) : 150-160, 160-170, 170-180, 180-190, 190-200

- Effectifs (individus dans chaque tranche de taille) : 12, 25, 30, 15, 8

1. Calculez les fréquences des différentes tranches de tailles.

2. Calculez manuellement et sous python les fréquences cumulées croissantes

3. Calculer les valeurs centrales des tranches de tailles.

4. Calculer  manuellement et sous python la moyenne arithmétique simple $\overline{x}$

5. Calculer manuellement et sous python le mode.

6. Calculer manuellement et sous python la médiane.

7. Représentez la courbe des fréquences cumulées croissantes pour illustrer la répartition cumulative des individus par taille.
```
##### Exercice 04
```{admonition} Exercice
:class: warning 
Les données suivantes concernent la durée des trajets domicile-travail (en minutes) d'une population d'employés :

- Durée des trajets (en minutes) : 0-10, 10-20, 20-30, 30-40, 40-50

- Effectifs (employés correspondant à chaque intervalle de temps) : 20, 50, 40, 25, 10

1. Calculez les fréquences pour chaque intervalle de durée de trajet.

2. Créez la représentation graphique adéquate pour afficher la répartition des employés en fonction de la durée des trajets.

3. Calculez les caractéristiques de tendence centrales

4. Représentez la courbe des fréquences cumulées croissantes pour illustrer la répartition cumulative des individus par durée de trajet.
```