---
title: "DS Project 1 - Checking Binary Search Tree Balance"
subtitle: "Balanced Tree Detection Using the isBalanced() Function"
summary: "Implemented an isBalanced() function that determines whether a Binary Search Tree (BST) with insertion, deletion, and search features is balanced."

type: post
date: 2025-10-13
share: false

image:
  filename: "bst1.jpg"

tags:
  - Data Structure
  - C++
  - Binary Search Tree
  - Balanced Tree
  - Algorithm

links:
  - icon: github
    icon_pack: fab
    name: "GitHub Repository"
    url: "https://github.com/sooobin34/DS_Project1"
---

<br>

## 🎯 Project Overview
This project implements the insertion and deletion operations of a **Binary Search Tree (BST)** and defines the `isBalanced()` function to determine whether the tree is balanced.  
A balanced tree is defined as one where **the height difference between the left and right subtrees is no more than 1**, and both subtrees themselves are balanced.

<br>

## 📄 Project Report  
For a detailed implementation process, refer to the [report](/files/ds_project123_report.pdf).

<br>

## ⚙️ Main Features & Structure
| Component | Description |
|------------|-------------|
| `getHeight()` | Recursively calculates the height of the subtree for a given node |
| `isBalanced()` | Compares the height difference between the left and right subtrees to determine balance |
| `insertNode()` | Inserts a key value following BST rules |
| `deleteNode()` | Maintains tree structure after deletion using the successor node (`findMin`) |
| `findMin()` | Returns the node with the smallest value in the right subtree |

<br>

## 🧠 Algorithm Summary
- **Balance Conditions:**  
  1. The left subtree is balanced  
  2. The right subtree is balanced  
  3. The height difference between the two subtrees is ≤ 1  
- **Traversal Method:** Recursive traversal  
- **Time Complexity:** O(n) (visits every node to compute height)

<br>

## 🧩 Technologies Used
- **Language:** C++  
- **Data Structure:** Binary Search Tree  
- **Core Functions:** Recursive height calculation and balance checking  
- **I/O Method:** Standard input (`scanf`) and standard output (`printf`)  

<br>

## 💡 Key Learnings
- Gained an understanding of how to check tree height and balance simultaneously using recursion.  
- Implementing insertion and deletion operations helped me grasp the importance of **node linkage and pointer management** in tree structures.  
- Built a conceptual foundation for **self-balancing trees** such as AVL and Red-Black Trees.  

<br>

## 📘 Conclusion
Through this project, I practiced the **concept of tree balance and recursive problem-solving techniques**.  
By implementing an algorithm that evaluates structural stability beyond basic insertion and deletion,  
I developed a clearer understanding of how theoretical data structure concepts translate into practical code.

<br>
