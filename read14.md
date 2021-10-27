# Trees

## Binary Trees, Binary Search Trees, and K-ary Trees

![Trees](https://i.stack.imgur.com/5kJXf.gif)

## Important Terminology

1. Node - A Tree node is a component which may contain it’s own values, and references to other nodes
2. Root - The root is the node at the beginning of the tree
3. K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.
4. Left - A reference to one child node, in a binary tree
5. Right - A reference to the other child node, in a binary tree
6. Edge - The edge in a tree is the link between a parent and child node
7. Leaf - A leaf is a node that does not have any children
8. Height - The height of a tree is the number of edges from the root to the furthest leaf

## Traversals

Allow us to search about a node and print a content of tree,there are categories of traversals:

### Depth First

Where we prioritize going through the depth (height) of the tree first. There are multiple ways to carry out depth first traversal, and each method changes the order in which we search/print the root

* Pre-order: root >> left >> right
* In-order: left >> root >> right
* Post-order: left >> right >> root

### Breadth First

Going through tree node by node it uses a queue

## Binary Tree

Binary Trees restrict the number of children to two (hence our left and right children).
there is no certain sorting in binary trees,the nodes can be added any where space allows.

## K-ary Trees

In k-ary trees the Nodes are able have more than 2 child nodes and Traversing a K-ary tree requires a similar approach to the breadth first traversal.

## Binary Search Trees

In this type nodes are arranged in that are smaller than the root are placed to the left, and all values that are larger than the root are placed to the right.

## Big-O

The Big O time complexity of a Binary Search Tree’s insertion and search operations is O(h), or O(height).

## Resources used in this reading

1. [Trees](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)
