# Les dictionnaires en Python
##### 1. Création

Un dictionnaire est une collection qui associe une clé à une valeur. Par exemple, il est possible d’associer la clé "nom" à un nom et la clé "prenom" à un prénom.

Pour créer un dictionnaire, on associe une clé à une valeur en les séparant par `:`, le tout entre accolades `{}` :



Pour initialiser un dictionnaire , on utile la syntaxe suivante:

```
my_dict = {}
```

```
my_dict = dict()
print(my_dict)
```

Affichage après exécution :

```
{}
```

##### 2. Comment ajouter des valeurs dans un dictionnaire

```
my_dict = {}
my_dict["nom"] = "youness"
my_dict["prenom"] = "jouilil"
print(my_dict)
```
Affichage après exécution :

```
{'nom': 'youness', 'prenom': 'jouilil'}

```
##### 3. Comment supprimer une entrée dans un dictionnaire
```
del my_dict["nom"]
```
Affichage après exécution :

```
{'prenom': 'jouilil'}
```


##### 4. Récupérer les clés et les valeurs d'un dictionnaire

###### 4.1. Récupérer les clés d'un dictionnaire python
```
my_dict = {"Adam" : (12, 16,0), "said": (17,8,9)}
print(my_dict.keys())
```
Affichage après exécution :
```
dict_keys(['Adam', 'said'])
```

###### 4.2. Récupérer les valeurs d'un dictionnaire python
```
my_dict = {"Adam" : (12, 16,0), "said": (17,8,9)}
print(my_dict.values())
```
Affichage après exécution :
```
dict_values([(12, 16, 0), (17, 8, 9)])
```
###### 4.3. Récupérer les clés et les valeurs d'un dictionnaire python
```
my_dict = {"Adam" : (12, 16,0), "said": (17,8,9)}
print(my_dict)
for cle, valeur in my_dict.items():
    print("les notes de M. ", cle, "en math , info, fran sont :", valeur)
```
Affichage après exécution :
```
les notes de M.  Adam en math , info, fran sont : (12, 16, 0)
les notes de M.  said en math , info, fran sont : (17, 8, 9)
```

```{admonition} Exercice
:class: tips 
Créez un dictionnaire appelé personne avec les clés suivantes : "nom", "âge", "ville", et assignez-leurs des valeurs appropriées.

- Affichez la valeur associée à la clé "âge" dans le dictionnaire personne.
- Ajoutez une clé "profession" avec une valeur associée au dictionnaire personne.
- Affichez le dictionnaire mis à jour.
- Supprimez la clé "ville" du dictionnaire personne et affichez le dictionnaire mis à jour.

```
