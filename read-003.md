# Read 03: FileIO & Exceptions:

## Read & Write Files in Python:

* **What Is a File?** : 
  - a file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable. In the end, these byte files are then translated into binary 1 and 0 for easier processing by the computer.
  - What this data represents depends on the format specification used, which is typically represented by an extension.

* **File Path**: is a string that represents the location of a file. It’s broken up into three major parts: **Folder Path** ,**File Name** and **Extension**.
* **Character Encodings** : An encoding is a *translation from byte data to human readable characters*. This is typically done by assigning a numerical value to represent a character. The two most common encodings are the **ASCII** and **UNICODE** Formats. ASCII can only store 128 characters, while Unicode can contain up to 1,114,112 characters.

* **Opening and Closing a File in Python** :
 - open file in python is done by invoking the **open()** built-in function. open() has a single required argument that is the path to the file. open() has a single return, the file object.

 - When you’re manipulating a file, there are two ways that you can use to ensure that a file is closed properly, even when encountering an error. The first way to close a file is to use the try-finally block:
  - Example:

```
reader = open('dog_breeds.txt')
try:
    # Further file processing goes here
finally:
    reader.close()
```

 - The second way to close a file is to use the with statement:

```
with open('dog_breeds.txt') as reader:
    # Further file processing goes here
```

 - The with statement automatically takes care of closing the file once it leaves the with block, even in cases of error.
 - You can use the second positional argument, **mode**. This argument is a string that contains multiple characters to represent how you want to open the file. The default and most common is 'r', which represents opening the file in read-only mode as a text file:

```
with open('dog_breeds.txt', 'r') as reader:
    # Further file processing goes here
```

  - **'r >> Open for reading (default)**
  - **'w'>> Open for writing, truncating (overwriting) the file first**
  - **'rb' or 'wb'>> Open in binary mode (read/write using byte data)**

* **Reading and Writing Opened Files**
 - There are multiple methods that can be called on a file object to help you out:
  + **.read(size=-1) >> This reads from the file based on the number of size bytes. If no argument is passed or None or -1 is passed, then the entire file is read.**
  + **.readline(size=-1) >> This reads at most size number of characters from the line. This continues to the end of the line and then wraps back around. If no argument is passed or None or -1 is passed, then the entire line (or rest of the line) is read.**
  + **.readlines() >> This reads the remaining lines from the file object and returns them as a list.**
 - A common thing to do while reading a file is to iterate over each line by use the Python .readline() method to perform that iteration.
 - Write methods :
  + **.write(string) >> This writes the string to the file.**
  + **.writelines(seq) >> This writes the sequence to the file. No line endings are appended to each sequence item. It’s up to you to add the appropriate line ending(s).**

* **Tips and Tricks**:
  * __file__ : The __file__ attribute is a special attribute of modules, similar to __name__. It is: “the pathname of the file from which the module was loaded, if it was loaded from a file.” 

--------------------------------------------------------------------

## Python Exceptions: 

* In Python, an error can be a **syntax error** or an **exception**
* **Syntax errors** occur when the parser detects an incorrect statement.
* **exception error** occurs whenever syntactically correct Python code results in an error.
* If you want to throw an error when a certain condition occurs using **raise**, you could go about it like this:

```
x = 10
if x > 5:
    raise Exception('x should not exceed 5. The value of x was: {}'.format(x))
```

1. **The AssertionError Exception**:If the condition of assert turns out to be False
2. **The try and except Block: Handling Exceptions**: The try and except block in Python is used to catch and handle exceptions. Python executes code following the try statement as a “normal” part of the program. The code that follows the except statement is the program’s response to any exceptions in the preceding try clause.
3. **The else Clause** :In Python, using the else statement, you can instruct a program to execute a certain block of code only in the absence of exceptions.

*  **finally** enables you to execute sections of code that should always run, with or without any previously encountered exceptions.
