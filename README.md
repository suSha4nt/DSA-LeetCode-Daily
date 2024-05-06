# Remove Nodes From Linked List
Problem Description
You are given the head of a linked list. Your task is to remove every node which has a node with a greater value anywhere to the right side of it.
Return the head of the modified linked list.

![image](https://github.com/suSha4nt/DSA-LeetCode-Daily/assets/157277750/84534f55-4fe7-4ed3-8acc-ad2720232655)


## Example <br>
Input: 1 -> 2 -> 8 -> 3 -> 7 </br>
Output: 1 -> 2 -> 3
## Explanation:

Node 1 has nodes with greater values (2, 8, 3, 7) to its right, so it is removed.
Node 2 has nodes with greater values (8, 3, 7) to its right, so it is removed.
Node 8 has nodes with greater values (3, 7) to its right, so it is removed.
Node 3 has nodes with greater values (7) to its right, so it is removed.
Node 7 has no nodes with greater values to its right, so it remains in the modified list.

## Approach
### We can solve this problem using different approaches:

#### Brute Force : </br>
Compare each node with all nodes to its right and remove it if there’s a greater value node to its right. </br>
#### Using a Stack : </br> 
Use a stack to keep track of nodes in decreasing order. Iterate through the linked list and pop nodes from the stack until we find a greater value node. </br>
#### Reverse the List : </br>
Reverse the linked list and then traverse it. If we find a node with a greater value than the maximum value encountered so far, we remove it. </br>


