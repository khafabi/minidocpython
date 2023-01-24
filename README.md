# Lists

Сделать лучше: Заменить пример "список из букв" на что-то попроще и полаконичнее
Статус: Prod
Тема: 1. Introduction to Python
Чему научили: Список: синтаксис, содержимое; индексы; сложение списков; len()

**Lists** are sequences of numbers, strings, or other values.

You've already assigned numeric and string values to variables. Variables can also contain lists in the same way.

The contents of the lists are written in square brackets and elements of the list are separated by a comma:

```python
new_list = [<element>, <element>, <element>, <element>, <element>]
```

In the variable `english_alphabet`, we'll save a list consisting of letters of the alphabet. A letter is a string, so each element is in quotes:

```python

english_alphabet = ['a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p','q','r','s','t','u','v','w','x','y','z']

```

What does the variable `english_alphabet` contain?

```python

print(english_alphabet)
# Returns:
# ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z']

```

Each element has its own serial number — **index**. Using the index, you can get the value of an element from a list.

Check in the simulator what this code's output will be:

```python

english_alphabet = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z']

print(english_alphabet[1]) # Print the content of the element with its index 1
print(english_alphabet[2]) # Print the content of the element with its index 2

```

Surprise! The output is:

```python

b
c

```

Hmm, index `1` didn't return the first element of the list. It returned the second. But there's no error here. Counting in the lists starts from zero.

The first element has the zero index:

```python

print(english_alphabet[0])
# Print the content of the element with its index
# Returns: а
```

The list of numbers may look like this:

```python

countdown = [5, 4, 3, 2, 1, 0]

```

You can make a list of expressions and it will store the calculated values:

```python

# store the second and the third rows of the Pythagoras table in the lists
pithagoras_2 = [
    2*1, 2*2, 2*3, 2*4, 2*5, 2*6, 2*7, 2*8, 2*9
]
pithagoras_3 = [
    3*1, 3*2, 3*3, 3*4, 3*5, 3*6, 3*7, 3*8, 3*9
]
print(pithagoras_2)
print(pithagoras_3)

```

```python

[2, 4, 6, 8, 10, 12, 14, 16, 18]
[3, 6, 9, 12, 15, 18, 21, 24, 27]

```

You can add another list to a list stored in a variable. For example, let's recruit the band members of The Beatles:

```python

# A list can contain just one element. There is only John Lennon in the frontman list:
# frontman only John Lennon:
frontman = ['John']

# A different list contains several musicians
members = ['Paul', 'Ringo', 'George']

# The addition of lists results in a new list
the_beatles = frontman + members

# Now the band is full:
print(the_beatles)

# Returns: ['John', 'Paul', 'Ringo', 'George']

```

There is a standard function that counts the elements of a list `len()`.

```python

count = len(the_beatles)
print(count)

# Returns 4

```

```python
count = len(the_beatles)
print(count)

# Returns 4
```

## Task 1

Teach Iris to work with the friends list.
To do this, create the `friends` list containing elements in this order:`'Joey'`, `'Monica'`, `'Ross'`, `'Phoebe'`, `'Chandler','Rachel'`.

After you've created the `friends` list, print its content.

---

### Прекод

```python
print("Hello, I'm Iris!")
# finish the code below
friends = ...
```

### Hint

A list is written in square brackets. Each element is written in quotes (the name is the same string), separated by comma: `['Joey', 'Monica', 'Ross', 'Phoebe', 'Chandler', 'Rachel']`

Print the content of the `friends` list with the `print` function

### Success text

The list is created. It looks good. And now Iris knows who you are friends with. This is useful information for a personal assistant.

### Авторское решение

```python
print("Hello, I'm Iris!")
friends = ['Joey', 'Monica', 'Ross', 'Phoebe', 'Chandler', 'Rachel']
print(friends)
```

Тест

