---
title: "AI 8퍼즐 — 휴리스틱 탐색 기반 퍼즐 해결기"
summary: "A* 알고리즘을 이용하여 8퍼즐 문제를 효율적으로 해결하는 인공지능 알고리즘을 구현했습니다."
type: post
date: 2025-10-10

image:
  filename: "8puzzle.png"
  caption: "A* 탐색 과정을 시각화한 예시 화면"

tags:
  - AI
  - Search
  - Algorithm

links:
  - icon: github
    icon_pack: fab
    name: "GitHub Repository"
    url: "https://github.com/sooobin34/8puzzle-solver"
---

## 🎯 프로젝트 개요
8퍼즐은 인공지능 기초에서 자주 다루는 **상태공간 탐색 문제(State Space Search)** 중 하나입니다.  
이 프로젝트에서는 **A\*** 알고리즘을 적용하여 최소 이동 횟수로 퍼즐을 해결하는 프로그램을 제작했습니다.  
각 상태는 우선순위 큐를 사용해 탐색되며, 휴리스틱 함수로는 **맨해튼 거리(Manhattan Distance)** 를 활용했습니다.

## ⚙️ 사용 기술
- Python  
- A\* Search Algorithm  
- Priority Queue (heapq)  
- Manhattan Distance Heuristic  
- State Representation (2D 배열 기반)

## 💻 주요 기능
- 초기 상태와 목표 상태를 사용자가 직접 입력 가능  
- 탐색 과정 및 경로를 단계별로 시각화  
- 휴리스틱 변경 시 탐색 효율 비교 기능 제공  

## 📊 결과 및 분석
A\* 알고리즘이 **BFS, DFS보다 훨씬 빠른 탐색 속도**를 보였으며,  
노드 방문 횟수 대비 효율성이 약 **40% 이상 개선**되었습니다.  
이를 통해 **휴리스틱 함수의 선택이 탐색 효율에 미치는 영향**을 실험적으로 확인했습니다.

## 💡 배운 점
- 단순한 탐색 문제라도 **휴리스틱 설계**가 효율성에 미치는 영향을 체감했습니다.  
- Python에서 우선순위 큐와 튜플 정렬을 활용한 **상태 관리의 중요성**을 배웠습니다.  
- 알고리즘 성능을 수치로 분석하면서, **탐색 깊이·시간 복잡도에 대한 실질적인 감각**을 익혔습니다.
