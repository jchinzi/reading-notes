## [Stacks and Queues](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/stacks_and_queues.html)

**Stack:** A data structure that consists of nodes

  - *Push*: adding nodes to the top of the stack
    - O(1) -> Will always take the same amount to time no matter how many nodes are in the stack
    - Steps to Push:
      - Assign the designated node as the new *top* with a next value equal to the original *top*
  - *Pop*: removing a node from the stack 
    - Cannot be performed on an empty stack
    - O(1) -> Will always take the same amount to time no matter how many nodes are in the stack
    - Steps to Pop:
      - Create a temporary reference to hold the reference currently at *top*
      - Reassign *top* to top.next
      - Reassign the *next* property in our temporary reference to NULL
      - Return the value of the temporary reference
  - *Top*: the top of the stack
  - *Peek*: view the value of the top Node in the stack
    - Cannot be performed on an empty stack
    - O(1) -> Will always take the same amount to time no matter how many nodes are in the stack
    - Should be called after *IsEmpty* or wrapped in a try/catch block to avoid empty stack exceptions
  - *IsEmpty*: boolean
      - O(1) -> Will always take the same amount to time no matter how many nodes are in the stack
    - Returns **true** when stack is empty (if *top* = NULL)
    - Otherwise, returns **false**

*Concepts Followed by Stacks:*

* FILO (First In Last Out)

* LIFO (Last In First Out)

---

*Common Queue Terminology:*

- *Enqueue*: Nodes added to the queue
  - O(1) -> Will always take the same amount to time no matter how many nodes are in the queue
  - Steps to Enqueue a new Node:
    - Change the *next* property of the *rear* node to point at the new node we are adding
    - Reassign the *rear* reference to the new node
- *Dequeue*: Nodes removed from the queue
  - O(1) -> Will always take the same amount to time no matter how many nodes are in the queue
  - Steps to Dequeue the Front Node:
    - Create a temporary reference to hold the reference currently at *front*
    - Reassign *front* to front.next
    - Reassign the *next* property in our temporary reference to NULL
    - Return the value of the temporary reference
- *Front*: First node of the queue
- *Rear*: Last node of the queue
- *Peek*: View the value of the *front* node in the queue
  - Cannot be called on an empty queue
  - O(1) -> Will always take the same amount to time no matter how many nodes are in the queue
  - Should be called after *IsEmpty* or wrapped in a try/catch block to avoid empty stack exceptions
- *IsEmpty*: boolean
    - O(1) -> Will always take the same amount to time no matter how many nodes are in the queue
    - Returns **true** when queue is empty (if *front* = NULL)
    - Otherwise, returns **false**

*Concepts Followed by Stacks:*

* FIFO (First In First Out)

* LILO (Last In Last Out)


---

[Home](https://jchinzi.github.io/reading-notes/)