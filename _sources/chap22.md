# Data Types in Algorithms

Data types define the kind of data that a variable can store and the operations that can be performed on it. Different data types are used based on the nature of the data being manipulated and the tasks that need to be performed.


- Integer (whole numbers)

- Real (decimal numbers)

- Character (single letters)

- String (sequence of characters)

- Boolean (True or False)

<center>
    
![Drag Racing](1.JPG)
    
</center>


```{admonition} Exercise: Identify the variable types
:class: tip


Below are different variables with values. Write the correct type next to each variable:

- Variable A = 25 → Type = ?

- Variable B = -3.14 → Type = ?

- Variable C = "Hello" → Type = ?

- Variable D = 'Z' → Type = ?

- Variable E = True → Type = ?

- Variable F = 0 → Type = ?

- Variable G = "2025" → Type = ?

- Variable H = False → Type = ?


```


## Criteria for Variable Names in Algorithmics


```{admonition} Criteria for Variable Names

- Must start with a letter :  A variable name cannot start with a number or special symbol.

**Example** : 

Correct: total, Age

Incorrect: 1total, _Age

- Can contain letters, digits, or underscores

**Example** : 

score1, user_name

- No spaces allowed, Use an underscore _ or camelCase instead of spaces.

**Example** : 

Correct: totalAmount, total_amount

Incorrect: total amount

- Should not use reserved keywords : Do not use words like if, while, for that are used by the algorithm language.

**Example** : 

Incorrect: if = 10

- Should be meaningful : Choose a name that describes the data it holds.

**Example** : 

Good: price, userName

Bad: x, temp (unless for short-term or simple use)

- Case-sensitive (in most languages)

Total and total can be different variables.

```


```{admonition}  Exercise
:class: tip

Given the following variable names and their assignments, determine if each variable name adheres to the rules of valid variable naming. If any variable name violates a rule, suggest a corrected version.

- 123variable = 50

- total amount = 100

- student-Grade = 95

- if = 10

- score1 = 100

- _age = 25

- User$Name = "Alex"

- total_score = 150

- Grade = 85

```


## Declaring Variables

In structured pseudocode, a variable is declared before it is used. The declaration specifies the variable name and, optionally, its data type.

**General syntax:**

```
var variable_name as DataType

```

**Examples:**
```
var n as Integer
var name as String
var price as Real
var isAvailable as Boolean
```