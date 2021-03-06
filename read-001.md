# Read 01: Topic:

## Pain and Suffering:

- Pain is a normal, built-in part of life on earth but what is avoidable, though, is suffering. All it takes is practice.

--------------------------------------------------------------------

## Beginners Guide to Big O:

**Big O notation:**

- is used in Computer Science to describe the performance or complexity of an algorithm. Big O specifically *describes the worst-case scenario*, and can be used to describe the execution time required or the space used (e.g. in memory or on disk) by an algorithm.

**Examples:**

1- **O(1) algorithm** describes an algorithm that will always execute in the same time (or space) regardless of the size of the input data set.
```
bool IsFirstElementNull(IList<String> elements)
{
    return elements[0] == null;
}
```
2- **O(N) algorithm** :describes an algorithm whose performance will grow **linearly** and in direct proportion to the size of the input data set.

```
bool ContainsValue(IEnumerable<string> elements, string value)
{
    foreach (var element in elements)
    {
        if (element == value) return true; 
    }     
    return false; 
}
```
3- **O(N²) algorithm** represents an algorithm whose performance is *directly proportional to the square of the size of the input data set*. This is common with algorithms that involve nested iterations over the data set. Deeper nested iterations will result in O(N³), O(N⁴) etc.

```
bool ContainsDuplicates(IList<string> elements)
{
    for (var outer = 0; outer < elements.Count; outer++) 
    {
        for (var inner = 0; inner < elements.Count; inner++) 
        { 
            // Don't compare with self 
            if (outer == inner) continue;             
            
            if (elements[outer] == elements[inner]) return true; 
        }
    }    
    return false;
}
```

4- **O(2^N) algorithm** denotes an algorithm whose growth doubles with each addition to the input data set. *The growth curve of an O(2^N) function is exponential* — starting off very shallow, then rising meteorically. An example of an O(2^N) function is the recursive calculation of Fibonacci numbers.

```
int Fibonacci(int number)
{
    if (number <= 1) return number;
       
    return Fibonacci(number - 2) + Fibonacci(number - 1); 
}
```
5- **O(log n) algorithm** :This notation means that the runtime complexity of your algorithm will be increased by one when the size of input data is doubled.

--------------------------------------------------------------------

## Facts and Myths about Names and Values:
* Names refer to Values and the assignment is making the name refer to that value.
* Many names can refer to one value
* Names are reassigned independently.
* Values live until no references .
* Assignment never copies data and changes are visible through all names.
* Mutable aliasing but Immutable values can't alias.
* Immutable values includes ints ,float ,strings,tuples.
* Changing ints : **rebinding** ,Changing a list :**mutating** .
* We can rebind lists like this : num=num+[7]
* We can't mutate an int because int is immutable .
* Mutable and Immutable are assigned the same so assignment is the same for all values but the aliasing can make it seem different .
* References can be more than just names like list elements,object attributes,dict values and keys,function arguments ,and anything in the left side of an assignment.
* for loops : 
```
for x in sequence:
    something(x)
```
* Names have no type and values have no scope

--------------------------------------------------------------------

## How to Setup an Awesome Python Environment for Data Science or Anything Else:

* Coding in Python is awesome due to the massive amount of freely available libraries, its readability, and the recently introduced type annotations. 
* **Pyenv** is a set of three tools , two of them are pyenv (used to install python) and pyenv-virtualenv (used to configure your global tools). 
* **Mypy** is a static type checker for python code, that finds errors before they appear.
* **Pre-commit** is a tool that executes checks before you commit code to your repository.
