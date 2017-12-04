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
Functions are defifne with two fundamental conponents:
1. Header:
   The header includes the keyword, def, the name of the function, and parameters the function requires.
2. Body:
   The body includes the statements that will be carries out by the function.
  
`@instructions`
- Create a function named hello_world that prints the string "Hello World!".

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
test_error()
test_object("hello_world()",
            undefined_msg = "You didn't declared the function hello_world() ",
            incorrect_msg = "Did you declare the function properly?")
success_msg("Great work!")
```

## Calling Functions

```yaml
type: NormalExercise
lang: python
xp: 100
key: 8edbbb3a1d
```
After defining a function, it must be called to be use. 
In the previous exercise, we create a function call "hello_world". In the last line of the code, we use the statement, hello_world(), to tell the program to look for the function called spam and execute it.
Now, you will learn how to do it.
  
`@instructions`
- Create a function named Sum that prints the answer of 1+1.
- Call the function

`@hint`
To call the function, use the name of the function follow by a parentheses, (), just like the previous excercise where we use "hello_world()".

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
test_error()
test_object("hello_world()",
            undefined_msg = "You didn't declared the function hello_world() ",
            incorrect_msg = "Did you declare the function properly?")
success_msg("Great work!")
```
