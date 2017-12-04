---
title : Introduction to Functions
description : This chapter will teach the basics about functions, such as defining and calling functions
---
## Defining Functions

```yaml
type: NormalExercise
lang: python
xp: 100
key: 8edbbb3a1d
```
This basic exercise will teach you how to create a function in python. 
Functions are defifne with two fundamental elements:

1. Header:
   The header includes the keyword, def, the name of the function, and parameters the function requires.
2. Body:
   The body includes the statements that will be carries out by the function when executed.
  
`@instructions`
- Create a function named `hello_world`
- Inside the body, use `print()` to display the string `"Hello World!"`.

`@hint`
- Use the keyword, `def`, and follow by the name of the function and parentheses, (), to create a funtion. 
- Include the statement `print()`, with `"Hello World!"` inside the parentheses, in the body.

`@sample_code`
```{python}
# Create a new function using def()
# Write the code below
def ________():
    print(______)
    
# Call the function
hello_world()
```

`@solution`
```{python}
# Create a new function using def()
# Write the code below
def hello_world():
    print("Hello World!")
    
# Call the function
hello_world()
```

`@sct`
```{python}
success_msg("Great work!")
```
---
## Calling Functions

```yaml
type: NormalExercise
lang: python
xp: 100
key: c61d77322e
```
After defining a function, it must be called to be implemented. 
In the previous excercise, we created a function named `hello_world` and call the function in the last statement,`hello_world()`. 
Using this statement, we tell the program to look for the function name `hello_world` and exexute it
  
`@instructions`
- Create a function named `Sum` that prints the answer of `1+1`.
- Call the function

`@hint`
To call the function, use the name of the function follow by a parentheses, (), just like the previous excercise where we use `hello_world()`.

`@sample_code`
```{python}
# Create a new function named "Sum"
def ________():
    # Print the Sum of 1+1
    print(______)
  
# Call the function 

```

`@solution`
```{python}
# Create a new function named "Sum"
def Sum():
    # Print the sum of 1+1
    print(1+1)
  
# Call the function 
Sum()
```

`@sct`
```{python}
success_msg("Great work!")
```
