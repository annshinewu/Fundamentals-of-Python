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
test_function_definition('hello_world', arg_defaults = False)
test_output_contains("Hello World!", no_output_msg = "Did you print `Hello World!`",pattern = False)
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
In the previous exercise, we created a function named `hello_world` and call the function in the last statement,`hello_world()`. 
Using this statement, we tell the program to look for the function name `hello_world` and execute it
  
`@instructions`
- Create a function named `Sum` that prints the answer of `1+1`.
- Call the function

`@hint`
To call the function, use the name of the function follow by a parentheses, (), just like the previous exercise where we use `hello_world()`.

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
test_function_definition('Sum', arg_defaults = False)
test_function("Sum", not_called_msg = "You didn't call the following function: Sum()")
test_output_contains("2", no_output_msg = "Did you print the result of `1+1`?",pattern = False)
success_msg("Great work!")
```

---
## Argument and Paremeters

```yaml
type: NormalExercise
lang: python
xp: 100
key: 8a9e65ebb1
```
In the previous exercises, we work on defeining and calling functions. Now, we are going to learn how to pass variables or values into a function. Looking at the following code: `def Sum(a, b)`. a and b is the parameter of the function, `Sum()`. A `parameter` acts as a variable name for a passed in `argument`. For example, we called the function with the following statement, `Sum(10,26)`. The argument passed in is 10 and 26. When the function was called, a holds the value 10 ,and b hols the value 26.
  
A function can require as many parameters as you like, but when you call the function, you should pass in the matching number of arguments.

`@instructions`
- Look at the function in the editor, `Subtract`. It should take in two arguments and subtract the two numbers. 
- Create a function named `Subtract` (this part is done for you).
- Fill in the paremeter so it perferm the function desired.
- Call the function with appropriate arguments that will output `5`

`@hint`
- To pass in arguments, you have to specify the paremeters in the parentheses, (). For example: def Multiply(a,b)
- To call the function, use the name of the function follow by a parentheses, ().
- To pass the arguments, type the number you want in the parentheses, (). Remind to seperate different arguments by comma.

`@sample_code`
```{python}
# Create a new function named "Subtract"
def Subtract(___,___):
    # Print the result of a-b
    print(a-b)
  
# Call the function 

```

`@solution`
```{python}
# Create a new function named "Subtract"
def Subtract(a, b):
    # Print the result of a-b
    print(a-b)
  
# Call the function 
Subtract(10,5)
```

`@sct`
```{python}
test_output_contains("5", no_output_msg = "The output is inccorect. Make sure the difference between two arguments is `5`?",pattern = False)
test_function_definition("Subtract", arg_names = True, arg_defaults = False)
test_function("Subtract", not_called_msg = "You didn't call the following function: ()")
success_msg("Great work!")
```

---
## Return

```yaml
type: NormalExercise
lang: python
xp: 100
key: 7cc546337c
```
In the body of the functions we defined in the prvious exercises, we use print to output the desired outcome. However, we can also use `return ` to escpae the function and send back a desired value.

`@instructions`
- Create a function named `CombineStr`.
- Fill in the paremeter so takes in two arguments.
- In the body of the function, combine the two `string` arguments, with a space between them and return the combined string.
- Call the function with appropriate arguments. (This part is done for you)

`@hint`
- To pass in arguments, you have to specify the paremeters in the parentheses, (). For example: def Multiply(a,b)
- To combine two string use `+`. For example: str1+str2
- To return the string type `return` and follow by the string that you want to return.

`@sample_code`
```{python}
# Create a new function named "CombineStr"
def ______(___,___):
    # Combine the two string
    combined = _____+" "+_____
    # Return the string
    
# Call the function 
print(CombineStr("Winnie","Li"))
```

`@solution`
```{python}
# Create a new function named "CombineStr"
def CombineStr(str1,str2):
    # Combine the two string
    combined = str1+" "+str2
    # Return the string
    return combined
  
# Call the function 
print(CombineStr("Winnie","Li"))
```

`@sct`
```{python}
test_output_contains("Winnie Li", no_output_msg = "The output is inccorect. Make sure to return the correct string.",pattern = False)
test_function("CombineStr", not_called_msg = "You didn't call the following function: CombineStr()")
test_function_definition("CombineStr", arg_names = False, arg_defaults = False)
success_msg("Great work!")
```

---
## Return True

```yaml
type: MultipleChoiceExercise
lang: python
xp: 50
skills: 1
key: c4dee315d7
```

Have a look at the choices. Select the one that returns the boolean value `True`.

Test it out it the shell to see the different output.

`@instructions`
- def ReturnTrue():
    return ("True")
- def ReturnTrue():
    return (Talse and False)
- def ReturnTrue():
    return (1 > 2)
- def ReturnTrue():
    return (1!= 1 or True)

`@hint`
- Test it out at the shell
- Remeber the function has to return the `boolean value` True
- `and` requires both condition to be true in order to return `True`
- `or` only requires one of the condition to be true.

`@sct`
```{python}
msg_bad = "That doesn't return the boolean value `True`"
msg_success = "Exactly! The function returns the boolean value `True`."
test_mc(4, [msg_bad, msg_bad, msg_bad, msg_success])
```

---
## Function Calling Function

```yaml
type: NormalExercise
lang: python
xp: 100
key: c9dae6a9e4
```
We've learn the basics of defining and calling functions and seen functions that print text or do simple arithmetic, but functions can do much more than that. For example, a function can call another function or itself, which is `recursive`. Look at the follow exmaple to better understand the idea.
`def fun_one(n):
  return n * 5

def fun_two(m):
  return fun_one(m) + 7`

`@instructions`
- Create a function named `Increment`.
- Fill in the paremeter so takes in two interger arguments. The first argument is the number to be added, and the second argument is the goal, which the first argument will be added untill it's equal to our goal.
- In the body of the function, add one to the first argument.
- Include an if-else statement in the body, so that when the number is equal to our goal the function will return the value. However, if it's not then it will call itself and take the number and the goal to be the arguments.
- Call the function with appropriate arguments. (This part is done for you)

`@hint`
- To pass in arguments, you have to specify the paremeters in the parentheses, (). For example: def Multiply(a,b)
- Adding one to the number simply use the arithemtic opertation, `+`.
- To create an if-statement, use the keyword `if` and type the condition in the parentheses, ().
- To return the value use `return` and follow by the variable that you want to return.
- Calling the function itself is like how we call another function in the previous exercises. Use `return` and follow by the name of the function and a parenthese with the right argument.

`@sample_code`
```{python}
# Create a new function named "CombineStr"
def ______(___,___):
    # Combine the two string
    combined = _____+" "+_____
    # Return the string
    
# Call the function 
print(CombineStr("Winnie","Li"))
```

`@solution`
```{python}
# Create a new function named "CombineStr"
def CombineStr(str1,str2):
    # Combine the two string
    combined = str1+" "+str2
    # Return the string
    return combined
  
# Call the function 
print(CombineStr("Winnie","Li"))
```

`@sct`
```{python}
test_output_contains("Winnie Li", no_output_msg = "The output is inccorect. Make sure to return the correct string.",pattern = False)
test_function("CombineStr", not_called_msg = "You didn't call the following function: CombineStr()")
test_function_definition("CombineStr", arg_names = False, arg_defaults = False)
success_msg("Great work!")
```