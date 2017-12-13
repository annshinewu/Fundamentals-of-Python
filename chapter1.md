---
title       : Decision Making & Loops
description : Insert the chapter description here
attachments :
  slides_link : https://s3.amazonaws.com/assets.datacamp.com/course/teach/slides_example.pdf


---
## Comparators

```yaml
type: NormalExercise
key: d286c86bf8
lang: python
xp: 100
skills: 2
```

There are six types of comparators:

1. (==) : Equals to
    
2. (<) : Less than
    
3. (<=) : Less than or equal to
    
4. (>) : Greater than

5. (>=) : Greater than or equal to

6. (!=) : Not equal to

Each of these comparator statements yields one of two values: True, False.

`@instructions`

Look at the unfinished statements.

Finish them by adding True or False, depending on the comment in the line above, to the variables.

Note that characters are compared using ASCII numbers (A = 65 and Z = 90 in increasing order)

So for example : b < c yields True

`@hint`
Try running the codes in the Python Shell!

`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}
# 5 < 4
bool_one =

# 5 != 3
bool_two =

# (5 * 3) > (4 * 4)
bool_three =

# 100 >= (50 * 2)
bool_four =

# 70 <= (4 * 35)
bool_five =

# (25 * 3) == (6 * 5)
bool_six =

# 'g' > 'b'
bool_seven =

# 'r' == 'a'
bool_eight =

```

`@solution`
```{python}
# 5 < 4
bool_one = False

# 5 != 3
bool_two = True

# (5 * 3) > (4 * 4)
bool_three = False

# 100 >= (50 * 2)
bool_four = True

# 70 <= (4 * 35)
bool_five = True

# (25 * 3) == (6 * 5)
bool_six = False

# 'g' > 'b'
bool_seven = True

# 'r' == 'a'
bool_eight = False

```

`@sct`
```{python}
test_object('bool_one', eq_condition = "equal", do_eval=True, incorrect_msg = "bool_one seems a bit off.")
test_object('bool_two', eq_condition = "equal", do_eval=True, incorrect_msg = "Check bool_two again.")
test_object('bool_three', eq_condition = "equal", do_eval=True, incorrect_msg = "Are you sure about bool_three?")
test_object('bool_four', eq_condition = "equal", do_eval=True, incorrect_msg = "Look at bool_four one more time.")
test_object('bool_five', eq_condition = "equal", do_eval=True, incorrect_msg = "bool_five seems a bit off")
test_object('bool_six', eq_condition = "equal", do_eval=True, incorrect_msg = "Check bool_six again.")
test_object('bool_seven', eq_condition = "equal", do_eval=True, incorrect_msg = "Are you sure about bool_seven?")
test_object('bool_eight', eq_condition = "equal", do_eval=True, incorrect_msg = "Look at bool_eight one more time.")

success_msg = "Congratulations!"
```


---
## Boolean Operators

```yaml
type: NormalExercise
key: 5149299321
lang: python
xp: 100
skills: 2
```
Now you have learned about comparators, lets combine more comparators in a statement!

Key words are used to combine the comparators:

1. (and) : requires both statement to be True

2. (or) : only requires one statement to be True

3. (not) : Gives the opposite of the statement



`@instructions`
Assign the according output for each statement in the comment above of the variables

For example:

(25 * 5) == (4 * 16) or (2 * 3) == (6)

bool = True

Since it is an 'or' statement, and the second statement is true, the value assigned should be true.

`@hint`
Remember what 'and' and 'or' requires

Be careful of the 'Not'

`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}
# (34) != (43) and (3*12) > (12)
bool_one = 

# (22) <= (11*2) or Not ((4) > (12)
bool_two = 

# (3) >= (43) or Not((42) > (12))
bool_three = 

# (7*8) != (78) and Not False
bool_four = 

# Not False and Not True
bool_five = 
```

`@solution`
```{python}
# (34) != (43) and (3*12) > (12)
bool_one = True

# (22) <= (11*2) or Not ((4) > (12)
bool_two = True

# (3) >= (43) or Not((42) > (12))
bool_three = False

# (7*8) != (78) and Not False
bool_four = True

# Not False and Not True
bool_five = False
```

`@sct`
```{python}
test_object('bool_one', eq_condition = "equal", do_eval=True, incorrect_msg = "bool_one seems a bit off.")
test_object('bool_two', eq_condition = "equal", do_eval=True, incorrect_msg = "Check bool_two again.")
test_object('bool_three', eq_condition = "equal", do_eval=True, incorrect_msg = "Are you sure about bool_three?")
test_object('bool_four', eq_condition = "equal", do_eval=True, incorrect_msg = "Look at bool_four one more time.")
test_object('bool_five', eq_condition = "equal", do_eval=True, incorrect_msg = "bool_five seems a bit off")

```

---
## Logic (If Else)

```yaml
type: NormalExercise
key: 3743d3d127
lang: python
xp: 100
skills: 2
```
'If' is a conditional statement that executes the code wrapped inside if the expression is True.