```python
# <!subteam^S02TD0J0E90> https://prestable.admin.team.practicum.com/faculties/5cdff940-05cf-4e1d-bfb2-8c4ea1e2952a/professions/0a91dc59-5bca-47d1-b192-0f341fe40176/tracks/e576b321-5066-4ad9-baeb-53c7b1578787/courses/da38a75e-248e-42cf-aeb8-e072c7dbf41e/topics/5d71237f-5aca-4ed5-be35-5889bf4c39fd/lessons/15f8962e-b783-47fc-bdcc-6789af409631/tasks/36f637ea-f37c-4e23-a71e-b3e2a1fb1d4c/test/

# COMMENT: changed 03.09.2021, 08.09.2021

_test.var('friends', m='The list items are written in square brackets separated by commas.')
_test.output(
    m=(
        'Unexpected output.<br>'
  		  'Your output:\n\n'
  		  f'```\n{_u._output}\n```\n\n'
  		  'Expected:\n\n'
        f'```\n{_a._output}\n```'
    )
)
```

- **ТЕСТЫ (AST)**
    
    ```python
    # <!subteam^S025RGQEJLR> https://prestable.admin.praktikum.yandex-team.ru/faculties/5cdff940-05cf-4e1d-bfb2-8c4ea1e2952a/professions/b5efac65-18c4-430f-a037-84cd7f72f617/tracks/d614460f-9709-4960-a51e-5f811f1800b1/courses/d1f214bf-341d-445f-8950-0387f8bd2c83/topics/f52e6249-a2f2-48bd-8b2e-d5943748565e/lessons/81202c5f-64cf-4f7a-a0a1-355a13a224cd/tasks/c26d00be-f3f3-4035-9784-236c3321488e/test
    
    # COMMENT: changed 03.09.2021, 08.09.2021
    
    _test.var('friends', m='A list is written in square brackets.')
    _test.output(
        m=(
          'Your program output does not match the expected.<br>'
      		'Your output:\n\n'
      		f'```\n{_u._output}\n```\n\n'
      		'Expected:\n\n'
          f'```\n{_a._output}\n```'
        )
    )
    ```
    

## Task 2

It's time for Iris to be polite and learn how to say hi. Iris, greet Phoebe first!

Add the code so that your program prints the phrase *Hi Phoebe, I'm Iris!*

### Precode

```python
friends = ['Joey', 'Monica', 'Ross', 'Phoebe', 'Chandler', 'Rachel']

# assign the value to the index variable,
# so that Phoebe is selected from the friends list
index = ...

print("Hello, ' + friends[index] + ", I'm Iris!")
```

### Solution

```python
friends = ['Joey', 'Monica', 'Ross', 'Phoebe', 'Chandler', 'Rachel']

# assign the value to the index variable,
# so that Phoebe is selected from the friends list
index = 3

print("Hello, ' + friends[index] + ", I'm Iris!")
```

Тест

```python
# <!subteam^S025RGQEJLR> https://prestable.admin.praktikum.yandex-team.ru/faculties/5cdff940-05cf-4e1d-bfb2-8c4ea1e2952a/professions/b5efac65-18c4-430f-a037-84cd7f72f617/tracks/d614460f-9709-4960-a51e-5f811f1800b1/courses/d1f214bf-341d-445f-8950-0387f8bd2c83/topics/f52e6249-a2f2-48bd-8b2e-d5943748565e/lessons/81202c5f-64cf-4f7a-a0a1-355a13a224cd/tasks/a3afd01a-7556-4459-900a-b3a45b03515f/test

# COMMENT: changed 22.07.2021, 08.09.2021

_test.call('print')
_test.output(
    m=(
       'Unexpected output.<br>'
  		 'Your output:\n\n'
  		 f'```\n{_u._output}\n```\n\n'
  		 'Expected:\n\n'
       f'```\n{_a._output}\n```'
    )
)
```

### Hint

All that is required is to assign a value to the `index` variable so that Phoebe is selected from the friends list. What is her position in the list? What index does the counting in the lists start from?

Don't change the string with the `print()` call.

### Success text

Don't have a hundred friends: by the time Iris says hi to everyone, the party will be over! But now it's clear why the index of the element is needed in the list.

## Task 3

Iris shouldn't just know your friends, but also be able to say something about them.

