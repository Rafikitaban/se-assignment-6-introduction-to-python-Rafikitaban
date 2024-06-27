[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15339563&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

Python is a high-level, interpreted programming language known for its simplicity and readability, which makes it accessible to beginners while being powerful enough for experienced developers.

Key Features include the following
Readability and Simplicity: Python's syntax is clear and concise, making it easy to learn and use.

Extensive Standard Library: Python comes with a rich standard library that supports many common programming tasks such as file I/O, system calls, and internet protocols.

Dynamic Typing and Automatic Memory Management: Python handles data types and memory allocation automatically, simplifying code development.

Cross-Platform Compatibility: Python runs on many operating systems, allowing for cross-platform development.

Large and Active Community: A vibrant community contributes to a vast ecosystem of third-party libraries and frameworks.

Versatility: Python is used for various applications, from web development to data analysis, scientific computing, artificial intelligence, and more.

Effective use cases
Web Development: Frameworks like Django and Flask make it easy to build robust web applications quickly.

Data Science and Analytics: Libraries like Pandas, NumPy, and Matplotlib are essential for data manipulation, analysis, and visualization.

Automation and Scripting: Python's simplicity and power make it an excellent choice for writing scripts to automate repetitive tasks.


2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

Download the Installer:
Go to the Python official website.
Click on the "Download Python" button to get the latest version.

Run the Installer:
Locate the downloaded installer file (usually in the Downloads folder) and double-click to run it.
Check the box "Add Python to PATH" at the bottom of the installer window.
Select "Install Now" or choose "Customize Installation" if you need to modify the installation settings.

Verify the Installation:
Open Command Prompt (type cmd in the Start menu and press Enter).
Type python --version and press Enter. This should display the installed Python version.
You can also verify the installation by typing pip --version to check if the package manager is installed correctly.

Set Up virtual environment
Open Command Prompt.
Navigate to the directory where you want to create your virtual environment.
Create a virtual environment using the venv module.

Activate the Virtual Environment
To activate the virtual environment, run: env\Scripts\activate

Install Packages in the Virtual Environment:
With the virtual environment activated, you can install packages using pip, run: pip install package_name

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

print("Hello, World!")

The print() function is a built-in Python function used to output text or other information to the console.
In this case, it outputs the string "Hello, World!".

The text "Hello, World!" is a string, which is a sequence of characters enclosed in quotation marks.
Strings in Python can be enclosed in either single (' ') or double (" ") quotation marks.

The print function is followed by parentheses ().
These parentheses are used to pass arguments (in this case, the string "Hello, World!") to the function.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

Integer (int): Whole numbers, positive or negative, without a decimal point.

Float (float): Numbers with a decimal point or in exponential (scientific) notation.

Boolean(bool): Represents one of two values: True or False.Used in conditional statements and logical operations.

List (list): An ordered collection of items (of any data type), enclosed in square brackets.

Tuple (tuple): An ordered collection of items similar to a list, but immutable (cannot be changed), enclosed in parentheses

Dictionary (dict): A collection of key-value pairs, enclosed in curly braces.

Set (set): An unordered collection of unique items, enclosed in curly braces.

5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

   Conditional statements in Python are used to perform different actions based on whether a condition is true or false. The primary conditional statements are if, elif (short for else if), and else.

   age = 16

if age < 16:
    print("You are a minor.")
elif age == 16:
    print("You are a teenager")
else:
    print("You are an adult.")

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

Functions in Python are reusable blocks of code that perform specific tasks. They allow you to organize your code, improve readability, and avoid redundancy. 

Modularity: Functions break down complex problems into smaller, manageable parts. You can focus on implementing individual functions and then combine them to build more complex functionality.

Reusability: Once defined, functions can be reused throughout your program. You don’t need to rewrite the same logic multiple times.

Abstraction: Functions abstract away implementation details. You can use a function without knowing how it works internally.

def add_numbers(a, b):
    """
    This function takes two arguments and returns their sum.
    """
    return a + b

'''Example of calling the function'''

result = add_numbers(3, 5)
print("The sum is:", result)

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

Ordered: Elements in a list are ordered and can be accessed by their index.

Indexed: You can access elements using their position (index) in the list.

Mutable: Elements in a list can be changed after the list is created.

Duplicate Elements: Lists can contain duplicate elements.
Syntax: Defined using square brackets [].

Unordered: Elements in a dictionary are not ordered and accessed by keys.

Key-Value Pairs: Consist of unique keys mapped to values.
Mutable: Values associated with keys can be changed, but keys themselves must be immutable.

Unique Keys: Keys in a dictionary must be unique.

Syntax: Defined using curly braces {} with key-value pairs separated by colons.

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

Exception handling in Python allows you to manage errors gracefully, preventing the program from crashing unexpectedly. It provides a mechanism to detect and handle errors, offering a way to continue program execution or provide useful feedback to the user.

'try' block 
try:
    file = open(file_path, 'r')
    data = file.read()
    print("File content:")
    print(data)

'except' block
except FileNotFoundError as e:
    print(f"Error: {e}")
except IOError as e:
    print(f"Error: {e}")
 
 'finally'
finally:
    try:
        file.close()
        print("File closed.")
    except UnboundLocalError:
        print("No file to close.")

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

Modules:
A module is a single file containing Python code. It can include functions, classes, and variables.
Modules allow you to organize your code into reusable components.
You can create your own custom modules or use built-in modules provided by Python.

Packages:
A package is a collection of related modules grouped together in a directory hierarchy.
Packages help organize large projects by providing a structured way to manage multiple modules.
A package typically contains an __init__.py file (which can be empty) to indicate that it’s a package.

Importing using math module:
import math

# Calculate the square root
x = 25
sqrt_x = math.sqrt(x)
print(f"Square root of {x} is {sqrt_x:.2f}")

# Calculate the factorial
n = 5
factorial_n = math.factorial(n)
print(f"Factorial of {n} is {factorial_n}")

# Use mathematical constants
pi_value = math.pi
print(f"Value of pi: {pi_value:.4f}")

Output 
Square root of 25 is 5.00
Factorial of 5 is 120
Value of pi: 3.1416


10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

Reading from a File:
To read the content of a file, you can use the open() function with the appropriate mode (e.g., 'r' for reading).

def read_file(filename):
    try:
        with open(filename, 'r') as file:
            content = file.read()
            print(content)
    except FileNotFoundError:
        print(f"File '{filename}' not found.")
# Usage:
read_file("sample.txt")

To write data to a file, use the open() function with the 'w' mode (for writing).

def write_to_file(filename, data_list):
    try:
        with open(filename, 'w') as file:
            for item in data_list:
                file.write(item + "\n")  # Add a newline after each string
        print(f"Data written to '{filename}'.")
    except Exception as e:
        print(f"Error writing to '{filename}': {e}")

# Example data (list of strings):
my_strings = ["Hello", "World", "Python", "File I/O"]

# Usage:
write_to_file("output.txt", my_strings)

# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


