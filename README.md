Algorithm
1. Begin the search for the LCA from the root node of the BST
2. If both nodes p and q are greater than the current node's value, it means the LCA lies in the right subtree side.
Therefore move to the right child of the current node.
3. If both nides p and q are less then the current node's value, it means the LCA lies in the left subtree side.
Therefore movw to left child of the current node.
4. If none of the above conditions are true, then one node is to the left and the other node is to the right of the current node.
5. The current node is either a p or q node.


Finding the LCA
LCA of nodes p and q if the current node does not satisfy any of the above-mentioned traversal conditions. 
This is because the paths from the root to p and q branch at this point, or one of them is an LCA.


End condition
If during the traversal, the current node become null.
It indicates that the LCA dne within the tree.
Which sould not happen in a vaild BST for two existing node.


This approach efficiently utilizes the BST property to minimize the traversal needed to find the LCA, 
resulting in a time complexity of O(h), where h is the height of the tree.
