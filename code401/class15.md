# Trees


> Node - A Tree node is a component which may contain it’s own values, and references to other nodes
> Root - The root is the node at the beginning of the tree
> K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.
> Left - A reference to one child node, in a binary tree
> Right - A reference to the other child node, in a binary tree
> Edge - The edge in a tree is the link between a parent and child node
> Leaf - A leaf is a node that does not have any children
> Height - The height of a tree is the number of edges from the root to the furthest leaf


## Depth First

**where we prioritize going through the depth (height) of the tree first.**

Three methods for depth first traversal:


* **Pre-order: root >> left >> right.**

Pre-order means that the root has to be looked at first. In our case, looking at the root just means that we output its value. When we call preOrder for the first time, the root will be added to the call stack

* **In-order: left >> root >> right**
* **Post-order: left >> right >> root**

## Breadth First

> Breadth first traversal iterates through the tree by going through each level of the tree node-by-node. So, given our starting tree one more time.
> breadth first traversal uses a queue (instead of the call stack via recursion) to traverse the width/breadth of the tree. 

## Adding a node

> use of breadth first traversal. During the traversal, we find the first node that does not have all it’s children filled, and insert the new node as a child. We fill the child slots from left to right.

> In the event you would like to have a node placed in a specific location, you need to reference both the new node to create, and the parent node upon which the child is attached to.

## Big O

* Searching for a specific node will be O(n).
* The Big O space complexity for a node insertion using breadth first insertion will be O(w), where w is the largest width of the tree. For example, in the above tree, w is 4.
* The maximum width for a perfect binary tree, is 2^(h-1), where h is the height of the tree. 

# Binary Search Trees

A Binary Search Tree (BST) is a type of tree that does have some structure attached to it. In a BST, nodes are organized in a manner where all values that are smaller than the root are placed to the left, and all values that are larger than the root are placed to the right.

