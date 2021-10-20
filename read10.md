# Stacks and Queues

![Stacks and Queues](https://www.atechdaily.com/resources/images/posts/2020/3/130/stackvsqueue.png)

## What is a Stack

A stack is  linear data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.

### Common terminology for a stack is

1. Push: Nodes or items that are put into the stack are pushed
2. Pop: Nodes or items that are removed from the stack are popped. When you attempt to pop an empty stack an exception will be raised.
3. Top: The top of the stack.
4. Peek: When you peek you will view the value of the top Node in the stack. When you attempt to peek an empty stack an exception will be raised.
5. IsEmpty: returns true when stack is empty otherwise returns false.

### Stacks follow these concepts

* FILO
First In Last Out

* LIFO
Last In First Out

## What is a Queue

A queue is a lot like a stack. It is a linear structure (FIFO) order, but they differ in how elements are removed. Queues are open from both ends

### Common terminology for a queue is

1. Enqueue - Nodes or items that are added to the queue.
2. Dequeue - Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.
3. Front - This is the front/first Node of the queue.
4. Rear - This is the rear/last Node of the queue.
5. Peek - When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.
6. IsEmpty - returns true when queue is empty otherwise returns false.
Queues follow these concepts:

* FIFO
First In First Out
* LILO
Last In Last Out

### Types of Queues

1. Circular Queue:the last element is connected to the first element to form a circle.

2. Priority Queue: elements are sorted based on priority.

## resources used in this reading

1. [Stacks](https://www.educative.io/blog/data-structures-stack-queue-java-tutorial#stack)
2. [Stacks and Queues](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/stacks_and_queues.html)
