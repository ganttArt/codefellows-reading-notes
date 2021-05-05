# Trees

[Link to Reading](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)

## Common Terminology

- **Node** - A Tree node is a component which may contain it’s own values, and references to other nodes
- **Root** - The root is the node at the beginning of the tree
- **K** - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.
- **Left** - A reference to one child node, in a binary tree
- **Right** - A reference to the other child node, in a binary tree
- **Edge** - The edge in a tree is the link between a parent and child node
- **Leaf** - A leaf is a node that does not have any children
- **Height** - The height of a tree is the number of edges from the root to the furthest leaf

## Traversals

### Depth First

- Pre-order: root >> left >> right
- In-order: left >> root >> right
- Post-order: left >> right >> root

### Breadth First

- Breadth first traversal iterates through the tree by going through each level of the tree node-by-node.

## Binary Tree Vs K-ary Trees vs Binary Search Trees

- **K-ary Trees** - If Nodes are able have more than 2 child nodes, we call the tree that contains them a K-ary Tree. In this type of tree we use K to refer to the maximum number of children that each Node is able to have.
- Binary Trees have at most two child nodes
- **BST** - A Binary Search Tree (BST) is a type of tree that does have some structure attached to it. In a BST, nodes are organized in a manner where all values that are smaller than the root are placed to the left, and all values that are larger than the root are placed to the right.
