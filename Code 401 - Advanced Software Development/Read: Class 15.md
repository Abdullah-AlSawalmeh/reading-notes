# Trees 🌳🌲🎄

---

- A tree is a nonlinear data structure, compared to arrays, linked lists, stacks and queues which are linear data structures. A tree can be empty with no nodes or a tree is a structure consisting of one node called the root and zero or one or more subtrees.

- Common Terminology

1. Node - A node is the individual item/data that makes up the data structure
2. Root - The root is the first/top Node in the tree
3. Left Child - The node that is positioned to the left of a root or node
4. Right Child - The node that is positioned to the right of a root or node
5. Edge - The edge in a tree is the link between a parent and child node
6. Leaf - A leaf is a node that does not contain any children
7. Height - The height of a tree is determined by the number of edges from the root to the bottommost node.

![](https://miro.medium.com/max/677/1*Z89j_NoDx9HkFcPHy3rPZg.png)

## Depth First

- Depth first traversal is where we prioritize going through the depth (height) of the tree first. There are multiple ways to carry out depth first traversal, and each method changes the order in which we search/print the root. Here are three methods for depth first traversal:

- Pre-order: root >> left >> right
- In-order: left >> root >> right
- Post-order: left >> right >> root

## Binary Trees

In all of our examples, we’ve been using a Binary Tree. Trees can have any number of children per node, but Binary Trees restrict the number of children to two (hence our left and right children).

There is no specific sorting order for a binary tree. Nodes can be added into a binary tree wherever space allows. Here is what a binary tree looks like:

## Binary Search Trees

A Binary Search Tree (BST) is a type of tree that does have some structure attached to it. In a BST, nodes are organized in a manner where all values that are smaller than the root are placed to the left, and all values that are larger than the root are placed to the right.

Here is how we would change our Binary Tree example into a Binary Search Tree:

## Big O in Trees

- The Big O time complexity of a Binary Search Tree’s insertion and search operations is O(h), or O(height). In the worst case, we will have to search all the way down to a leaf, which will require searching through as many nodes as the tree is tall. In a balanced (or “perfect”) tree, the height of the tree is log(n). In an unbalanced tree, the worst case height of the tree is n.

<img src="https://static1.squarespace.com/static/506e28cee4b04973cff61716/t/5192688ce4b011d27a007c75/1368549518511/B+Tree+and+Binary+Tree+Data+Structures.jpg?format=1500w" width="700px" height="400px">
