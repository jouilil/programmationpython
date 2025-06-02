# General Structure of an Algorithm

An algorithm follows a structured format that ensures clarity and logical flow.

```{admonition} General Structure
:class: tip

An algorithm consists of the following sections:

- **Algorithm Name** – Identifies the algorithm.

- **Declaration Section** – Defines variables and data types.

- **Action Section** – Enclosed between ‘Begin’ and ‘End’, where operations and logic are executed.

```

**Example**

This algorithm reads two numbers, adds them, and displays the result.

```
Algorithm SumTwoNumbers  

// Declaration Section  
var num1, num2, sum as Integer  

// Action Section  
Begin  
   Read(num1, num2)  
   sum ← num1 + num2  
   Display(sum)  
End
```