The syntax for If statements is:

    if (5 == 5):
        print('Hi')
        
Since the expression in the if statement (5 == 5) yields True, the statement wrapper inside the if statement will be executed and 'Hi' will be printed

'Else' is a complement statement that executes the code inside if the if statement is False

An example for if-else statements would be:

    if(5!=5):
        print('Hi')
    else:
        print('Bye')
        
Since the expression in the if statement (5!=5) yields False, the statement in the if statement will not be executed, and thus moved on to the next statement
the else statement, executing the statement wrapped in else, which is to print 'Bye'

`@instructions`
Create an if statement comparing variable x with the string 'bananas', and make the statement wrapped inside print the string 'I love bananas!'

Then, create an else statement with the statement that prints the string 'I love apples!'

Run the code, and see which output will be printed!

(variable x has already been assigned to a value)

`@hint`
Review the syntax 
`@pre_exercise_code`
```{python}
x = 'apples'

```

`@sample_code`
```{python}
if ( ___ == ___):
    print (___)
else:
    print (___)
```

`@solution`
```{python}
if (x == 'bananas'):
    print ('I love bananas!')
else:
    print ('I love apples!')
```

`@sct`
```{python}
test_output_contains('I love apples!', pattern = False, no_output_msg = 'Did you properly code the if expression?')
success_msg = "Congratulations!"
```


---
## Elif Statement

```yaml
type: NormalExercise
key: 2d9ecedd68
lang: python
xp: 100
skills: 2
```

Another statement other than if and else is 'elif', which is short for else if

The elif statement is used when the if expression is False

It allows the programmer to provide a new condition after the first if statement

The statement in elif will execute if its expression yields True, or else it passes to the next elif statement or else statement

There can be infinite amount of elif statement, but in an if-elif-else statement, only one statement will be executed.

An example of an elif statement would be:

    if(5==6):
        print('one')
    elif(5==5):
        print('two')
    else:
        print('three')
Since 5 does not equal to 6, the if statement will not be executed, so the code moves on the the next statement.

in the elif expression, since 5 equals to 5, the computer will execute the statement wrapped inside elif and print the string 'two'

Since one statement has already been executed, the program jumps out from the if-elif-else statement, so the else statement will not be executed.

`@instructions`
Add an elif statement in between the if and else statements, and set the expression so that it compares variable x to string 'avocado' by seeing if they are equal

Run the code and see what is the output!
`@hint`
Review the elif syntax and make sure to add the correct expression

`@pre_exercise_code`
```{python}
x = 'avocados'
```

`@sample_code`
```{python}
if (x == 'bananas'):
    print ('I love bananas!')
#insert your code here
___
else:
    print ('I love apples!')
```

`@solution`
```{python}
if (x == 'bananas'):
    print ('I love bananas!')
elif(x == 'avocados'):
    print ('I love avocados!')
else:
    print ('I love apples!')
```

`@sct`
```{python}
test_output_contains('I love avocados!', pattern = False, no_output_msg = 'Did you properly code the if expression?')
success_msg = "Congratulations!"
```

---
## While Loops

```yaml
type: NormalExercise
key: 5dd1342b15
lang: python
xp: 100
skills: 2
```
In this exercise, you will be learning about 'While Loops'

A while loop loops the statement wrapped inside as long as its condition is fulfilled, or yields the value True.

This is the basic syntax for a while loop is:

    while(condition):
        statement(s)

The basic flow of a while loop is:

1. First, the while loop checks the condition

2. If the condition is true, then it iterates the statements wrapped inside once.

3. It checks for the condtion again: repeats step 2 if it is True, if False, the program exits the loop

An example of a while loop would be:

    x = 2
    while(x < 4):
        print (x)
        x += 1

In this code, x is initially declared as the integer 2.

Then it goes in the while loop

First iteration, it yields True since 2 < 4, thus the program prints x and increases x by 1

It continues on for another iteration before the expression becomes 4 < 4, which is False, thus exiting the while loop.

`@instructions`
Variable x has already been declared for you.

Create a while loop that has a condtion of x being greater than or equal to 2

And inside the while loop, it prints the string "x" and decreases varaible x by 1.

Run the program and see how many times is "x" printed.
`@hint`
Review the syntax of while loop and see where to put the condition and statements.

`@pre_exercise_code`
```{python}
x = 10

```

`@sample_code`
```{python}

```

`@solution`
```{python}
while ( x >= 2):
    print("x")
    x -= 1

```

`@sct`
```{python}
test_object('x', eq_condition = "equal", do_eval=True, incorrect_msg = "Is the condition set for while loop correct?")

test_output_contains('x\nx\nx\nx\nx\nx\nx\nx\nx\n', pattern = False, no_output_msg = 'Is the output correct?')


```

---
## For Loops

```yaml
type: NormalExercise
key: 28273d4514
lang: python
xp: 100
skills: 2
```
An alternatwive for using a while loop would be a For Loop.

