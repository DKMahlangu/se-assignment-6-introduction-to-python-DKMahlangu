# SE-Assignment-6
## Assignment: Introduction to Python

### 1. Python Basics:
**What is Python?** Python is an interpreted, object-oriented, high-level programming language with dynamic semantics. Its high-level built in data structures, combined with dynamic typing and dynamic binding, make it very attractive for Rapid Application Development, as well as for use as a scripting or glue language to connect existing components together.(https://www.python.org/doc/essays/blurb/)

#### Key Features of Python
- **Readable and Maintainable Code:** Python's clean and straightforward syntax allows developers to write code that is easy to read and maintain.
- **Extensive Standard Library:** Python has a rich standard library that provides modules and functions for various tasks, reducing the need for external libraries.
- **Dynamic Typing:** Python uses dynamic typing, meaning you don't need to declare the type of a variable explicitly.
- **Interpreted Language:** Python is an interpreted language, allowing you to run code directly without needing a compilation step.
- **Cross-Platform Compatibility:** Python runs on various operating systems, including Windows, macOS, and Linux, making it highly portable.
- **Large and Active Community:** Python has a vast and active community, providing extensive documentation, tutorials, and third-party libraries.
- **Support for Multiple Programming Paradigms:** Python supports procedural, object-oriented, and functional programming paradigms.

#### Use Cases Where Python is Particularly Effective
- **Web Development:** Frameworks like Django and Flask make it easy to build robust and scalable web applications.
- **Data Science and Machine Learning:** Libraries like Pandas, NumPy, and Scikit-Learn are essential tools for data analysis and machine learning.
- **Scripting and Automation:** Python is often used for writing scripts to automate repetitive tasks.
- **Scientific Computing:** Libraries like SciPy and Matplotlib are widely used for scientific research and visualization.
- **Artificial Intelligence and Deep Learning:** Frameworks like TensorFlow and PyTorch enable the development of complex AI and deep learning models.
- **Game Development:** Libraries like Pygame make it possible to develop simple 2D games.

### 2. Installing Python:
#### Steps to Install Python on Windows
- Open your web browser and go to the official Python website (https://www.python.org/), then navigate to the `Downloads` section and download the latest Python version for Windows.
- When the download is done, on your local machine go to `file explorer` then `downloads` to locate the downloaded installer file then `double-click to run it`.
- A window will open, select `Customize installation` and proceed. Click on the `Add Path` check box, it will set the Python path automatically. (Ensure that the options for “Install for all users” and “Precompile standard library” are checked.)
- Click the `Install` button to begin the installation process. You may be prompted by User Account Control (UAC) to allow changes to your computer. Click `Yes` to proceed.

#### How to verify the installation and set up a virtual environment.
- On your local machune press `Win + R`, type `cmd`, and press Enter to open the Command Prompt then type `python --version`(You should see the installed Python version printed on the screen, e.g., Python 3.10.0.)
- Check if `pip` is installed by typing `pip --version` (You should see the version of pip printed on the screen, e.g., pip 21.1.2). if pip is not installed you can install it by typing `python get-pip.py`.

### 3. Python Syntax and Semantics:
  
Here is a simple Python program that prints "Hello, World!" to the console: `print("Hello, World!")`

#### Explanation of Basic Syntax Elements
1. Function Call: `print` This is a built-in Python function used to output text or other data to the console. Functions in Python are called by writing the function name followed by parentheses ().
2. String: `"Hello, World!"` This is a string, a sequence of characters enclosed in quotes. In Python, strings can be enclosed in single quotes (') or double quotes (").
3. Parentheses: `()` Parentheses are used to enclose the arguments passed to a function. In this case, "Hello, World!" is the argument passed to the print function.
4. Argument: `"Hello, World!"` inside the parentheses is the argument provided to the print function. The argument is what the function will process and output. 

### 4. Data Types and Variables:

Python has several basic data types that are used to store different kinds of data. Here are the primary ones:

1. Integers (int): Whole numbers, positive or negative, without a decimal point (e.g., 1, -34, 9999).
2. Floating-Point Numbers (float): Numbers that contain a decimal point (e.g., 3.14, -0.5, 2e6).
3. Strings (str): Sequences of characters enclosed in single, double, or triple quotes (e.g., "Hello", 'Python', "").
4. Booleans (bool): Logical values representing True or False .
5. Lists (list): Ordered collections of items, which can be of different data types (e.g., [1, 'two', 3.14]).
6. Tuples (tuple): Unchangeable ordered collections of elements (e.g., (1, 2, 'three')).
7. Dictionaries (dict): Unordered collections of key-value pairs (e.g., {'name': 'John', 'age': 30}).
8.NoneType (None): A special value indicating the absence of a value.
 
       # Create variables of different data types:
       num = 10  # int
       pi = 3.14  # float
       my_string = "This is a string"  # str
       numbers_list = [1, 2, 3, 4, 5]  # list
       fruit_tuple = ("apple", "banana", "orange")  # tuple
       student_dict = {"name": "Alex", "age": 21}  # dict
       is_raining = False  # bool
       nothing = None  # NoneType
               
       # Print the variables:
       print("Number:", num)
       print("Pi:", pi)
       print("String:", my_string)
       print("List:", numbers_list)
       print("Tuple:", fruit_tuple)
       print("Dictionary:", student_dict)
       print("Boolean:", is_raining)
       print("Nothing:", nothing)

### 5. Control Structures:
#### Conditional Statements
Conditional statements allow you to execute specific blocks of code based on whether a condition is true or false. The most common conditional statement is the `if-else` statement.
- **if condition:** code block to execute if condition is True.
- **else:** code block to execute if condition is False.

#### Example
           age = 18

         if age >= 18:
             print("You are an adult")
         else:
             print("You are not an adult")
#### Loops
Loops allow you to execute a block of code multiple times. The primary loop constructs in Python are `for`.
- **for item in iterable:** code block to execute for each item in the iterable.

#### Example
       numbers = [1, 2, 3, 4, 5]

     for number in numbers:
         print(number)

#### Combined Example
You can combine conditional statements and loops to create complex control flow.
    
    #Example combining if-else statement and for loop
      numbers = [1, 2, 3, 4, 5]
      
      for number in numbers:
          if number % 2 == 0:
              print(f"{number} is even.")
          else:
              print(f"{number} is odd.")

- **for Loop:** Iterates over the list numbers. For each iteration, the variable number takes the value of the current item in the sequence.
- **if-else Statement:** Checks if the current number is even by using the modulus operator %. If number % 2 == 0 is true, it prints that the number is even otherwise, it prints that the number is odd.

### 6. Functions in Python:
**Functions in Python** are blocks of reusable code that perform a specific task. They help in organizing code, making it more modular, readable, and easier to maintain. Functions also allow for code reuse, reducing redundancy.

#### Why Functions are Useful:
1. **Modularity:** Functions break down complex problems into smaller, manageable pieces.
2. **Code Reusability:** Once a function is defined, it can be used multiple times in a program, avoiding code duplication.
3. **Readability:** Functions make the code cleaner and more understandable.
4. **Maintainability:** Functions make it easier to update and maintain code, as changes can be made in one place rather than throughout the codebase.

Here’s how to define a simple function that takes two arguments and returns their sum and also how to call it:

        # Define the function
        def add_numbers(a, b):
            """
            This function takes two arguments a and b,
            and returns their sum.
            """
            return a + b
        
        # Call the function and print the result
        result = add_numbers(5, 7)
        print("The sum is:", result)  # Output: The sum is: 12

#### Function Definition:
- **def add_numbers(a, b):**`def` is used to define a function, `add_numbers` is the name of the function. `(a, b)` are the parameters of the function.
- **""" ... """:** This is a docstring that describes what the function does.
- **return a + b:** This statement returns the sum of a and b.

#### Function Call:
- **result = add_numbers(5, 7):** This line calls the add_numbers function with arguments 5 and 7. The function returns the sum, which is assigned to the variable result.
- **print("The sum is:", result):** This line prints the result to the console.

### 7. Lists and Dictionaries:
#### Differences Between Lists and Dictionaries in Python
####Lists
- Ordered sequence of elements of any data type.
- Elements indexed by their position in the list.
- Defined using square brackets `[]`.
- Access elements by index.
- Supports operations like addition, deletion, insertion, concatenation.
- Mutable, can be modified after creation.

####Dictionaries
- Unordered collection of key-value pairs.
- Keys must be unique and immutable, can be of any data type.
- Defined using `curly braces {}` with key-value pairs separated by a `colon :`.
- Access elements by key.
- Values can be of any data type.
- Supports operations like adding, deleting, updating key-value pairs.
- Mutable, can be modified after creation.

#### Script Demonstrating Basic Operations on Lists and Dictionaries

      # Create a list of numbers
      my_list = [1, 2, 3, 4, 5]
      
      # Create a dictionary with key-value pairs
      my_dict = {'name': 'John', 'age': 30, 'city': 'New York'}
      
      # Print the list
      print("List:", my_list)
      
      # Print the dictionary
      print("Dictionary:", my_dict)
      
      # Add an element to the list
      my_list.append(6)
      
      # Add a key-value pair to the dictionary
      my_dict['state'] = 'California'
      
      # Print the updated list
      print("Updated List:", my_list)
      
      # Print the updated dictionary
      print("Updated Dictionary:", my_dict)
      
      # Access an element from the list using index
      print("First element in list:", my_list[0])
      
      # Access a value from the dictionary using key
      print("Name from dictionary:", my_dict['name'])
      
      # Remove an element from the list by index
      del my_list[2]
      
      # Remove a key-value pair from the dictionary using key
      del my_dict['city']
      
      # Print the final list
      print("Final List:", my_list)
      
      # Print the final dictionary
      print("Final Dictionary:", my_dict)

  #### Output
    List: [1, 2, 3, 4, 5]
    Dictionary: {'name': 'John', 'age': 30, 'city': 'New York'}
    Updated List: [1, 2, 3, 4, 5, 6]
    Updated Dictionary: {'name': 'John', 'age': 30, 'city': 'New York', 'state': 'California'}
    First element in list: 1
    Name from dictionary: John
    Final List: [1, 2, 4, 5, 6]
    Final Dictionary: {'name': 'John', 'age': 30, 'state': 'California'}

### 8. Exception Handling:
#### Exception Handling in Python
Exception handling in Python is a mechanism to handle runtime errors, ensuring that the program continues to execute even if an error occurs. It allows you to manage and respond to various error conditions gracefully without crashing the program.

#### Example of Using try, except, and finally
Here’s an example that demonstrates how to use try, except, and finally blocks to handle errors in a Python script:

      def divide_numbers(a, b):
    try:
        # Try to perform the division
        result = a / b
    except ZeroDivisionError as e:
        # Handle the case where division by zero occurs
        print("Error: Cannot divide by zero.")
        result = None
    except TypeError as e:
        # Handle the case where the input types are not numbers
        print("Error: Invalid input type. Both arguments must be numbers.")
        result = None
    finally:
        # This block will always be executed
        print("Execution of the try-except block is complete.")
    return result
    
    # Example usage of the function
    num1 = 10
    num2 = 0
    
    print(f"Dividing {num1} by {num2}...")
    result = divide_numbers(num1, num2)
    print("Result:", result)
    
    num1 = 10
    num2 = 2
    
    print(f"\nDividing {num1} by {num2}...")
    result = divide_numbers(num1, num2)
    print("Result:", result)
    
    num1 = 10
    num2 = "a"
    
    print(f"\nDividing {num1} by {num2}...")
    result = divide_numbers(num1, num2)
    print("Result:", result)

1. **Try Block:**
- Contains the code that might raise an exception
- Contains the code that attempts to divide a by b. This is where the potential exception might occur.
2. **Except ZeroDivisionError as e:**
- Contains the code that runs if an exception occurs in the try block.
- Catches the ZeroDivisionError if b is zero. Prints an error message and sets result to None.
**except TypeError as e:**
- Catches the TypeError if a or b are not numbers. Prints an error message and sets result to None.
3. **Finally Block:**
- Contains the code that runs no matter what, after the try and except blocks. This block is optional and is often used for cleanup actions.
- Executes regardless of whether an exception occurred or not. Prints a completion message.

### 9. Modules and Packages:
#### Modules
A module in Python is a file containing Python definitions and statements. Modules allow you to organize your code into separate files, making it more manageable and reusable. Each Python file (.py) is a module.

#### Packages
A package is a collection of modules organized in directories that provide a hierarchical structure. Packages allow you to organize related modules together. A directory containing a special __init__.py file is considered a package. The __init__.py file can be empty or contain initialization code for the package.
   
#### Importing and Using a Module
- To use a module in your script, you need to import it. You can import a module using the import statement. Once imported, you can access the module’s functions, classes, and variables.
- Example Using the `math` Module: The `math` module is a built-in Python module that provides mathematical functions. To immport the `math module` we type `import math`.

#### Example Script
      import math
    
    # Calculate the square root of a number
    number = 16
    sqrt = math.sqrt(number)
    print(f"The square root of {number} is {sqrt}")
    
    # Calculate the sine of an angle in radians
    angle = math.pi / 2  # 90 degrees
    sine = math.sin(angle)
    print(f"The sine of {angle} radians is {sine}")
    
    # Calculate the power of a number
    base = 2
    exponent = 3
    power = math.pow(base, exponent)
    print(f"{base} raised to the power of {exponent} is {power}")
    
    # Use some constants from the math module
    pi = math.pi
    e = math.e
    print(f"The value of pi is {pi}")
    print(f"The value of e is {e}")

### 10. File I/O:
Python provides built-in functions to handle file operations such as reading from and writing to files. Here are the basic steps to perform these operations:

#### Reading from a File
To read from a file, you typically use the open() function to open the file in read mode ('r'). You can then use methods like read(), readline(), or readlines() to read the content.

    # Open the file in read mode
    with open('example.txt', 'r') as file:
        # Read the entire content of the file
        content = file.read()
    
    # Print the content to the console
    print(content)

#### Writing to a File
To write to a file, you open it in write mode ('w') or append mode ('a'). Write mode will overwrite the existing content, while append mode will add to the existing content.

    # List of strings to write to the file
    lines = [
        "Hello, World!",
        "This is a test file.",
        "Writing multiple lines to a file.",
        "Python makes file handling easy."
    ]
    # Open the file in write mode
    with open('output.txt', 'w') as file:
        # Write each string to the file
        for line in lines:
            file.write(line + '\n')  # Add a newline character after each string

