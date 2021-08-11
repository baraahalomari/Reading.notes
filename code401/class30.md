# Hash Tables

> Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. 

> Buckets - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.

> Collisions - A collision is what happens when more than one key gets hashed to the same location of the hashtable.

### Uses :

* Hold unique values  * Dictionary  * Library


> Hashtables are a data structure that utilize key value pairs. This means every Node or Bucket has both a key, and a value.

### Creating a Hash :

* Add or multiply all the ASCII values together.
* Multiply it by a prime number such as 599.
* Use modulo to get the remainder of the result, when divided by the total size of the array.
* Insert into the array at that index.

## Collisions 

* Collision occurs when more than one key hashes to the same index in an array.
* Changing the initial state of the buckets.
Instead of starting them all as null we can initialize a LinkedList in each one.
* Now if two keys resolve to the same index in the array then their key/value pairs can be stored as a node in a linked list.
* Since different keys can lead to the same bucket it’s important to store the entire key/value pair in the bucket, not just the value.


### It is important to have a good hash function with the following basic requirements:
* Easy to compute.
* Uniform distribution.
* Less collisions.

## Internal Methods :

* Add() : When adding a new key/value pair to a hashtable.
* Find() : “The Find takes in a key, gets the Hash, and goes to the index location specified. Once at the index location is found in the array, it is then the responsibility of the algorithm the iterate through the bucket and see if the key exists and return the value”.
* Contains() : “The Contains method will accept a key, and return a bool on if that key exists inside the hashtable. The best way to do this is to have the contains call the GetHash and check the hashtable if the key exists in the table given the index returned”.
* GetHash() : “The GetHash will accept a key as a string, conduct the hash, and then return the index of the array where the key/value should be placed”.

# basics of hash tables

> Hashing is a technique that is used to uniquely identify a specific object from a group of similar objects.

* In hashing, large keys are converted into small keys by using hash functions. The values are then stored in a data structure called hash table.
* The idea of hashing is to distribute entries (key/value pairs) uniformly across an array. 
* Each element is assigned a key (converted key). By using that key you can access the element in O(1) time. 
* Using the key, the algorithm (hash function) computes an index that suggests where an entry can be found or inserted.

## Hash function

> A hash function is any function that can be used to map a data set of an arbitrary size to a data set of a fixed size, which falls into the hash table.
>  The values returned by a hash function are called hash values, hash codes, hash sums, or simply hashes.

### Basic requirements:

* Easy to compute: It should be easy to compute and must not become an algorithm in itself.

* Uniform distribution: It should provide a uniform distribution across the hash table and should not result in clustering.

* Less collisions: Collisions occur when pairs of elements are mapped to the same hash value. These should be avoided.

### Linear probing (open addressing or closed hashing)
> In open addressing, instead of in linked lists, all entry records are stored in the array itself. When a new entry has to be inserted, the hash index of the hashed value is computed and then the array is examined (starting with the hashed index). If the slot at the hashed index is unoccupied, then the entry record is inserted in slot at the hashed index else it proceeds in some probe sequence until it finds an unoccupied slot.

> Linear probing is when the interval between successive probes is fixed (usually to 1). Let’s assume that the hashed index for a particular entry is index.

### Quadratic Probing

> Quadratic probing is similar to linear probing and the only difference is the interval between successive probes or entry slots. Here, when the slot at a hashed index for an entry record is already occupied, you must start traversing until you find an unoccupied slot. The interval between slots is computed by adding the successive value of an arbitrary polynomial in the original hashed index.

### Double hashing

> Double hashing is similar to linear probing and the only difference is the interval between successive probes. Here, the interval between probes is computed by using two hash functions.


