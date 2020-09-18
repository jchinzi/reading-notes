### Hash Tables

Hash(key) --> index

To store a value: append key and value to the end of the linked list at that index position.

To read a value: access the linked list at that index position and search for the node with the matching key.  Then return that key/value pair.

---

*Terms:*

- Hash: the result of some algorithm taking an incoming string and converting it into a value that could be used (in this case) to determine the index of the array.  Using a hash to determine an index means that we are able to reverse the process and look up the index of the key using the hash in O(1) time.

    Ex. of Steps to Create a Hash:
    1.  Add or multiply all the ASCII values together.
    1.  Multiply it by a prime number such as 599.
    1.  Use modulo to get the remainder of the result, when divided by the total size of the array.
    1.  Insert into the array at that index.

- Buckets: contained in each index of the array of the hashtable.  Each index must be a bucket so that multiple key/value pairs can be contained in the case of a collision.  To implement this, each index in the array is an initialization of a LinkedList rather than a null index value.

- Collision: when two or more keys get hashed to the same index in the same hashtable

---

*Common Uses:*

- Unique values
- Dictionary
- Library

---

*Reference:*

[Code Fellows - Hashtables](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)
[Hacker Earth - Basics of Hash Tables](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)
[Paul Programming - Into to Hash Tables (video)](https://www.youtube.com/watch?v=MfhjkfocRR0&ab_channel=PaulProgramming)

---

[Home](https://jchinzi.github.io/reading-notes/)