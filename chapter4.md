---
title       : Introduction to Functions
description : This chapter will teach the basics about functions, suchs as defining and calling functions
---
## Defining Functions

```yaml
type: NormalExercise
lang: python
xp: 100
```
This basic exercise will challenge you to create a function in python. 
Functions are defifne with two fundamental conponents:
1. Header:
   The header includes the keyword, def, the name of the function, and parameters the function requires.
2. Body:
   The body includes the statements that will be carries out by the function.
   
`@instructions`
- Create a function called helloworld that prints the string "Hello World".

`@hint`
Use the keyword def and follow by the name of the function and parentheses, (), to create a funtion. 
Then, include the statement that prints "Hello World" in the body.

`@pre_exercise_code`
```{python}
# Create a new function using def()
# Write the code below
```
`@solution`
```{python}
# Create a new function using def()
# Write the code below
def helloworld():
   print("Hellow World!")
```

`@sct`
```{python}
test_error()
test_object("hellowworld()",
            undefined_msg = "Make sure to define the function!",
            incorrect_msg = "Have you correctly define the function?")
test_function("print",
               incorrect_msg = "Have you correctly use the "print()"?)
success_msg("Great work! You have sucessfully create a function.")
```
