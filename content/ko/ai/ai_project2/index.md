---
title: "AI Project 2 - 8퍼즐"
subtitle: "DFS, BFS, UCS, A* 탐색을 이용한 8퍼즐 탐색 알고리즘"
summary: "DFS, BFS, UCS, A* 탐색을 이용한 8퍼즐 문제 해결"

type: post
date: 2025-10-10
share: false
draft: false

image:
  filename: "8puzzle.jpg"

tags:
  - Artificial Intelligence
  - Search Algorithm
  - Python
  - A*

links:
  - icon: github
    icon_pack: fab
    name: "GitHub Repository"
    url: "https://github.com/sooobin34/AI_Project2"      
---
<br>

## 🧩 프로젝트 개요
이 프로젝트는 인공지능 기초 수업의 탐색 알고리즘 단원 과제로 수행한 **8퍼즐 문제(8-Puzzle Problem)** 해결 프로젝트입니다.  
목표 상태에 도달하기 위해 다양한 탐색 기법(DFS, BFS, UCS, A*)을 직접 구현하고 성능을 비교하였습니다.8퍼즐은 3×3 보드에 숫자 타일이 배치되어 있으며, 빈 칸(0)을 상하좌우로 이동시켜 목표 상태에 도달하는 문제입니다.

<br>

## 📄 프로젝트 보고서
프로젝트에 대해 더 알고 싶다면 [보고서](/files/ai_project2_report.pdf)를 다운받으세요!

<br>

## ⚙️ 구현 내용
### 🔹 1. 탐색 알고리즘 구현
- **DFS (깊이 우선 탐색)** : 스택 기반의 탐색으로, 메모리 효율적이지만 최적해를 보장하지 않음  
- **BFS (너비 우선 탐색)** : 큐 기반 탐색으로, 최단 경로를 보장하지만 메모리 사용량이 큼  
- **UCS (Uniform Cost Search)** : 이동 비용을 고려한 탐색으로, 항상 최소 비용 경로 탐색  
- **A\*** : 휴리스틱 함수를 적용한 탐색으로, 가장 효율적으로 목표 상태에 도달함  

<br>

### 🔹 2. 휴리스틱 함수 (Heuristic)
A\* 탐색에서는 **misplaced tile heuristic**을 사용하였습니다.  
이 함수는 제 위치에 있지 않은 타일의 개수를 세어 추정 비용을 계산합니다.

```python
def heuristic(state, problem=None):
    misplaced = 0
    goal = [[1,2,3],[4,5,6],[7,8,0]]
    for row in range(3):
        for col in range(3):
            if state.cells[row][col] != 0 and state.cells[row][col] != goal[row][col]:
                misplaced += 1
    return misplaced
```

<br>

## 🧠 주요 수정 포인트
| 항목 | 변경 내용 |
|------|------------|
| `type: langing` → ✅ `type: post` | 오타 수정 및 블로그형 포맷 적용 |
| `sections:` 제거 | Markdown 본문을 직접 작성하도록 단순화 |
| 깃허브 버튼 추가 | 본문 맨 아래에 시각적으로 깔끔한 버튼 추가 |
| 코드블록 유지 | 파이썬 코드 그대로 유지 (렌더링 깨지지 않음) |
| 불필요한 들여쓰기 제거 | Markdown 파싱 오류 방지 |

<br>