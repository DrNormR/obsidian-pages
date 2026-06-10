---
{"dg-publish":true,"permalink":"/newman/stem-programming-presentation/variable-notes-reformatted/","noteIcon":""}
---


---

# Python Variables

## Python Variable Rules

![Pasted image 20260610095432.png](/img/user/Newman/STEM%20Programming%20Presentation/~media/Pasted%20image%2020260610095432.png)

Here are the rules for naming variables in Python:

1. Case-sensitive: Variable names are case-sensitive, meaning myVariable and myvariable are considered different variables.
2. Start with a letter or underscore: Variable names must start with either a letter (a-z or A-Z) or an underscore (_).
3. So you can do x1, but not 1x
4. Contain only letters, numbers, or underscores: Variable names can contain letters, numbers, and underscores, but cannot contain spaces or other special characters.
5. Avoid reserved keywords: Variable names cannot be the same as Python's reserved keywords (e.g., if, else, for, while, def).

Best Practices:

- Meaningful names: Choose variable names that clearly describe their purpose. For example, instead of using x, you could use customer_name.
- Use underscores for multiple-word names: If you need to use multiple words in a variable name, separate them with underscores (e.g., my_variable).
- Avoid using single-letter variables: While it's sometimes acceptable to use single-letter variables for temporary values, it's generally better to use more descriptive names.

By following these rules and best practices, you can create clear and readable Python code.

---

## Variable Types

![Pasted image 20260610095046.png](/img/user/Newman/STEM%20Programming%20Presentation/~media/Pasted%20image%2020260610095046.png)

- Variables come in different types
- I think of them like tools, because you need all different types depending on the job
- Integers
- floats
- strings
- booleans

1. Text Type:
	
	- str: String, used for text.
2. Numeric Types:
	
	- int: Integer, used for whole numbers.
	- float: Floating-point number, used for decimal numbers.
	- complex: Complex number, used for numbers with real and imaginary parts.
3. Sequence Types:
	
	- list: Ordered, mutable collection of items.
	- tuple: Ordered, immutable collection of items.
	- range: Represents a sequence of numbers.
4. Mapping Type:
	
	- dict: Dictionary, used for key-value pairs.
5. Set Types:
	
	- set: Unordered collection of unique items.
	- frozenset: Immutable version of a set.
6. Boolean Type:
	
	- bool: Boolean, used for True or False values.
7. Binary Types:
	
	- bytes: Immutable sequence of bytes.
	- bytearray: Mutable sequence of bytes.
	- memoryview: Allows access to the internal data of an object that supports the buffer protocol.
8. None Type:
	
	- NoneType: Represents the absence of a value or a null value.

---

# Integers

![Pasted image 20260610095614.png](/img/user/Newman/STEM%20Programming%20Presentation/~media/Pasted%20image%2020260610095614.png)

- An integer is also known as just a number, or maybe as a whole number

An integer variable in programming is a data type that stores whole numbers without decimal points. These numbers can be positive, negative, or zero.

Examples of integer variables:

```python
age = 25
year = 2023
temperature = -10
```

Key characteristics of integer variables:

- Whole numbers: Integers do not have decimal points.
- Range: The range of integers a programming language can represent depends on its implementation.
- Arithmetic operations: Integers can be used in addition, subtraction, multiplication, and division.
- Comparison operators: Integers can be compared using ==, !=, <, >, <=, >=.

Integer variables are commonly used in programming for various tasks, such as counting, indexing, and performing calculations.

## Code Examples

```python
myint = 5
print(myint)
```

```python
myint = 5
print(myint)

myint = 'cat'
print(myint)
```

```python
a = 5
b = 6
a = b
print(a)
print(b)
```

```python
a = 5
b = 6
# a = b
print(a)
print(b)
```

---

# Floats

![Pasted image 20260610100043.png](/img/user/Newman/STEM%20Programming%20Presentation/~media/Pasted%20image%2020260610100043.png)

- And now we have floats, which I like to call floating point decimal numbers
	- By the way, who likes a root beer float?
	- Forget the float, who loves root beer?
- So if you're a math person, you might not think there's a big difference between these
	- 5
	- 5.0
	- 5.0000000000
	- 000000005
	- 00005.000
- But this is where math guys and computer guys have a rare disagreement
	- For a computer, the difference between an integer and a float is really important
	- The reason is that all those zeroes have to be stored in memory, so they are meaningful
