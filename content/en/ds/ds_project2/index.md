---
title: "DS Project 2 - Counting Path Sums in a Binary Search Tree"
subtitle: "Calculating the Number of Paths Starting from the Root with a Sum Equal to X"
summary: "Implemented a program that counts all paths starting from the root of a Binary Search Tree (BST) whose node values sum up to X."

type: post
date: 2025-10-14
share: false

image:
  filename: "bst2.jpg"
# Third Unsplash image (bst2.jpg): https://images.unsplash.com/photo-1664526937033-fe2c11f1be25?ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&q=80&w=1332

tags:
  - Data Structure
  - C++
  - Binary Search Tree
  - Path Sum
  - Algorithm

links:
  - icon: github
    icon_pack: fab
    name: "GitHub Repository"
    url: "https://github.com/sooobin34/DS_Project2"
---

<br>

## 🎯 Project Overview
This project is based on a **Binary Search Tree (BST)** and implements a program that **counts all paths starting from the root whose node values sum to X**.  

By traversing each node, the program keeps track of the cumulative sum at each step and uses an **`unordered_map`** to efficiently calculate the number of paths where the same sum occurs.

<br>

## 📄 Project Report  
For detailed design steps and execution results, refer to the [report](/files/ds_project123_report.pdf).

<br>

## ⚙️ Main Features & Structure
| Component | Description |
|------------|-------------|
| `insertNode()` | Inserts a given key following BST rules |
| `deleteNode()` | Maintains tree structure after deletion using the successor node (`findMin`) |
| `countPathsWithSum()` | Recursively counts all paths whose cumulative sum equals X |
| `findMin()` | Returns the node with the smallest value in the right subtree |
| `unordered_map` | Stores frequency of path sums to avoid redundant calculations |

<br>

## 🧠 Algorithm Summary
- **Traversal Method:** DFS (Depth-First Search)  
- **Core Idea:**  
  - Calculate cumulative sums for all paths starting from the root  
  - Check in the hash map whether `(currentSum - targetSum)` has appeared before  
  - Efficiently count overlapping paths without redundancy  
- **Time Complexity:** O(n)  
- **Space Complexity:** O(n) (due to the hash map for storing path sums)

<br>

## 🧩 Technologies Used
- **Language:** C++  
- **Data Structure:** Binary Search Tree  
- **Algorithm:** DFS + Prefix Sum + Hash Map  
- **I/O Method:** Standard input (`scanf`) / Standard output (`printf`)  

<br>

## 💡 Key Learnings
- Understood the relationship between **recursive traversal and cumulative sum computation** in a Binary Search Tree.  
- Learned how to apply **hash maps for tracking cumulative sums** when solving path sum problems.  
- Realized the importance of balancing **time and space efficiency** during tree traversal and problem-solving.  

<br>

## 📘 Conclusion
Through this project, I learned how to combine **prefix sums** and **DFS traversal techniques** to efficiently solve problems beyond basic Binary Search Tree operations.

<dr>
