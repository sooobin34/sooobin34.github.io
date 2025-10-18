---
title: "DS Project 3 - Korean–English / English–Korean Dictionary"
subtitle: "Bidirectional Dictionary Implementation Using a Binary Search Tree"
summary: "Implemented a bidirectional dictionary based on a Binary Search Tree (BST) that supports both Korean→English and English→Korean word searches."

type: post
date: 2025-10-14
share: false

image:
  filename: "bst3.jpg"
# Fourth Unsplash image (bst3.jpg): https://images.unsplash.com/photo-1675044794037-9262cedb6d5d?ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&q=80&w=1332

tags:
  - Data Structure
  - C++
  - Binary Search Tree
  - Dictionary
  - String Search

links:
  - icon: github
    icon_pack: fab
    name: "GitHub Repository"
    url: "https://github.com/sooobin34/DS_Project3"
---

<br>

## 🎯 Project Overview
This project implements a program that manages both **Korean–English (K-E)** and **English–Korean (E-K)** dictionaries using a **Binary Search Tree (BST)**.  

Each dictionary consists of a key–value relationship:  
- K-E Dictionary: *Korean word → English word*  
- E-K Dictionary: *English word → Korean word*  

Users can perform word insertion, bilingual search, and dictionary printing.  
By using a tree-based search structure, the program enables efficient word lookup and management.

<br>

## 📄 Project Report  
For detailed design and experimental results, refer to the [report](/files/ds_project123_report.pdf).

<br>

## ⚙️ Main Features & Structure
| Component | Description |
|------------|-------------|
| `insert()` | Inserts Korean and English words into two separate trees (K-E, E-K) |
| `searchWord()` | Takes a Korean word as input and returns its English translation (K-E search) |
| `searchMeaning()` | Takes an English word as input and returns its Korean translation (E-K search) |
| `printAllWords()` | Prints both dictionaries in sorted order (inorder traversal) |
| `remove()` | Deletes the specified word from the tree (duplicate keys not allowed) |

<br>

## 🧠 Algorithm Summary
- **Data Structure:** Binary Search Tree  
- **Search Criteria:** Lexicographical order using `strcmp`  
- **Traversal Methods:**  
  - **Inorder traversal** for dictionary printing  
  - K-E and E-K dictionaries are managed separately in independent trees  
- **Time Complexity:**  
  - Insertion / Search / Deletion: O(log n)  
  - Printing: O(n)  
- **Key Points:**  
  - Supports **string inputs containing spaces** in both languages  
  - Each word is managed as a **node object (`Record`)** for reusability  

<br>

## 🧩 Technologies Used
- **Language:** C++  
- **Data Structure:** Binary Search Tree  
- **Core Classes:** `Record`, `BinaryNode`, `BinSrchTree`, `Dictionary`  
- **Input/Output:** String input handling using `cin` and `getline()`  
- **Search Options:**  
  - `k` → Korean–English (K-E) search  
  - `e` → English–Korean (E-K) search  
  - `p` → Print all dictionary entries  
  - `q` → Quit program  

<br>

## 💡 Key Learnings
- Learned the importance of **string-based comparison and sorting** when implementing a Binary Search Tree for textual data.  
- Practiced using `getline()` to handle **string inputs containing spaces**.  
- Understood the need for **data consistency and memory management** when maintaining two trees simultaneously.  
- Designed and implemented a **bidirectional search structure (K→E, E→K)** using tree traversal logic.  

<br>

## 📘 Conclusion
Through this project, I reconfirmed the **efficiency of tree-based search structures**.  
By implementing a BST with strings as keys, I gained a clear understanding of how **comparison operations, insertion/deletion logic, and traversal methods** differ from numerical trees.  
Managing two trees in parallel provided practical insight into **data redundancy handling and search optimization** beyond single-structure systems.

<dr>
