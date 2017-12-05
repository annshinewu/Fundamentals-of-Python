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
print string1

# Declare and initialize string2
string2 = "I am the second string"

# Print string2
print string2

```

`@sct`
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki
test_output_contains("I am the first string", pattern=False, no_output_msg= "You have not printed string1 correctly")
test_output_contains("I am the second string", pattern=False, no_output_msg= "You have not printed string2 correctly")
test_object(string1, eq_condition="equal", do_eval=True, undefined_msg="Your string1 has not been defined", incorrect_msg="Your string1 is not initialized properly")
test_object(string2, eq_condition="equal", do_eval=True, undefined_msg="Your string2 has not been defined", incorrect_msg="Your string2 is not initialized properly")

success_msg("Great work!")
```
