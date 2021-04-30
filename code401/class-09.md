# Implementation: Stacks and Queues

[Link to reading](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/stacks_and_queues.html)

## Stack

### Terminology

- **Push** - Items that are put into the stack
- **Pop** - Nodes or items that are removed from the stack are popped.
- **Top** - This is the top of the stack.
- **Peek** - View the value of the top Node in the stack.
- **IsEmpty** - returns true when stack is empty otherwise returns false.

### Stacks are

- **First In Last Out:** the first item added in the stack will be the last item popped out of the stack.
- **Last In First Out:** the last item added to the stack will be the first item popped out of the stack.

### Implementation

- The implementation shown uses Nodes that have a value and a next. The next indicates the node below it in the stack. The node at the bottom of the stack will have a next of null.
- Using this implementation the methods of Pop, Peek and isEmpty in O(1) time complexity
- A common alternative implementation is to just use an array.

---

## Queue

### Terminology

- **Enqueue** - Nodes or items that are added to the queue.
- **Dequeue** - Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.
- **Front** - This is the front/first Node of the queue.
- **Rear** - This is the rear/last Node of the queue.
- **Peek** - When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.
- **IsEmpty** - returns true when queue is empty otherwise returns false.

### Queues are

- **First In First Out:** the first item in the queue will be the first item out of the queue.
- **Last In Last Out:** the last item in the queue will be the last item out of the queue.

### Implementation

- In this implementation, we again use Nodes with a value and a next. We need to keep track of both the Rear and the Front of the queue at all times. Because we always know these values, Enqueuing and Dequeuing is always O(1) time complexity.
- The Rear node has a next of null. The Front node has a next that points to the next node in the queue (the one that will be dequeued after the front node).
- Another popular implementation of a Queue is to use an array.
