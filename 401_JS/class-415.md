# Trees

## Key Terms

* **Node**: the individual item/data that makes up the data structure
* **Root**: the first/top *node* in the tree
* **Left Child**: *node* positioned to the left of a root or node
* **Right Child**:  *node* positioned to the right of a root or node
* **Edge**: the link between a parent and child *node*
* **Leaf**: *node* that does not contain any children
* **Height**: determined by the number of edges from the *root* to the bottommost *node*

## Traversals

* The most common way to traverse a tree is by using *recursion*, which relies on the *call stack* to navigate back up the tree after reaching the end of a sub-path

**Depth First**

*Pre-Order*: 
> root >> left >> right  

Pseudocode:
```
ALGORITHM preOrder(root)
// INPUT <-- root node
// OUTPUT <-- pre-order output of tree node's values

    OUTPUT <-- root.value

    if root.left is not Null
        preOrder(root.left)

    if root.right is not NULL
        preOrder(root.right)
```

*In-Order*: 
> left >> root >> right  

Pseudocode:
```
ALGORITHM inOrder(root)
// INPUT <-- root node
// OUTPUT <-- in-order output of tree node's values

    if root.left is not NULL
        inOrder(root.left)

    OUTPUT <-- root.value

    if root.right is not NULL
        inOrder(root.right)
```


*Post-Order*: 
> left >> right >> root  

Pseudocode:
```
ALGORITHM postOrder(root)
// INPUT <-- root node
// OUTPUT <-- post-order output of tree node's values

    if root.left is not NULL
        postOrder(root.left)

    if root.right is not NULL
        postOrder(root.right)

    OUTPUT <-- root.value
```

**Breadth First**

* Breadth First traversal usually uses a queue rather than the call stack via recursion

  - Beginning with the *root*, we can enqueue the root and then in dequeueing it we can use that root node in our code to enqueue the *left* and *right* child of it.

    -   Continuing in this fashion, as each node is dequeued we can enqueue that nodes children (if any) to continue digging deeper each round 

Pseudocode:
```
ALGORITHM breadthFirst(root)
// INPUT  <-- root node
// OUTPUT <-- front node of queue to console

  Queue breadth <-- new Queue()
  breadth.enqueue(root)

  while breadth.peek()
    node front = breadth.dequeue()
    OUTPUT <-- front.value

    if front.left is not NULL
      breadth.enqueue(front.left)

    if front.right is not NULL
      breadth.enqueue(front.right)
```

## Binary Trees

*   While *trees* can have any number of children per node, *binary trees* (as the name suggests) are limited to two children per node (a left and right child)

*   Beyond the two child limit, there is no formal structure to how nodes are organized in a binary tree
    -   One strategy for adding new nodes is to use *breadth first* traversal to find the first empty child slot and fill it.  This results in filling out the tree top down before adding a new layer of depth to the tree

**Big O**

*   Big O time complexity of inserting a new node or searching for a specific node is O(n), where n is the number of nodes in the tree

*   Big O space complexity for inserting a new node using breadth first insertion is O(w), where w is the largest width of the tree
    -   A 'perfect' tree then has a maximum width of 2^(h-1) where h is the tree height and can be calculated by log n (where n is the number of nodes)

## Binary Search Trees

*   BST is a type of tree that does have some structure attached to it
    -   Nodes are organized in a manner where all values *smaller* than the root are placed to the left and all values *larger* than the root are placed to the right
        -   Organizing a tree this way makes it more efficient to search later

**Big O**

*   Big O time complexity of searching for a specific node in a BST is O(), where h is the height of the tree
    -   Height could be anywhere between log(n) (in the case of a perfectly balanced tree) to n (in an entirely one sided tree)

*   Big O space complexity for a BST search is O(1) - searches require no additional space

## Reference Link:

[Trees](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)


---

[Home](https://jchinzi.github.io/reading-notes/)