# Read 11: Data Analysis:

## What is Jupyter Lab?

* **JupyterLab** is an open-source web application primarily designed to provide a user interface based on Jupyter Notebook.It enables you to work with documents and activities such as Jupyter notebooks, text editors, terminals, and custom components in a flexible, integrated, and extensible manner.

* You can arrange multiple documents and activities side by side in the work area using tabs and splitters. Documents and activities integrate with each other, enabling new workflows for interactive computing, such as:

  * Code Consoles provide transient scratchpads for running code interactively, with full support for rich output. A code console can be linked to a notebook kernel as a computation log from the notebook.
  
  * Kernel-backed documents enable code in any text file (Markdown, Python, R, LaTeX, etc.) to be run interactively in any Jupyter kernel.
  
  * Notebook cell outputs can be mirrored into their own tab, side by side with the notebook, enabling simple dashboards with interactive controls backed by a kernel.
  
  * Multiple views of documents with different editors or viewers enable live editing of documents reflected in other viewers. For example, it is easy to have live preview of Markdown, Delimiter-separated Values, or Vega/Vega-Lite documents.
  
*  **JupyterLab** will eventually replace the classic Jupyter Notebook. Throughout this transition, the same notebook document format will be supported by both the classic Notebook and JupyterLab.

--------------------------------------------------------------------

## Numpy Tutorial:

* **NumPy** is the fundamental package for array computing with Python.

* With **NumPy**, we work with multidimensional arrays.In n a NumPy array, the number of dimensions is called the rank, and each dimension is called an axis.

* We can create a **NumPy** array using the **numpy.array** function.

* One of the limitations of NumPy is that all the elements in an array have to be of the same type.
  
* We can check the number of rows and columns in our data using the shape property of NumPy arrays.
  
* We can create an array where every element is zero using numpy.zeros.

* We can create an array where each element is a random number using numpy.random.rand.

* NumPy is zero-indexed, meaning that the index of the first row is 0, and the index of the first column is 0.

* (:). A colon indicates that we want to select all the elements from the starting index up to but not including the ending index.
