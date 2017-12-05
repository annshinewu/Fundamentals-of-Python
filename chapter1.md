---
title       : Standard Data Types
description : In this chapter, we will explore the various standard data types used in Python.
attachments :
  slides_link : 

---
## Introducing Standard Data Types

```yaml
type: MultipleChoiceExercise
lang: python
xp: 50
skills: 1
key: c4dee315d7
```

Which one of these is not one of the five standard data types in Python?

`@instructions`
- Number
- While Loop
- String
- Tuple
- List
- Dictionary

`@hint`
Which does not represent or store a specific value or variable?

`@pre_exercise_code`
```{python}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer


```

`@sct`
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct!"
msg_success = "Exactly! A while loop is not a standard data type."
test_mc(2, [msg_bad, msg_success, msg_bad, msg_bad, msg_bad, msg_bad])
```

---
## Introducing Strings!

```yaml
type: NormalExercise
lang: python
xp: 100
skills: 1
key: b0a5dd001a
```

So... what do you think a string is?

A string is a contingous set of characters represented in quotation marks. For example, this would be a string: `"Hello, I am a string."`.

`@instructions`
- Declare a string called `string1` and set its value to `"I am the first string"`
- Print `string1`
- Declare a second string called `string2` and set its value to `"I am the second string"`
- Print `string2`

`@hint`
- You don't have to program anything for `string1`. It has already been declared, initialized, and printed.
- Use the sample code provided for `string1` to declare, initialized, and print `string2`

`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}
# Declare and initialize string1
string1 = "I am the first string"
print (string1)
string2 = ___
print (___)
```

`@solution`
```{python}
# Declare and initialize string1
string1 = "I am the first string"

# Print string1
print (string1)
# Declare and initialize string2
string2 = "I am the second string"

# Print string2
print (string2)
```

`@sct`
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki
test_object("string1", eq_condition="equal", do_eval=True, undefined_msg="Your string1 has not been defined", incorrect_msg="Your string1 is not initialized properly")
test_object("string2", eq_condition="equal", do_eval=True, undefined_msg="Your string2 has not been defined", incorrect_msg="Your string2 is not initialized properly")
test_output_contains("I am the first string", pattern=False, no_output_msg= "You have not printed string1 correctly")
test_output_contains("I am the second string", pattern=False, no_output_msg= "You have not printed string2 correctly")

success_msg("Great work!")
```

---
## String Operations

```yaml
type: NormalExercise
key: 4e96055c96
lang: python
xp: 100
skills: 2
```
As we have learned in the previous lesson, in order to print a complete string, you must call "print (string_name)" 
But other than printing the entire string, are there some ways you could print a subset of a string?
`@instructions`
- There are various ways to print a subset of strings
- For example, you can specify which character to print by indicating its index within the whole string or indicating a range of indexes.
- Look at the sample code for the various ways to print a string.
- Now, work on string2 (which has already been defined for you) to print various ranges of the string.

`@hint`
- The index of the first character in a string is ZERO, not one!
`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}
string1 = "My favorite fruit is "
print (string1)          # Prints complete string
print (string1[0])       # Prints first character of the string
print (string1[1:5])     # Prints characters starting from 2nd to 5th
print (string1[7:])      # Prints string starting from 8th character
print (string1 * 5)      # Prints string 5 times
print (string1 + "apples!") # Prints concatenated string

string2 = "This is an exercise to print strings."
print (___) # 1. Print the complete string
print (___) # 2. Print the 5th character
print (___) # 3. Print characters starting from the 5th to 7th
print (___) # 4. Print all characters starting from the 9th character
print (___) # 5. Print the string 7 times
print (___) # 6. print a concatentated string by adding "YAY!"
```

`@solution`
```{python}
string1 = "My favorite fruit is "
print (string1)          # Prints complete string
print (string1[0])       # Prints first character of the string
print (string1[1:5])     # Prints characters starting from 2nd to 5th
print (string1[7:])      # Prints string starting from 8th character
print (string1 * 5)      # Prints string 5 times
print (string1 + "apples!") # Prints concatenated string

string2 = "This is an exercise to print strings. "
print (string2)          # 1. Print the complete string
print (string2[4])       # 2. Print the 5th character
print (string2[4:5])     # 3. Print characters starting from the 5th to 7th
print (string2[8:])      # 4. Print all characters starting from the 9th character
print (string2 * 7)      # 5. Print the string 7 times
print (string2 + "YAY!") # 6. print a concatentated string by adding "YAY!"
```

`@sct`
```{python}
test_output_contains("This is an exercise to print strings.", pattern=False, no_output_msg= "You have not printed the first instruction correctly")
test_output_contains(" ", pattern=False, no_output_msg= "You have not printed the second instruction correctly")
test_output_contains("is an exercise to print strings. ", pattern=False, no_output_msg= "You have not printed the third instruction correctly")
test_output_contains("is an exercise to print strings. ", pattern=False, no_output_msg= "You have not printed the second instruction correctly")
test_output_contains("n exercise to print strings. ", pattern=False, no_output_msg= "You have not printed the fourth instruction correctly")
test_output_contains("This is an exercise to print strings. This is an exercise to print strings. This is an exercise to print strings. This is an exercise to print strings. This is an exercise to print strings. This is an exercise to print strings. This is an exercise to print strings. ", pattern=False, no_output_msg= "You have not printed the fifth instruction correctly")
test_output_contains("This is an exercise to print strings. YAY!", pattern=False, no_output_msg= "You have not printed the sixth instruction correctly")

success_msg("Great work!")
```
