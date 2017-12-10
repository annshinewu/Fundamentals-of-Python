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

    def fcn_one(x):
        return x * 5

    def fcn_two(y):
    return fun_one(y) + 7

This program will take in a argument, `y`, and call the function `fcn_one` and pass in `y`, then plus 7 to the result return from `fcn_one`

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
# Create a new function named "Increment"
def ______(___,___):
    # Check if the number is eual to our goal
    if (___ == ___):
        return ___
    else:
        # Add one to the number
        ___ += 1
        # Call the function, Increment, and pass the number in.
        return ____
  
# Call the function 
print(Increment(0,10))
```

`@solution`
```{python}
# Create a new function named "Increment"
def Increment(num,goal):
    # Check if the number is eual to our goal
    if (num == goal):
        return num
    else:
        # Add one to the number
        num += 1
        # Call the function, Increment, and pass the number in.
        return Increment(num,goal)
  
# Call the function 
print(Increment(0,10))
```

`@sct`
```{python}
test_output_contains("10", no_output_msg = "The output is inccorect. Make sure the returned value is euqal to our goal, `10`.",pattern = False)
test_function("Increment", not_called_msg = "You didn't call the following function: Increment()")
test_function_definition("Increment", arg_names = False, arg_defaults = False)
success_msg("Great work!")
```

---
## Math Module

```yaml
type: NormalExercise
lang: python
xp: 100
key: 085e26ba73
```
In the previous exercises, we learn how to program `user-define function`, which is functions create by ourselves; However, there are many built-in `modules` that we can import. A module is a file that contains definitions, including variables and functions, that we can use.

    import math
    print(math.sqrt(25))

This program will output `5`, which is the answer of sqare roots 25. Adding `math.` infront is very crucial, since python doesn't know what sqrt() means, and the module named math that includes a number of useful variables and functions, and sqrt() is one of those functions. In order to access the function math, we need to tell Python to import from the math module.

`@instructions`
- import the module `math`.
- Print out the result of square roots 49

`@hint`
- Use math. infront of the function sqrt() and insert 49 between the parentheses, ().

`@sample_code`
```{python}
# Import math module
 
 
# Pring the result of square roots 49

```

`@solution`
```{python}
# Import math module
import math

# Pring the result of square roots 49
print(math.sqrt(49))
```

`@sct`
```{python}
test_output_contains("7", no_output_msg = "The output is inccorect. Make sure the output is `7`.",pattern = False)
test_import("math", same_as = True)
test_function("math.sqrt",
              incorrect_msg = "You didn't use `math.sqrt()` correctly.")
success_msg("Great work!")
```

---
## More Mathematical Functions

```yaml
type: NormalExercise
lang: python
xp: 100
key: 7723b9f10e
```
There are much more functions in `math` module other than `sqrt()`. For example: 

    1. sqrt(x) # Return the square roots of x
    2. fabs(x) # Return the absolute value of x
    3. pow(x,y) # Return the answer of x^y 
      (Note: x and y are double)
    4. cos(x) # Return the cosine of x in radians

`@instructions`
- import the module `math`.
- Use functions is math module to calculate the answer for the following equation, (5^3)^(1/2)
- print out the result

`@hint`
- Use sqrt() and pow()

`@sample_code`
```{python}
# Import math module
 
 
# Calculate (5^3)^(1/2) and store in `ans`
ans = _____

#Print out `ans`

```

`@solution`
```{python}
# Import math module
import math
 
# Calculate (5^3)^(1/2) and store in `ans`
ans = math.sqrt(math.pow(5.0,3.0))

