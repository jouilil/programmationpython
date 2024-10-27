# Tuples en Python

##### 1.  Définition

On définit tuples avec des parenthèses.

Un tuple est une liste qui ne peut plus être modifiée. Autrement dit, les tuples ressemblent aux listes, mais on ne peut pas les modifier une fois qu’ils ont été créés (un objet immuable)

##### 2. Comment créer un tuple ?

Pour créer un tuple, on utilise les parenthèses `()` puis on place les éléments à l'intérieur en les séparant par une virgule.



```
# Créer un tuple vide
mon_tuple = ()

```

Pour créer un tuple , vous pouvez utiliser la syntaxe suivante:

```
mon_tuple = (1,7,"voiture", True)
type(mon_tuple)
```

```
<class 'tuple'>
```

##### 3. Affichage

```
mon_tuple[0]
```

```
1
```

```
mon_tuple[1] = "famille"
```

On utilisera un tuple pour définir des sortes de constantes qui n'ont donc pas vocation à changer.

```{admonition} <font color='blue'> Remarque</font>
:class: tip

Les tuples sont surtout utiliser pour définir les constantes qui n'ont donc pas vocation à changer. 

les tuples ne permettent pas d'ajouter, de supprimer ou de modifier des éléments une fois créés. Toute tentative de modification d'un tuple entraînera une erreur.

```
##### 4. Concaténation

```
tuple1 = (0, 8, 1, 2, 3)
tuple2 = ('Ali', 'said', 'Fatima')
print(tuple1 + tuple2)
```

```
(0, 8, 1, 2, 3, 'Ali', 'said', 'Fatima')
```

```
tuple3=(0, 8, 1, 2, 3, 'Ali', 'said', 'Fatima')
print(len(tuple3))
```

Parfois, les tuples ne sont pas entourés de parenthèses, même s’il s’agit quand même de tuples.

```
a,b = 2, 3
print(a)
print(b)
#Ceci revient
(a,b) = (2, 3)
```