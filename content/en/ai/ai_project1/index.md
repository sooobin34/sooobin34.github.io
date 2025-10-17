---
title: "AI Project 1 – Omok"
subtitle: "Alpha-Beta Based Artificial Intelligence Omok Player"
summary: "Developed an Omok (Gomoku) AI player using a search algorithm and heuristic evaluation function."

type: post
date: 2025-10-10
share: false
draft: false

image:
  filename: "omok_ai.jpg"

tags:
  - Artificial Intelligence
  - Game AI
  - Search Algorithm
  - Python

links:
  - icon: github
    icon_pack: fab
    name: "GitHub Repository"
    url: "https://github.com/sooobin34/AI_Project1"
---

<br>

## 🎯 Project Overview
This project implements an **Omok (Gomoku) AI player** using the **Alpha-Beta pruning algorithm** and a **heuristic evaluation function**.  
The AI determines the optimal stone placement by pruning unnecessary branches, allowing it to make **reasonable moves within 5 seconds**.

<br>

## 📄 Project Report
If you’d like to learn more about the project, [download the report](/files/ai_project1_report.pdf)!

<br>

## ⚙️ Main Features & Structure
| Component | Description |
|------------|-------------|
| `get_candidate_moves()` | Searches valid candidate coordinates around existing stones to reduce unnecessary computation |
| `find_critical_block()` | Detects offensive or defensive situations (e.g., 3- or 4-in-a-row) and responds immediately |
| `evaluate()` | Calculates scores based on stone continuity, open ends, and opponent’s state |
| `minimax()` | Determines the optimal move based on search depth with Alpha-Beta pruning applied |
| `act()` | Integrates all functions to execute the AI’s actual move |

<br>

## 🧠 Algorithm Summary
- **Search Algorithm:** Minimax + Alpha-Beta Pruning  
- **Heuristic Evaluation:** Weighted by the number of connected stones (`count`) and open directions (`open_ends`)  
- **Search Depth:** Up to 2 levels (ensures response within 5 seconds)  
- **Strategy:**  
  1. Prioritize winning moves  
  2. Block opponent’s 4-in-a-row  
  3. Block opponent’s 3-in-a-row  
  4. Choose optimal move based on heuristic evaluation  

<br>

## 🧩 Technologies Used
- **Language:** Python  
- **Libraries:** NumPy, copy  
- **Modules:** `omok.py` (game environment), `ai.py` (AI logic)  
- **Search Technique:** DFS-based state tree + Alpha-Beta pruning  

<br>

## 📈 Results & Performance
- Improved search efficiency by **approximately 45%** compared to basic Minimax  
- Able to make sound decisions **within the 5-second time limit**  
- **Performance improved further** when refining the heuristic evaluation function  

<br>

## 💡 Key Learnings
- Realized the importance of **search space reduction and heuristic design** in game AI.  
- Gained experience in **mathematically modeling the decision-making process** of AI.  
- Understood how the combination of **search algorithms and heuristics** leads to more efficient and intelligent behavior than simple rule-based logic.

<br>
