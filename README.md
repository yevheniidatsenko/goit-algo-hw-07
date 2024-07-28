# Trees and balancing

This repository contains an implementation of an AVL tree with functionalities to insert nodes, find the minimum and maximum values, and calculate the sum of all values in the tree.

## Description

An AVL tree is a self-balancing binary search tree where the difference between the heights of left and right subtrees cannot be more than one for all nodes. This implementation includes:

1. Inserting nodes into the AVL tree.
2. Finding the minimum value in the AVL tree.
3. Finding the maximum value in the AVL tree.
4. Calculating the sum of all values in the AVL tree.

## Tasks

### Task 1

Write an algorithm (function) that finds the maximum value in a binary search tree or AVL tree. Use any tree implementation from your notes or another source.

### Task 2

Write an algorithm (function) that finds the minimum value in a binary search tree or AVL tree. Use any tree implementation from your notes or another source.

### Task 3

Write an algorithm (function) that finds the sum of all values in a binary search tree or AVL tree. Use any tree implementation from your notes or another source.

## Usage

### Inserting Nodes

The `insert` method is used to insert nodes into the AVL tree. It ensures that the tree remains balanced after each insertion.

### Finding the Minimum Value

The `get_min_value_node` method is used to find the node with the minimum value in the AVL tree.

### Finding the Maximum Value

The `get_max_value_node` method is used to find the node with the maximum value in the AVL tree.

### Calculating the Sum of All Values

The `get_sum_values` method calculates the sum of all values stored in the AVL tree.

## Example

Here is an example of how to use the AVL tree implementation:

```python
if __name__ == "__main__":
    tree = AVLTree()
    root = None
    values = [22, 5, -10, 31, 14, 28, 40, 32, 47]

    print("Inserting values into AVL tree:")
    for value in values:
        root = tree.insert(root, value)

    print("AVL Tree:")
    print(root)

    print("Minimum value in the tree:", tree.get_min_value_node(root).key)
    print("Maximum value in the tree:", tree.get_max_value_node(root).key)
    print("Sum of all values in the tree:", tree.get_sum_values(root))
```

### Output

Inserting values into AVL tree:
AVL Tree:
Root: 22
L--- 5
L--- -10
R--- 14
R--- 31
L--- 28
R--- 40
L--- 32
R--- 47

Minimum value in the tree: -10
Maximum value in the tree: 47
Sum of all values in the tree: 209
