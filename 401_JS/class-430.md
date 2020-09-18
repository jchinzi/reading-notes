### Hash Tables

Hash(key) --> index

*Terms:*

- Hash: the result of some algorithm taking an incoming string and converting it into a value that could be used (in this case) to determine the index of the array.  Using a hash to determine an index means that we are able to reverse the process and look up the index of the key using the hash in O(1) time.

- Buckets: contained in each index of the array of the hashtable.  Each index must be a bucket so that multiple key/value pairs can be contained in the case of a collision.  To implement this, each index in the array is an initialization of a LinkedList rather than a null index value.

- Collision: when two or more keys get hashed to the same index in the same hashtable

*Common Uses:*

- Unique values
- Dictionary
- Library



---

[Home](https://jchinzi.github.io/reading-notes/)