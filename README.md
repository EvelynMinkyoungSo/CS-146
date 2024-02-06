Approach 
Step 1
Create a `HashMap` that will store integer values as keys and their indices as values. 
This map serves to keep track of the elements we've already seen as we iterate through the array.

Step 2
Loop through the array of numbers. For each element, 
calculate its complement by subtracting the element's value from the target value.

Step 3
For every element, check if its complement already exists in the map. 
If it does, it means we have found the two numbers that add up to the target. 
The indices of these numbers are then retrieved - one directly from the map (for the complement) 
and the other is the current index in the array.

Step 4
If no solution is found by the end of the iteration, throw an `IllegalArgumentException`. 
This serves as a safeguard, although the problem statement guarantees exactly one solution.

Array [3,1,4,2,5,7,6]
Target [8]
Starting at the first element 3 index 0 and move to the next element.

This approach with O(n) time complexity.
