name: inverse
layout: true
class: center, middle, inverse
---
# Intro to Scientific Python

---
layout: false

### <span style="color:purple">Python packages</span>


You can install individual Python packages using:

- Python Package Index (PyPI): `pip install`
- Conda 

--

You can also use a Python distribution for scientific computing:

- Anaconda


---
### <span style="color:purple">Python packages</span>

More about PyPI and Conda/Anaconda:

- PyPI:
    - package manager for the Python language
    - might require compatible compilers (not as big issue as it used to be)
    

- Conda:
    - package manager (not only for Python)
    - environment manager
    - compilers are never needed (using already compiled form, i.e. binaries)
    - provide dependency checks: ensures that the environment will work properly
 
--

Installing Python packages used to be hard (especially on Windows), 
but this has been improved a lot! 

In most cases you will not have any issues installing packages, 
but to be safe - use project specific environments (will be discussed later)

---
### <span style="color:purple">Conda and Anaconda</span>


- Anaconda
    - distribution of the Python and R programming languages for 
    scientific computing (data science, machine learning)
    - includes more than 1500 popular data-science packages
    - manage libraries, dependencies, and environments with Conda
    - includes Anaconda Navigator - a desktop graphical user interface
    (GUI; Jupyter Notebook, Spyder and other application available)
    
--

In order to use Conda:
 
 - install [Miniconda](https://docs.conda.io/en/latest/miniconda.html): a free minimal installer for conda


In order to have the Anaconda full distribution:

- install [Anaconda](https://www.anaconda.com/distribution/) 
- could be also installed from Miniconda


---
   
### <span style="color:purple">Creating and using Conda environments</span>

Why do we use conda (or python) environments?

- to avoid conflicts in libraries required in different projects

- to be safe when creating a new environment (so we don't break the working one)


--

Creating a conda environment

```
conda create -n project_name python=3.7
```

Activating existing conda environment

```
conda activate project_name
```

Checking the existing conda environments

```
conda info --envs
```

Installing python packages

```
conda install numpy jupyter
```

Deactivating conda environment
```
conda deactivate
```

---

### <span style="color:purple">Jupyter notebook</span>

- What is a notebook document?
    
    - contains both computer code (e.g. python, R) 
    and rich text elements (paragraph, equations, figures, links, etc…)
    - is a human-readable documents containing the analysis description 
    and the results (figures, tables, etc..) 
    - is an executable documents which can be run to perform data analysis

--

- What is a Jupyter Notebook app

    -  application that allows editing 
    and running notebook documents via a web browser
    - requires a kernel (i.e. "computational engine") to execute
     the code from a notebook (ipython used to execute Python code)
    - can be executed on a local desktop (no internet access required)
    - or can be installed on a remote server (accessed through the internet)
    
---
   
### <span style="color:purple">Jupyter notebook</span>

Let's open a jupyter notebook on your local browser:

```python
jupyter notebook
```
If jupyter is installed, this should automatically open the application 
in your local browser.

If not, use the remote resources:
https://jupyter.org/try

--

There are three types of "cells":

- code cell: for computational code
- markdown cell: for a nicely formatted report (text, equations, etc.)
- raw cell: for raw form text

---
 
### <span style="color:purple">Jupyter notebook</span>

Let's explore the jupyter notebook and review the last class

1. create a list of integers from 0 to 9 (use `range`)
2. print all even numbers from 0 to 9
3. create a new list that contains the second power of all elements 
of the list
4. use list comprehension for creating the new list
5. import `math` library and review available functions
6. use `!` to run a simple shell command
7. use `%timeit` to time the execution

notes from the class: 
https://github.com/djarecka/scientific_python_intro_tutorial/blob/master/week2.ipynb

--

you can find more:

 - https://github.com/ipython/ipython-in-depth
 - https://blog.dominodatalab.com/lesser-known-ways-of-using-notebooks/
 
---
### <span style="color:purple">NumPy</span>

- a general-purpose array-processing package
- provides a high-performance multidimensional array objects 
and tools for working with these arrays
- the fundamental package for scientific computing with Python

--

We will follow the scipy-lectures to learn about NumPy:

https://scipy-lectures.org/intro/numpy/array_object.html


