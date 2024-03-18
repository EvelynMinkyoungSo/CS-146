Java Solution Approach

1. Utility Method for BST Validation:
A private static method `isBSTUtil` recursively traverses the tree, maintaining a range (left_limit, right_limit) for allowable node values at each point.
The root node starts with (Long.MIN_VALUE, Long.MAX_VALUE) to represent the infinite possible range of BST values.
   
2. Base Case:
If the current node is null, it implies a valid BST structure at this branch, returning true.
   
3. Validation Check:
For a non-null node, check if its value is within the range defined by left_limit and right_limit. If not, the tree is not a BST.
   
4. Recursive Calls:
The method calls itself for the left and right children of the current node, updating the limits accordingly.
For the left child, the right_limit becomes the current node's value, and for the right child, the left_limit is updated.

Tree Construction from Input
A method createTreeFromInput constructs the binary tree level by level from a string array of values. Special handling for "null" strings allows building a complete tree structure including empty branches.

Python Solution Approach

1. Utility Function for BST Validation:
Similar to the Java version, isBSTUtil function check if the tree rooted at the given node is a BST within specified limits.

2. Recursive Depth-First Search:
The logic for base case, validation, and recursive traversal is identical, adjusted for Python's syntax and data types (float('-inf') and float('inf') for representing infinite range).

3. Tree Construction from Input:
A more Pythonic construction method create_tree_from_input uses list comprehension for initial node creation and a reverse list to manage children assignment in a loop.
