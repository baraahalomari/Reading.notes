# Linked Lists

> List is a sequence of Nodes that are connected/linked to each other. The most defining feature of a Linked List is that each Node references the next Node in the link.

* **Linked List**: A data structure that contains nodes that links/points to the next node in the list.
* **Singly**: refers to the number of references the node has. 
* **Doubly**: refers to there being two (double) references within the node.
* **Node**:  individual items/links that live in a linked list.
* **Next**:  This property contains the reference to the next node.
* **Head**:  is a reference of type Node to the first node in a linked list.
* **Current** : Current is a reference of type Node to the node that is currently being looked at. 

> we are not able to use a foreach or for loop. The best way to approach a traversal is through the use of a while() loop. 

> If we accidentally end up trying to traverse on a node that is null, a NullReferenceException gets thrown and our program will crash/end.

## what exactly is happening through an example:

* creating Current at the Head.
* We create a while loop. 
* checking if the value of the current node is equal to the value we are looking for.
* If the Current node does not contain the value we are looking for, we then must move Current to the next node that is being referenced. 
* Once we hit the end, we know that we did not find the value and return true at any point, so the value is not in the LinkedList. We return false.

## Traversal Big O

The Big O of time for Includes would be O(n). This is because, at its worse case, the node we are looking for will be the very last node in the linked list. 

> The Big O of space for Includes would be O(1). This is because there is no additional space being used than what is already given to us with the linked list input.

## Adding a Node

* If we want to add a node with an O(1) efficiency, we have to replace the current Head of the linked list with the new node, without losing the reference to the next node in the list.

ALGORITHM Add(newValue)

// INPUT <-- Value to add

// OUTPUT <-- No output

  newNode <-- NEW Node

  newNode.Value <-- newValue

  newNode.Next <-- Head

  Head <-- newNode

* Adding a node to the middle of a linked list is a bit different than adding to the beginning. This is because we are working with more nodes and must re-allocate to make room for the new node.

ALGORITHM AddBefore(newValue, valueToAddBefore)

// INPUT <-- New value, Value to add before

// OUTPUT <-- boolean

  Current <-- Head
  
  IF Current is equal to NULL

    return FALSE


  WHILE Current.Next is not equal to NULL

    IF Current.Next.Value is equal to valueToAddBefore

      newNode <-- NEW Node

      newNode.Value <-- newValue

      newNode.Next <-- Current.Next

      Current.Next <-- newNode

      return TRUE


    Current <-- Current.Next;


  return FALSE

# What’s a Linked List, Anyway pt1

## Linear data structures

> There is a sequence and an order to how they are constructed and traversed.

In non-linear data structures, items don’t have to be arranged in order, which means that we could traverse the data structure non-sequentially.

> Trees and graphs are also non-linear data structures that we traverse in different ways.

>  Just as characters, numbers, words, sentences require bytes of memory to represent them, so do data structures.

The fundamental difference between arrays and linked lists is that arrays are static data structures, while linked lists are dynamic data structures. A static data structure needs all of its resources to be allocated when the structure is created; this means that even if the structure was to grow or shrink in size and elements were to be added or removed, it still always needs a given size and amount of memory. If more elements needed to be added to a static data structure and it didn’t have enough memory, you’d need to copy the data of that array, for example, and recreate it with more memory, so that you could add elements to it.


## Parts of a linked list

The starting point of the list is a reference to the first node, which is referred to as the head. Nearly all linked lists must have a head, because this is effectively the only entry point to the list and all of its elements, and without it, you wouldn’t know where to start! The end of the list isn’t a node, but rather a node that points to null, or an empty value.

> A node only knows about what data it contains, and who its neighbor is.

## Lists for all shapes and sizes

Singly linked lists are the simplest type of linked list, based solely on the fact that they only go in one direction. There is a single track that we can traverse the list in; we start at the head node, and traverse from the root until the last node, which will end at an empty null value.

# What’s a Linked List, Anyway pt2 

## Big O (Links to an external site.)

* major points to consider for algorithms: how much time it requires at runtime given how much time and memory it needs
> amount of time it takes for an action to run based on the amount of elements we pass into it (n)

* O(1) -> constant
* O(n) function -> linear
* O(n^2) -> just avoid this if you can

## Growing a linked list (Links to an external site.)

* expand linked lists by rearranging the next and previous pointers
* inserting at the head:

> start with the head node
> make new node and set its next to previous head node
> set new node as the head
> inserting at the beginning is good because it takes the same amount of time to process no matter how long the list is
* inserting at the tail:
> find the last node (where tail === null)
> create new node
> set the pointer to null
> direct preceding node to our new node
> is bad if we have a big list because we have to traverse from the head all the way to the tail. in order. no skipping







