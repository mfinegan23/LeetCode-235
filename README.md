# LeetCode-235

This repository contains the solution to LeetCode Problem #235: Lowest Common Ancestor of a Binary Search Tree.

# Problem Statement:
Given a Binary Search Tree (BST), find the Lowest Common Ancestor (LCA) of two given nodes p and q.

The LCA is defined as the lowest node in the BST that has both p and q as descendants (a node can be a descendant of itself).

Example 1:
Input: root = [6,2,8,0,4,7,9,null,null,3,5], p = 2, q = 8  
Output: 6

Example 2:
Input: root = [6,2,8,0,4,7,9,null,null,3,5], p = 2, q = 4  
Output: 2

Example 3:
Input: root = [2,1], p = 2, q = 1  
Output: 2

# Constraints:

The number of nodes in the tree is in the range [2, 10^5].

-10^9 <= Node.val <= 10^9

All Node.val are unique.

p != q

p and q will exist in the BST.

# Solution:
The solution is implemented in Java. It uses the properties of a Binary Search Tree to efficiently find the Lowest Common Ancestor:

Recursive Approach:
If both p and q are less than the current node's value, the LCA lies in the left subtree.
If both p and q are greater than the current node's value, the LCA lies in the right subtree.
If p and q lie on either side of the current node (or one of them is equal to the current node), the current node is the LCA.


# How to Run
Clone the Repository:

git clone https://github.com/your-username/lowest-common-ancestor-bst.git
cd lowest-common-ancestor-bst

Compile the Code: Ensure you have Java installed on your machine. 
Compile the Solution.java file: javac Solution.java

Run the Solution: Create test cases for the lowestCommonAncestor method in a main function, or integrate it with a testing framework to verify its correctness.

Testing: You can use online IDEs like LeetCode to test the solution with custom test cases.


#
Note: In the video solution, lowestCommonAncestor is referred to as LCA as the method name.
