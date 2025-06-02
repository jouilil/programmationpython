#  Conditional Structures


## 1. The if Statement

```{admonition} Definition
:class: attention

The if statement tests a condition and executes a block of code only if the condition is true.

```

**Syntax**

```
if (condition) then
    instructions    
end if
```
**Examples**

```
if (temperature > 30) then
    print("It is hot")
end if

if age >= 18:
    print("You are eligible to vote.")
end if

```

## 2. The if-else Statement

```{admonition} Definition
:class: attention

This structure provides an alternative set of instructions if the condition is false.
```

**Syntax**
```
if (condition) then
    instructions if true
else
    instructions if false
end if
```

**Examples**

```
if (score >= 10) then
    print("Passed")
else
    print("Failed")
end if
```

## 3. The if-else if Ladder

```{admonition} Definition
:class: attention
The if-else if Ladder : Used when multiple conditions must be checked in sequence.
```
**Syntax**
```
if (condition1) then
    instructions
else if (condition2) then
    instructions
else
    default instructions
end if
```
