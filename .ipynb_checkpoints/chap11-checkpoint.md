# Introduction to Algorithms



##### 1.  What's an algorithm ?

```{admonition} <font color='blue'>Algorithmics</font>
:class: tip

**Algorithmics** refers to the discipline that studies algorithms and their applications in computer science.

```

```{admonition} <font color='blue'> Algorithm </font>
:class: tip

**An algorithm** is any well-deûned computational procedure that takes some value,
or set of values, as input and produces some value, or set of values, as output in a
ûnite amount of time. An algorithm is thus a sequence of computational steps that
transform the input into the output.

```

##### 2.  Algorithmics vs Algorithm

```{admonition} <font color='blue'>Algorithmics vs Algorithm</font>
:class: tip

- **Algorithm**: A specific procedure or set of instructions for solving a problem.

- **Algorithmics**: The field of study that focuses on the design, analysis, and optimization of algorithms.
```



```{admonition} <font color='blue'>Examples of Algorithms</font>
:class: tip

- Weather prediction algorithm


- Traffic light control algorithm

- Sorting and Searching Algorithms

- Machine Learning and AI Algorithms

- Spam filtering algorithm (used in email services)

- Face recognition algorithm (used in security systems)

- Speech recognition algorithm (used in virtual assistants)

- Fraud detection algorithm (used in banking)

- Recommendation system algorithm (used in Netflix, YouTube)

An algorithm can be, for example, a cooking recipe:

- Ingredients

- Follow a recipe

- Final dish

```

##### 3. Algorithm vs program

```{admonition} algorithm vs program
**An algorithm** is a general procedure or logical sequence for solving a problem.

**A program** is the actual implementation of an algorithm in a programming language that a computer can execute.


```

**Example** : Here is an algorithm/a Python program that asks the user to enter a number and then calculates its double:


**Algorithm**: Calculate Double of a Number

- Step 01 : Start

- Step 02 : Prompt the user to enter a number

- Step 03 : Read the number

- Step 04 : Compute the double of the number (result = number × 2)

- Step 05 : Display the result

- Step 06 : End

**Program** : Calculate Double of a Number

```python
# Ask the user to enter a number
num = float(input("Enter a number: "))

# Calculate the double
double_num = num * 2

# Display the result
print("The double of", num, "is", double_num)
```

**Example 02 :** Here is an algorithm/a program that asks the user to enter their age and then determines whether they are a minor or an adult.

**Algorithm: Check Majority**

- Step 01 : Start

- Step 02 : Ask the user to enter their age

- Step 03 : Read the age

- Step 04 : If the age is greater than or equal to 18, display "You are an adult". Otherwise, display "You are a minor"

- Step 05 : End

**Program: Check Majority**

```Python 
age = int(input("Enter your age: "))

# Check if the user is a minor or an adult
if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")
```

**Example of an algorithm** : To determine the largest number in a given list, the following steps are followed:

1. Start with the first number. 

2. Compare with the next number. 

3. Keep the largest and continue until the end. 

4. Output the largest number.

**Examples of a program** : Below is a Python implementation of the algorithm:

```Python 
numbers = [4, 7, 1, 9, 3]

print(max(numbers))

```

**Key difference :**

**An algorithm** is language-independent, whereas a program depends on a specific programming language. An algorithm outlines the logic, while a program translates that logic into executable code. 

**An algorithm** cannot be run directly, but a program can be executed by a computer.

##### 4. Steps of an Algorithm


```{admonition} <font color='blue'> Steps of an Algorithm </font>
:class: tip


- **Inputs**: This step involves identifying the necessary data required to solve the problem.

- **Processing**: This step determines how the input data is transformed to produce the desired results.

- **Outputs**: Displaying the results. This can include showing numerical values, generating reports, creating graphs, or any other form of presenting the results that helps the user understand the conclusions of the algorithm.

```