The `index` variable contains the number of the friend whose information we are interested in.

Get the value of the element with the index stored in the `index` variable from the `friends` list and teach Iris to print the message:

***{friend's name with the index number}** lives in New York*

### Precode

```python
print("Hello, I'm Iris!")
friends = ['Joey', 'Monica', 'Ross', 'Phoebe', 'Chandler', 'Rachel']

# you can change the index before sending it to the verification
# and see what the code does
index = 2

# add your code here
```

### Hint

For example, you can write this: `print(friends[index], 'lives in New York')`

### Success text

Alright, let's go to New York!

Just kidding :) Let's go back to coding.

### Авторское решение

```python
print("Hello, I'm Iris!")
friends = ['Joey', 'Monica', 'Ross', 'Phoebe', 'Chandler', 'Rachel']

friend_index = 2
print(friends[friend_index] + 'lives in New York')
```

Тест

```python
# <!subteam^S02TD0J0E90> https://prestable.admin.team.practicum.com/faculties/5cdff940-05cf-4e1d-bfb2-8c4ea1e2952a/professions/0a91dc59-5bca-47d1-b192-0f341fe40176/tracks/e576b321-5066-4ad9-baeb-53c7b1578787/courses/da38a75e-248e-42cf-aeb8-e072c7dbf41e/topics/5d71237f-5aca-4ed5-be35-5889bf4c39fd/lessons/15f8962e-b783-47fc-bdcc-6789af409631/tasks/a094336c-c6a0-46c8-a03a-0e21b57f50c7/test/

# COMMENT: changed 22.07.2021, 08.09.2021

_test.call('print', args=["Hi, I'm Iris!"])
mess = 'The output doesn't match the task'
if 'lives' in _u._output:
    _a.output = _a._output.replace('lives', 'lives')

_test.output(
    m=(
        'Unexpected output.<br>'
        'Your output:\n\n'
        f'```\n{_u._output}\n```\n\n'
        'Expected:\n\n'
        f'```\n{_a._output}\n```'
    )
)
```

## Task 4

Let's give Iris some functionality. We'll teach her to count friends.

1. Declare the variable `count` and store the number of friends in it. Count them by calling the `len()` function.
2. {{Display}}[be_eng_python_Display] the `You have {number} friends` string, where `{number}` is the value of the variable `count`.

---

### Precode

```python
print("Hello, I'm Iris!")
friends = ['Joey', 'Monica', 'Ross', 'Phoebe', 'Chandler', 'Rachel']

# add your code here
```

### Hint

```python
`print('You have'+ str(count) + ' friends')`
```

### Success text

Iris learned to count the items on the list and say how many there are. Children usually start doing this by the age of two. But Iris learns a lot faster. Soon she'll take over the world! Just kidding :)

### Solution

```python
print("Hello, I'm Iris")
friends = ['Joey', 'Monica', 'Ross', 'Phoebe', 'Chandler', 'Rachel']
count = len(friends)
print('You have'+ str(count) + ' friends')
```

Тест

```python
# <!subteam^S02TD0J0E90> https://prestable.admin.team.practicum.com/faculties/5cdff940-05cf-4e1d-bfb2-8c4ea1e2952a/professions/0a91dc59-5bca-47d1-b192-0f341fe40176/tracks/e576b321-5066-4ad9-baeb-53c7b1578787/courses/da38a75e-248e-42cf-aeb8-e072c7dbf41e/topics/5d71237f-5aca-4ed5-be35-5889bf4c39fd/lessons/15f8962e-b783-47fc-bdcc-6789af409631/tasks/e3f72850-d709-40d4-bf57-a6f7792a5732/test/

# COMMENT: changed 22.07.2021, 08.09.2021

_test.call('print')
_test.output(
    m=(
         'Unexpected output.<br>'
  		   'Your output:\n\n'
  		   f'```\n{_u._output}\n```\n\n'
  		   'Expected:\n\n'
         f'```\n{_a._output}\n```'
    )
)
```

### Glossary keys

[be_eng_python_Display]  

Output to the screen. Provided by the `print()` function.
