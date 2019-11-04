name: inverse
layout: true
class: center, middle, inverse
---
# Intro to Scientific Python

---
layout: false
###<span style="color:purple">Who am I?</span>


- <span style="color:purple">Dorota Jarecka</span> 
   - John Gabrieli Lab (PI: Satra Ghosh)
   - PhD in Physics
   - Working on scientific software 
 
---

### <span style="color:purple">Who are you?</span>
 
 - What's your name and where you work?
 - Why do you want to learn Python?
 - Have you tried to learn Python before? Hod did it go? 
 - Do you have Python installed on your laptop (do you know the version)?
 - What is your operating system? 
  

---

### <span style="color:purple">Programming languages</span>

- There are multiple programming languages people are using, and they differ:
   - low-level vs high level
   - compiled vs interpreted
   - general-purpose vs domain-specific
   - static vs dynamic typing
   - open source vs closed source
   - different design philosophy
   
--    
but don't concentrate too much on these points...

---

### <span style="color:purple">Python language</span>
- Python is:
   - high level language (strong abstraction from the details of the computer)
   - interpreted (don't have to compile first)
   - general-purpose 
   - dynamically typed
   - free and open source software (code is available for everyone)
   - design philosophy: code readability
      

---

### <span style="color:purple">How to run Python</span>

- To execute Python code you can:
   
    - open a standard interactive session: type `python` in your terminal
    - open an interactive session with ipython (you have to install first): type `ipython` in your terminal
    - write the code in a file with `.py` extension using plain text editor
    (e.g. gedit, nano, vi, vim, emacs) and execute the code by running python 
    interpreter from the terminal - `python your_code.py`
    - using Integrated Development Environment (IDE, e.g. PyCharm, Spider, Atom): 
    IDE provides additional features such as code execution, code linting, testing and debugging
    - using jupyter notebook: a web-based interactive computational environment,
    can be used to create documents that contain live code, equations, visualizations and narrative text 
    
Today, you can use an online interpreter: 
https://www.onlinegdb.com/online_python_interpreter

---

### <span style="color:purple">Hello World in Python</span>
- A "Hello World" program
    - a computer program that outputs "Hello, World!"
    - one of the simplest programs possible in almost all computer languages
    - used to quickly compare syntax between various programming languages
    - you can find many comparisons: http://helloworldcollection.de/

- Python: 
    - focus on code readibilty
    -  avoid boilerplate code
    
    ```python
    print("Hello World")
    ```

---

### <span style="color:purple">Python: dynamically typed language</span>
-  statically typed
    - type of a variable is known at compile time
    - often it means that the type of each variable has to be specified
    by the programmer (e.g. `int a`, `long b` in `C`)
    
-  dynamically typed
    - the type is associated with run-time values
    - programmer do not have to specify types (e.g. `a = 1`, `b = 1.5`)
    
--

Let's try to type:
```python
a = 1
b = 1.5
sum = a + b
print(sum)
```

--

Now we can check the type:

```python
print("type of a is: ", type(a))
```

--
And what is the type of `sum`?

```python
print("type of sum is: ", type(sum))
```
---

### <span style="color:purple">Python: data types</span>
   
- int (integer)
    - e.g. `3`, `20000`
- float
    - system-defined precision
    - e.g. `2.4`, `2.`
- complex
    - real and imaginary parts
    - e.g. `2 + 3j`
- str (string)
    - a sequence of characters
    - e.g. `"Hello"`, `'Hi'`, `""" used for multiple lines """`
- bool
    - represents logical values
    - can be `True` or `False`
- NoneType
    - represents the absence of a value
    - `None`
---

### <span style="color:purple">Python: data structures</span>
   
- list
    - mutable
    - can contain mixed types
    - e.g. `[1, 10]`, `[1, "Hi", 3.3]`
    - 0-indexed, the first element is 0
    - accessing an element or elements: `a[0]`, `a[1:]`, `a[:2]` 

- tuple
    - immutable
    - can contain mixed types
    - e.g. `(1, 10)`, `(1, "Hi", 3.3)`
    - 0-indexed, the first element is 0
    - accessing an element or elements: `a[0]`, `a[1:]`, `a[:2]` 

- dict (dictionary)
    - mutable
    - a collection of (key, value) pairs
    - each possible key appears at most once
    - e.g. `{"name": "Dorota", "city": "Somerville"}`
    - accessing an element: `a["name"]`


---

### <span style="color:purple">Python: statements and control flow</span>

- `=` 
    - assignment 
    - e.g. `a=3`   
- `if` statement 
    - conditionally executes a block of code 
    - can be combined with  `else` and `elif`(i.e., else if)
- `for` statement 
    - iterates over an iterable object 
    - used e.g. with `list`, `tuple`
- `while` statement 
    - executes a block of code as long as its condition is true
- `def` statement 
    - defines a new function
-  `import` statement 
    - used to import modules/packages whose functions or variables can be used in the current program


---

### <span style="color:purple">Python packages</span>
   
- In order to do anything useful in Python we need to use additional packages:


- Python has two main types of packages:
    - belong to the standard library
    - do not belong to the standard library
    
--
    
- A popular packages from the standard library: 
    - `os`: functions for interacting with the operating system
    - `datetime`:  for manipulating dates and times
    - `math`: gives access to the underlying C library functions for floating point math
    - `random`: tools for making random selections
    - and many others...
    
-- 

- A popular packages NOT from the standard library: 
    - `numpy`: multidimensional array
    - `scipy`: many scientific tools for linear algebra, optimization, integration, ...
    - `pandas`: data structures and data analysis tools; support for data frames
    - `matplotlib`, `seaborn`: visualization
    - and many others...

--

Let's practice using the standard library

 
