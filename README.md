1. Ensure that the starting pixel coordinates are within the bounds of the image.
2. If the starting pixel's color is already the target color, return the image as-is to avoid unnecessary processing.
3. Recursively apply the DFS algorithm to change the color of the connected component, starting from the specified pixel.
4. After completing the DFS traversal and updating the colors, return the modified image grid.


In Java the solution is encapsulated within a class 'Solution'
with a method 'floodFill' that performs the operation and a helper method 'fill' for the recursive DFS logic.

In python a class 'Solution' is defined with a method 'floodFill', 
including a nested helper function 'dfs' for the recursive logic.

The core of solution utilizes the Depth-First Search algorithm, 
a recursive strategy to explore and modify pixels that are 4-directionally connected and share the same initial color as the starting pixel. 
