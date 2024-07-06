### Python Basics

#### What is Python?
Python is a high-level, interpreted programming language known for its simplicity and readability. It supports multiple programming paradigms and is widely used for various applications from web development to scientific computing.

#### Key Features
- **Easy to Read**: Clean and concise syntax.
- **Versatile**: Supports both procedural and object-oriented programming.
- **Extensive Libraries**: Rich standard library and numerous third-party packages.
- **Interpreted**: No compilation step, immediate feedback.
- **Platform Independent**: Runs on Windows, macOS, Linux, and more.

#### Use Cases
- **Web Development**: Frameworks like Django and Flask.
- **Data Analysis**: Libraries like Pandas and NumPy.
- **Machine Learning**: Libraries like TensorFlow and PyTorch.
- **Automation**: Scripting tasks and workflows.

### Installing Python

#### Steps to Install Python
1. **Download Python**: Go to [python.org](https://www.python.org/downloads/) and download the installer for your operating system.
   
2. **Run Installer**: Execute the downloaded installer and follow the prompts.

3. **Verify Installation**: Open a terminal or command prompt and type:
   ```bash
   python --version
   ```

#### Setting Up a Virtual Environment
1. **Install virtualenv** (if not installed):
   ```bash
   pip install virtualenv
   ```

2. **Create a virtual environment**:
   ```bash
   virtualenv venv
   ```

3. **Activate the virtual environment**:
   - On Windows:
     ```bash
     venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source venv/bin/activate
     ```

### Python Syntax and Semantics

#### Hello World Program
```python
# This is a comment
print("Hello, World!")
```

#### Basic Syntax Elements
- **Print Statement**: Outputs text to the console.
- **String**: Enclosed in quotes (`" "`).

### Data Types and Variables

#### Basic Data Types
- **int**: Integer numbers (e.g., `5`).
- **float**: Floating-point numbers (e.g., `3.14`).
- **str**: Strings of text (e.g., `"Hello"`).
- **bool**: Boolean values (`True` or `False`).

#### Example Script
```python
# Variables
num1 = 5
num2 = 3.5
name = "Alice"
is_valid = True
```

### Control Structures

#### Conditional Statements and Loops

##### If-Else Statement
```python
# Example if-else statement
x = 10
if x > 5:
    print("x is greater than 5")
else:
    print("x is less than or equal to 5")
```

##### For Loop
```python
# Example for loop
for i in range(5):
    print(i)
```

### Functions in Python

#### What are Functions?
Functions are reusable blocks of code that perform a specific task. They improve code readability, modularity, and maintainability.

#### Example Function
```python
# Function definition
def add_numbers(a, b):
    return a + b

# Function call
result = add_numbers(3, 5)
print("Sum:", result)
```

### Lists and Dictionaries

#### Differences Between Lists and Dictionaries

- **Lists**: Ordered collection of items accessed by index.
- **Dictionaries**: Unordered collection of key-value pairs.

#### Example Script
```python
# List
numbers = [1, 2, 3, 4, 5]

# Dictionary
person = {'name': 'Alice', 'age': 30, 'city': 'New York'}

# Basic operations
print(numbers[0])           # Accessing the first element in the list
print(person['name'])       # Accessing value by key in dictionary
numbers.append(6)           # Adding an element to the list
person['email'] = 'alice@example.com'  # Adding a new key-value pair to dictionary
```

### Exception Handling

#### What is Exception Handling?
Exception handling is a mechanism to handle runtime errors gracefully without terminating the program.

#### Example Script
```python
# Example with try-except-finally
try:
    x = 1 / 0  # Division by zero
except ZeroDivisionError:
    print("Error: Division by zero!")
finally:
    print("This will always execute, regardless of exception.")
```

### Modules and Packages

#### Modules and Packages in Python

- **Modules**: Python files containing definitions and statements.
- **Packages**: Directories of Python modules with a `__init__.py` file.

#### Example Using Math Module
```python
# Importing the math module
import math

# Using math module
print(math.sqrt(25))   # Square root function
print(math.pi)         # Value of pi
```

### File I/O

#### Reading from and Writing to Files

#### Reading a File
```python
# Reading from a file
with open('file.txt', 'r') as file:
    content = file.read()
    print(content)
```

#### Writing to a File
```python
# Writing to a file
data = ["Line 1\n", "Line 2\n", "Line 3\n"]
with open('output.txt', 'w') as file:
    file.writelines(data)
```

---