#Print out `ans`
print(ans)
```

`@sct`
```{python}
test_import("math", not_imported_msg = "Did you import math?", same_as = True)
test_function("math.pow", incorrect_msg = "Did you use `math.pow()`?.")
test_output_contains("11.180339887498949", no_output_msg = "The output is inccorect. Make sure the output is the answer of `(5^3)^(1/2)`.",pattern = False)
success_msg("Great work!")
```

---
## Lambda Function

```yaml
type: MultipleChoiceExercise
lang: python
xp: 50
key: 290cb7555f
```
When we define a function we often give it a name; however, Python also supports creating `anonymous functions`, functions that define without a name, using a construct called `lambda`. Therefore, `anonymous functions` are also called `lambda functions`.

    def fcn_one(x):
        return x * 2
    print(fcn_one(2))
    
    num = lambda x: x*2
    print(num(2))

In the program above, lambda x: x * 2 is the lambda function. x is the argument and x * 2 is the expression that gets evaluated and returned. This function has no name. It returns a function object which is assigned to the `identifier`, a name used to identify a variable, `num`. 

Have a look at the choices. Select the lambda function that will return the same value as the following functions.

    def num(x):
	    return (math.pow(x,2))
	
 Test it out it the shell to see the different output.
 

`@instructions`
- num = def x: math.pow(x,2)
- num = lambda x: x**2
- def lambda(x):  return (math.pow(x,2))
- num = lambda x: math.pow(x,2)

`@hint`
- Remeber the return type of pow() is always double
- lambda function us the keyword `lambda` to define

`@pre_exercise_code`
```{python}
import math
```

`@sct`
```{python}
msg_bad = "That is incorrect! Try it on the shell to check"
msg_success = "Correct!"
test_mc(4, [msg_bad, msg_bad, msg_bad, msg_success])
```

---
## Falling Distance

```yaml
type: NormalExercise
lang: python
xp: 100
key: 105e15156b
```
In this exercise, we will be utilizing all the technques we learn in the chapter and write a program that help us calculate the falling distance of a object using the equation, `d = 0.5*g*t^2`.

The variables in the formula are as follows: d is the distance in meters. g is 9.8, and t is the amount of time, in seconds, that the object has been falling.

Also, we will importing the module `random` in this program and use the function `randint()` that help us generate random numbers.
For expample,  `random.randint(5,10)` will generate an integer between 5 and 10

`@instructions`
- Write a function named `getTime` that generate a number from 1~50 (inclusive).
- Write a function named `fallingDistance` that accepts an objects's falling time (in seconds) as an argument. (The function should return the distance, in meters, that the object has fallen durin that time interval.)
- Write a function named `printDistance` that accepts the distance calculated by `fallingDistance` and print it out in the following format: `Distance = __ meters`. Ex. Distance = 10 meters.

`@hint`
- Use the keyword, `import`, to import a module. Ex. `import math`
- Use the function, `randint()`in th randome module to genertate randome number. Ex. `random.randint(5,10)`
- To define a function use the keyword `def` follow by the name of the function, just like `def Sum()`
- To print the output using the format, simply use `+` to combine them. Ex. print(`x = `+str) will print `x = Hi` if str = Hi. (Note: to combine string with numerical variable type you need to cast it to string by using `str(num)`)

`@sample_code`
```{python}
# Import module needed


# Define the funcion getTime()
 
 
# Define the funcion fallingDistance()


# Define the funcion printDistance()


#Call the function getTime()
t = 

#Call the function fallingDistance()
d = 

#Call the function printDistance()

```

`@solution`
```{python}
# Import module needed
import random

# Define the funcion getTime()
def getTime():
    return random.randint(1,50)
 
# Define the funcion fallingDistance()
def fallingDistance(time):
    return 0.5*9.8*t**2

# Define the funcion printDistance()
def printDistance(distance):
    return "Distance: "+str(distance)+" meters"

#Call the function getTime()
t = getTime()

#Call the function fallingDistance()
d = fallingDistance(t)

#Call the function printDistance()
printDistance(d)
```

`@sct`
```{python}
test_import("random", not_imported_msg = "Did you import random?", same_as = True)
test_function_definition("getTime", arg_names = False, arg_defaults = False)
test_function_definition("fallingDistance", arg_names = False, arg_defaults = False)
test_function_definition("printDistance", arg_names = False, arg_defaults = False)
#test_function("random.randint", not_called_msg = "You didn't call the following function: random.randint()", incorrect_msg = "Did you call random.randint() with correct arguments?")
#test_function("str",not_called_msg = "You didn't call the following function: str()")
test_function("getTime", not_called_msg = "You didn't call the following function: getTime()")
test_function("fallingDistance", not_called_msg = "You didn't call the following function: fallingDistance()")
test_function("printDistance", not_called_msg = "You didn't call the following function: printDistance()")
success_msg("Great work!")
```