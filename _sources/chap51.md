#### Eléments théoriques


##### 1. Différents types de données

Les données peuvent se présenter sous des formes variées, et chaque type de données requiert des méthodes spécifiques de représentation graphique afin de faciliter leur analyse et leur interprétation. Voici une description détaillée de ces catégories :

```{admonition} Types de données

- Données structurées :

Les données structurées sont organisées selon un format précis, ce qui les rend facilement exploitables par des outils d’analyse. Ces données incluent, par exemple, les résultats de sondages, des fichiers contenant des notes académiques, ou encore des listes de préférences. Leur structure permet une représentation claire sous forme de tableaux, de diagrammes ou d'histogrammes, ce qui facilite l'identification de tendances ou de relations.

- Séries temporelles: 

Les séries temporelles concernent des données collectées ou observées sur une période donnée, permettant d’étudier l’évolution de phénomènes dans le temps. Par exemple, l’analyse de la variation de la température moyenne terrestre, des fluctuations des marchés financiers ou encore du nombre hebdomadaire de cas de grippe repose sur ce type de données. Les graphiques en courbes, les diagrammes de tendances et les visualisations dynamiques sont souvent utilisés pour en saisir les évolutions et les patterns.

- Données géographiques :

Ces données décrivent des phénomènes localisés dans l’espace et sont souvent associées à des coordonnées géographiques. Elles permettent de cartographier des phénomènes tels que la répartition des espèces végétales dans différentes régions, l’indice de pauvreté au niveau mondial ou encore la position d’un téléphone portable à un moment donné. La cartographie thématique, les diagrammes en couches et les systèmes d’information géographique (SIG) constituent des outils privilégiés pour leur analyse.

- Données non structurées:

Contrairement aux données structurées, les données non structurées n’ont pas de format standard ou organisé. Elles incluent, par exemple, des contenus textuels, des images, des vidéos ou des enregistrements audio. Ces données nécessitent des techniques avancées, telles que l’analyse textuelle, la reconnaissance d’images ou encore l’apprentissage automatique, pour en extraire des informations exploitables. Leur représentation graphique peut inclure des nuages de mots, des diagrammes d’association ou des visualisations basées sur des modèles d’apprentissage.
```

##### 2. Types de variables

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

##### 3. Axes de données

Les données peuvent être classées selon leurs dimensions, chacune nécessitant des axes spécifiques pour leur visualisation.

```{admonition} Axes de données

**Les données unidimensionnelles  (1D)**: Elles se concentrent sur une seule variable et peuvent être représentées sur un axe linéaire.

- La répartition des âges dans une population : représentée par un histogramme pour montrer la fréquence des différentes tranches d’âge.

- Les résultats d’un examen pour une classe : affichés sous forme d’un graphique en barres où chaque barre représente une note et sa fréquence.

- Le nombre de visiteurs dans un musée sur une journée : visualisé par un diagramme en bâtons.

**Données temporelles** : Les données temporelles, bien qu'unidimensionnelles dans leur nature, évoluent dans le temps. Elles utilisent un axe temporel pour montrer l’évolution ou les tendances.

- L'évolution du prix du pétrole sur une année : illustrée par un graphique en courbes pour montrer les fluctuations mensuelles.

- Le suivi des températures quotidiennes dans une ville : représenté par une courbe qui met en évidence les variations journalières.

- Les ventes trimestrielles d’une entreprise : affichées sur un graphique de tendances pour analyser les performances commerciales.

- Les pics d’affluence dans les transports publics : représentés par un graphique en aires pour visualiser les périodes de forte fréquentation.

**Données bidimensionnelles (2D)** : Les données bidimensionnelles mettent en relation deux variables sur un plan cartésien ou une carte.

- La relation entre l'âge et le revenu d’un groupe de personnes : visualisée par un graphique de dispersion pour identifier des corrélations.

- La répartition des écoles dans une région : représentée sur une carte géographique avec des points localisant chaque établissement.

- La consommation énergétique en fonction de la température extérieure : illustrée par un graphique en lignes croisées.

- Une carte montrant le taux de vaccination par région : représentée par une carte thématique avec des zones colorées selon le pourcentage de vaccination.

**Données tridimensionnelles (3D)**  Elles ajoutent une profondeur supplémentaire, permettant de visualiser simultanément trois variables.

- La topographie d’un territoire : représentée par une carte en relief ou un graphique de surface en 3D montrant les variations d’altitude.

- La variation de la température, de l’humidité et de la pression atmosphérique dans une région : affichée sur un diagramme en 3D pour analyser les interactions entre ces variables.

- L’analyse des ventes par produit, par région et par période : visualisée par un histogramme 3D où chaque dimension représente une variable.
- Les trajectoires des vols aériens : illustrées sur une carte en 3D montrant les altitudes et les itinéraires.

**Données arborescentes et graphes** : Ces données illustrent des relations hiérarchiques ou des réseaux complexes.

- Un arbre généalogique : représenté sous forme d’arborescence montrant les relations familiales entre individus.

- La hiérarchie d’une entreprise : visualisée par un organigramme indiquant les liens entre les différents départements et postes.

- Les connexions entre utilisateurs d’un réseau social : représentées par un graphe où chaque nœud correspond à un individu et chaque lien montre une interaction.

- L’analyse des flux logistiques d’une entreprise : illustrée par un diagramme en arbre pour montrer les chemins empruntés par les produits, de la production à la distribution.
```

##### 6. Bonne pratiques

```{admonition} Bonne pratiques

**Comment choisir le graphique adapté à chaque type de données ?**

**Quelles sont les pièges à éviter ?**