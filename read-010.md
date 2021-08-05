# Read 10: Stacks and Queues:

## What is a Stack?

* Stack is a linear data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous. It follows a particular order in which the operations are performed.The order may be **LIFO(Last In First Out)** or **FILO(First In Last Out)**.

* Common terminology for a stack is:

  * **Push**: Nodes or items that are put into the stack are pushed.
  
  * **Pop**: Nodes or items that are removed from the stack are popped. When you attempt to pop an empty stack an exception will be raised.
  
  * **Top**: This is the top of the stack.
  
  * **Peek**: When you peek you will view the value of the top Node in the stack. When you attempt to peek an empty stack an exception will be raised.
  
  *  **IsEmpty**: Returns true when stack is empty otherwise returns false.

![Stack](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/stack1.PNG)

--------------------------------------------------------------------

## What is a Queue?

* A Queue is a linear structure which follows a particular order in which the operations are performed. The order is First In First Out (FIFO).

* The difference between stacks and queues is in removing. In a stack we remove the item the most recently added; in a queue, we remove the item the least recently added.

* Common terminology for a queue is:

  * **Enqueue**: Nodes or items that are added to the queue.
  
  * **Dequeue**: Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.
  
  * **Front**: This is the front/first Node of the queue.
  
  * **Rear**: This is the rear/last Node of the queue.
  
  * **Peek**: When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.
  
  * **IsEmpty**: returns true when queue is empty otherwise returns false.

![Queue](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/Queue.PNG)
