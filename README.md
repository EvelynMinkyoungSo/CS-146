Lab 4 (Binary Tree Inversion Solution)

//Java Solution Approach
1. A recursive function invertTree(TreeNode root), inverts the tree.
This function checks if the if the current node is null.
If not, it swaps the left and right children of the node.
2. Uses a queue to perform level-order traversal and print the tree.
This is done to verify the correct inversion of the tree.

##Python Solution Approach
1. A recursive function, invertTree(self, root), within a class Solution.
It inverts the tree by swap the left - right children of each node.
2. Use a function, printTree(root), to print the tree in level order.
This function uses a list as a queue to keep track of the nodes.

