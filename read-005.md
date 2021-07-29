# Read 05: Linked Lists:

## What is a Linked List?

* **A Linked List** is a sequence of **Nodes** that are connected/linked to each other. The most defining feature of a Linked List is that each Node references the next Node in the link. 

* There are two types of Linked List - **Singly** and **Doubly**:
- **Singly:** Singly refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the Next node in a linked list.

- **Doubly:** Doubly refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous node.

--------------------------------------------------------------------

## Linear data structures:
 If we really want to understand the basics of linked lists, it’s important that we talk about what type of data structure they are.
 One characteristic of linked lists is that they are linear data structures, which means that there is a sequence and an order to how they are constructed and traversed.
 Linear structures, however, are the opposite of non-linear structures. In non-linear data structures, items don’t have to be arranged in order, which means that we could traverse the data structure non-sequentially.

--------------------------------------------------------------------

## Big O:
 There are two major points to consider when thinking about how an algorithm performs: how much time it requires at runtime given how much time and memory it needs.
 One way to think about Big O notation is a way to express the amount of time that a function, action, or algorithm takes to run based on how many elements we pass to that function.
 
 * An O(1) function takes constant time, which is to say that it doesn’t matter how many elements we have, or how huge our input is: it’ll always take the same amount of time and memory to run our algorithm.
 * An O(n) function is linear, which means that as our input grows (from ten numbers, to ten thousand, to ten million), the space and time that we need to run that algorithm grows linearly.
 <br>
 For a little contrast, we can also compare these two functions to something starkly different: an O(n²) function, which clearly takes exponentially more time and memory the more elements that you have. It’s pretty safe to say that we want to avoid O(n²) algorithms, just from looking at that crazy red line! 