- Why do we call it a floating point?
	- [show Microsoft calculator]

A float variable in programming is a data type used to store real numbers that have decimal points.

Key characteristics of float variables:

- Decimal points
- Wide range
- Limited precision
- Arithmetic operations
- Comparison operators

Examples:

```python
pi = 3.14159
temperature = 25.7
discount = 0.2
```

## Code Examples

```python
myfloat = 13.51
print(myfloat)
```

```python
myfloat = 13.51
print(myfloat)

myfloat = 13
print(myfloat)
```

---

# Booleans

![Pasted image 20260610100127.png](/img/user/Newman/STEM%20Programming%20Presentation/~media/Pasted%20image%2020260610100127.png)

- Now let's talk about Boolean values
- These are true/false values
- In programming, they are very often used with conditional statements

```python
isEmployee = True
print(isEmployee)
```

```python
isRaining = False
isHot = False
isSnowing = False

if isHot == True:
    print("You should wear shorts")
else:
    print("You should wear pants")
```

```python
print(1 == 1)
```

```python
print(1 == 1)
print(1 == 2)
print(100 > 0)
print(100 < 0)
print(55 <= 55)
print(55 >= 56)
```

Boolean values are a fundamental data type in programming that represent one of two states: True or False.

Examples:

```python
if x > 0:
    print("x is positive")
else:
    print("x is negative or zero")
```

```python
if (x > 0) and (y > 0):
    print("Both x and y are positive")
```

```python
def is_even(number):
    return number % 2 == 0
```

---

# Strings

![Pasted image 20260610100303.png](/img/user/Newman/STEM%20Programming%20Presentation/~media/Pasted%20image%2020260610100303.png)

- Now we get to the string data type
- Strings are usually abbrev. str
- Strings are called strings because they're a character string

```python
greeting = "Hello World!"
fruit = "apple"
```

```python
greeting = "Hello World!"
fruit = "apple"

print(greeting)
print("I would like to eat the", fruit)
```

```python
greeting = "Hello World!"
v1 = 'roller'
v2 = 'skates'

print(greeting)
print(v1 + v2)
```

Strings are immutable, indexable, sliceable, and support many operations.

Examples:

```python
first_name = "John"
last_name = "Doe"
full_name = first_name + " " + last_name

message = "Hello, world!"
index = message.find("world")

age = 30
greeting = f"You are {age} years old."

print(full_name)
print(index)
print(greeting)
```

---

# Mixing Data Types

![Pasted image 20260610100415.png](/img/user/Newman/STEM%20Programming%20Presentation/~media/Pasted%20image%2020260610100415.png)

```python
fav_Number = 12
tempF = 98.6
nickname = "Cobra"
is_student = True

print(fav_Number + tempF)
```

```python
fav_Number = 12
age = 20
tempF = 98.6
weight = 170.5
nickname = "Cobra"
fav_Color = 'blue'
is_student = True
is_right_handed = True

print(fav_Number + tempF)
print(fav_Number + age)
print(fav_Color + nickname)
```

```python
fav_Number = 12
age = 20
tempF = 98.6
weight = 170.5
nickname = "Cobra"
fav_Color = 'blue'
is_student = True
is_right_handed = True

print(fav_Number + tempF)
print(fav_Number + age)
print(fav_Color + nickname)
print(fav_Number + nickname)
```

```python
fav_Number = 12
age = 20
tempF = 98.6
weight = 170.5
nickname = "Cobra"
fav_Color = 'blue'
is_student = True
is_right_handed = True

print(fav_Number + tempF)
print(fav_Number + age)
print(fav_Color + nickname)
# print(fav_Number + nickname)

print(is_right_handed + is_student)
print(is_right_handed + age)
```

---

# Checking Variable Types

![Pasted image 20260610100503.png](/img/user/Newman/STEM%20Programming%20Presentation/~media/Pasted%20image%2020260610100503.png)

```python
fav_Number = 12
tempF = 98.6
nickname = "Cobra"
is_student = True

type(is_student)
```

```python
fav_Number = 12
tempF = 98.6
nickname = "Cobra"
is_student = True

print(type(is_student))
```

```python
print('My favorite number is', fav_Number, 'and my current body temp is ', tempF, 'It is ', is_right_handed, 'that I\'m right-handed')
```

Escape characters:

```
\n  Newline
\t  Tab
\\  Backslash
\'  Single Quote
\"  Double Quote
```

---

