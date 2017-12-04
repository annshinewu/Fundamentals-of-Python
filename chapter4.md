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
This basic exercise will challenge you to create a function in python. 
Functions are defifne with two fundamental conponents:
1. Header:
   The header includes the keyword, def, the name of the function, and parameters the function requires.
2. Body:
   The body includes the statements that will be carries out by the function.
  
`@instructions`
- Create a function called hello_world that prints the string "Hello World!".

`@hint`
Use the keyword def and follow by the name of the function and parentheses, (), to create a funtion. 
Then, include the statement that prints "Hello World!" in the body.

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

test_function("numpy.unique",
              not_called_msg = "Don't remove the call of `np.unique` to define `ints`.",
              incorrect_msg = "Don't change the call of `np.unique` to define `ints`.")

success_msg("Great work!")
```
