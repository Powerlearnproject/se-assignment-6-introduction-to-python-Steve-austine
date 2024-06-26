[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15333279&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

Python is a high-level, interpreted programming language known for its readability and simplicity. Here are some key features:

- **Readable and Maintainable Code**: Python's clean syntax helps developers write readable and maintainable code.
- **Extensive Standard Library**: Python comes with a rich standard library that supports many common programming tasks such as file I/O, system calls, and data manipulation.
- **Interpreted Language**: Python is an interpreted language, which means code is executed line by line, making debugging easier.
- **Dynamic Typing**: Python handles data types dynamically, which means you don't need to declare variable types explicitly.
- **Cross-Platform Compatibility**: Python can run on various operating systems like Windows, macOS, and Linux without requiring significant changes.
- **Community and Libraries**: Python has a large community and an extensive collection of third-party libraries that extend its capabilities.

**Use Cases:**

- **Web Development**: Frameworks like Django and Flask make web development quick and efficient.
- **Data Science and Machine Learning**: Libraries like Pandas, NumPy, and Scikit-learn are widely used for data analysis and machine learning.
- **Automation and Scripting**: Python is ideal for automating repetitive tasks and writing scripts.
- **Software Development**: Python can be used for developing desktop applications and even some mobile applications.



2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

1. **Download**: Go to the [official Python website](https://www.python.org/downloads/) and download the installer for Windows.
2. **Run Installer**: Execute the installer. Ensure you check the "Add Python to PATH" option.
3. **Verify Installation**:
   ```
   python --version
   ```
4. **Set Up Virtual Environment**:
   ```
   python -m venv myenv
   myenv\Scripts\activate
   ```

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

```python
print("Hello, World!")
```

**Explanation:**

- **print**: A built-in function that outputs text to the console.
- **"Hello, World!"**: A string literal enclosed in double quotes.
- **()**: Parentheses are used to pass arguments to functions.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

**Basic Data Types:**

- **int**: Integer numbers, e.g., `1`, `42`.
- **float**: Floating-point numbers, e.g., `3.14`, `0.001`.
- **str**: Strings, e.g., `"Hello"`, `"Python"`.
- **bool**: Boolean values, `True` or `False`.
- **list**: Ordered collections of items, e.g., `[1, 2, 3]`.
- **dict**: Key-value pairs, e.g., `{"name": "Alice", "age": 30}`.
- **tuple**: Ordered, immutable collections of items, e.g., `(1, 2, 3)`.
- **set**: Unordered collections of unique items, e.g., `{1, 2, 3}`.

**Script:**

```python
# Integer
a = 10
print(a, type(a))

# Float
b = 3.14
print(b, type(b))

# String
c = "Hello, Python"
print(c, type(c))

# Boolean
d = True
print(d, type(d))

# List
e = [1, 2, 3]
print(e, type(e))

# Dictionary
f = {"name": "Alice", "age": 30}
print(f, type(f))

# Tuple
g = (1, 2, 3)
print(g, type(g))

# Set
h = {1, 2, 3}
print(h, type(h))
```
5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

   **Conditional Statements:**

Conditional statements allow you to execute certain pieces of code based on whether a condition is true or false.

**Example of if-else statement:**

```python
x = 10
if x > 5:
    print("x is greater than 5")
else:
    print("x is not greater than 5")
```

**Loops:**

Loops are used to execute a block of code multiple times.

**Example of for loop:**

```python
numbers = [1, 2, 3, 4, 5]
for number in numbers:
    print(number)
```

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

Functions are reusable blocks of code that perform a specific task. They help in organizing code, making it more readable and maintainable.

**Example:**

```python
def add(a, b):
    return a + b

# Calling the function
result = add(5, 3)
print(result)
```

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

   *Lists:**

- Ordered collections of items.
- Accessed by index.
- Allows duplicate elements.

**Dictionaries:**

- Unordered collections of key-value pairs.
- Accessed by key.
- Keys must be unique.

**Script:**

```python
# List
numbers = [1, 2, 3, 4, 5]
numbers.append(6)
print(numbers)
print(numbers[2])

# Dictionary
person = {"name": "Alice", "age": 30}
person["email"] = "alice@example.com"
print(person)
print(person["name"])

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.


Exception handling allows you to handle runtime errors gracefully and execute code even if an error occurs.

**Example:**

```python
try:
    result = 10 / 0
except ZeroDivisionError as e:
    print(f"Error occurred: {e}")
finally:
    print("This block is always executed")
```

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.


**Modules:**

Modules are Python files containing code (variables, functions, classes) that can be reused in other Python programs.

**Packages:**

Packages are collections of modules grouped under a common directory.

**Example:**

```python
import math

# Using the math module
result = math.sqrt(16)
print(result)
```

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.


**Reading from a file:**

```python
with open('example.txt', 'r') as file:
    content = file.read()
    print(content)
```

**Writing to a file:**

```python
lines = ["Line 1", "Line 2", "Line 3"]
with open('example.txt', 'w') as file:
    for line in lines:
        file.write(line + "\n")

# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].
