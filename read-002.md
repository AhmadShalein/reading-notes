# Read 02: Testing and Modules:

## In Tests We Trust - TDD with Python:

Unit tests are some pieces of code to exercise the input, the output and the behaviour of your code. You can write them anytime you want. But Test-Driven Development is a strategy to think (and write!) tests first.

The API is pretty straightforward and your work was almost done. But with TDD we need to think about tests first.

- unit tests are pieces of code to exercise input, output, and behavior of code.

```
- test-driven development is a way to write tests first

- this makes it more dynamic for code to run.
```

- when creating tests we should separate them from module.

- Other thing to care about is the structure. A convention widely used is the AAA : Arrange, Act and Assert.

**Arrange**: you need to organize the data needed to execute that piece of code (input).
**Act**: here you will execute the code being tested (exercise the behaviour).
**Assert**: after executing the code, you will check if the result (output) is the same as you were expecting.

--------------------------------------------------------------------

## Recursion:

**What is Recursion?**

- The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called as recursive function. Using recursive algorithm, certain problems can be solved quite easily. Examples of such problems are Towers of Hanoi (TOH), Inorder/Preorder/Postorder Tree Traversals, DFS of Graph, etc.

```
 f(n) = 1 + 2 + 3..... + n
 approach 2 - Recursive adding

 f(n) = 1     n = 1
 f(n) = n + f(n-1) n>1
```

**What is base condition in recursion?**

- In the recursive program, the solution to the base case is provided and the solution of the bigger problem is expressed in terms of smaller problems.

**What are the disadvantages of recursive programming over iterative programming?**

- both recursive and iterative programs have the same problem-solving powers, i.e., every recursive program can be written iteratively and vice versa is also true. The recursive program has greater space requirements than iterative program as all functions will remain in the stack until the base case is reached. It also has greater time requirements because of function calls and returns overhead.

--------------------------------------------------------------------

## Python Lists:

- Lists are used to store multiple items in a single variable.

- Lists are one of 4 built-in data types in Python used to store collections of data, the other 3 are Tuple, Set, and Dictionary, all with different qualities and usage.
 
- Lists are created using square brackets.