The syntax of a for loop is:

for x in range(10):

The for loop above iterates starting from x = 0 all the way till x = 10, meaning that it has iterated for 10 times.

`@instructions`
Create a for loop that iterates variable x for 15 times, 

each time aggregating x's value by timing 2

and finally, print out x's final value
`@hint`
Recall the example for for loop with the range(number)

Remember, the instruction says to print out the FINAL value of x, not in each iteration

`@pre_exercise_code`
```{python}
x = 1
```

`@sample_code`
```{python}

```

`@solution`
```{python}
for x in range(15):
    x *= 2
print (x)
```

`@sct`
```{python}
test_object('x', eq_condition = "equal", do_eval=True, incorrect_msg = "Check your for loop condition and increasing statement again.")

```


---
## Loop Control Statements

```yaml
type: NormalExercise
key: 28fb295e0c
lang: python
xp: 100
skills: 2
```
Another usage for loops is loop control statements.

It is similar to a normal loop, but the uniqueness is that it checks for specific requirements through every iteration of a et of data.

For example:

    for x in range(25):
        if x % 2 == 0:
            print (x)

A loop control statement is basically a loop that contains a conditional statement, controlling each executive statement inside the loop for each iterations.

In the example above, it prints all even numbers (with the expression of x%2==0, finding all numbers divisible by 2) wihtin the range of 0 to 25(using the for loop)

Loop Control Statements are especially useful when processing arrays or a set of data.
`@instructions`
An array named array has already been declared for you.

Create a loop control statement that iterates every element in array, and prints out the value if the element in the array is greater than or equal to the first element.

**first element is already named 'first'
`@hint`

`@pre_exercise_code`
```{python}
array = [5, 3, 7, 8, 2, 7, 9, 2, 7, 5, 6, 10, 12, 3, 2, 14, 6]
```

`@sample_code`
```{python}
first = array[0]

```

`@solution`
```{python}
first = array[0]
for x in array:
    if(x >= first):
        print (x)
```

`@sct`
```{python}
test_output_contains('5\n7\n8\n7\n9\n7\n5\n6\n10\n12\n14\n6', pattern = False, no_output_msg = 'Is the output correct?')

```

---
## Nested Loops

```yaml
type: NormalExercise
key: 2260e70a56
lang: python
xp: 100
skills: 2
```
In this exercise, you will be learning how loops can be within loops, and its usage.

The basic structure of a nested loop codew segment is:

    while(condition):
        while(condition):
            statements
        statements


`@instructions`
array a and b have already been declared for you

Create a nested loop that checks if each of the element in array a is in either one of the elements in array b, checking separately.

If it is true, then it will print out the element; it prints nothing if it is false.

`@hint`
Use for loops to check every element in the arrays
`@pre_exercise_code`
```{python}
a = [312, 51312, 51, 31, 34, 52, 52, 43, 73, 34, 72, 34]
b = [51, 73, 31, 452, 5622, 3123, 52, 34, 513, 623, 6]

```

`@sample_code`
```{python}
for ____ in ____:
    for ____ in ____:
        if (________):
            ________
            break
```

`@solution`
```{python}
for x in a:
    for y in b:
        if (x == y):
            print (x)
            break
```

`@sct`
```{python}
test_output_contains('51\n31\n34\n52\n52\n73\n34\n34', pattern = False, no_output_msg = 'Check the parameter of for loops and conditions in if statement')

```

---
## Practice Decision Making & Loops

```yaml
type: NormalExercise
key: 79b97721b4
lang: python
xp: 100
skills: 2
```
In this chapter, you've learned about comparators, if-elif-else statements, for/while loops, loop control statements, and nested loops.

Now it's time to combine them altogether!

`@instructions`
array a, b, and c has already been declared for you and array b and c have same sizes of 7 elements.

Create a code that compares a element in array a to every element in arrays b and c.

The requirements are:

1. the element must be greater than all elements in array b

2. the element must be smaller than all the elements in array c

Once that element of array a meets both of the requirements, it is then printed out.

Fill in the blanks of the code to have the correct output.


`@hint`
Make sure to include two requirements in the if statement that alters check (using keyword 'and')

Check to see if the arrays that are iterating are correct.
`@pre_exercise_code`
```{python}
a = [3, 623, 45, 63, 110, 130, 411, 149, 91]
b = [31, 41, 5, 3, 42, 62, 34]
c = [31231, 4123, 412, 634, 423, 986, 150]
```

`@sample_code`
```{python}
check = True
for ___ in ____:
    for index in range(___):
        if(_______):
            check = ___
        else:
            check = ___
            break
    if(___):
        print(___)
```

`@solution`
```{python}
check = True
for x in a:
    for index in range(7):
        if(x > b[index] and x < c[index]):
            check = True
        else:
          check = False
          break
    if (check):
      print (x)

```

`@sct`
```{python}
test_output_contains('63\n110\n130\n\n149\n91', pattern = False, no_output_msg = 'The output is wrong, check the code again')

```
