---
title: "DS Project 2 - 이진 탐색 트리 합 경로 세기"
subtitle: "루트에서 시작하는 경로의 합이 X가 되는 경우의 수 계산"
summary: "이진 탐색 트리에서 루트 노드부터 시작하는 경로 중 합이 X가 되는 모든 경우의 수를 계산하는 프로그램을 구현했습니다."

type: post
date: 2025-10-14
share: false

image:
  filename: "bst.jpg"

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
    url: "https://github.com/sooobin34/ds_project2"
---

<br>

## 🎯 프로젝트 개요
이 프로젝트는 **이진 탐색 트리(Binary Search Tree)** 를 기반으로,  
루트 노드부터 시작하는 모든 경로 중에서 **노드들의 합이 X가 되는 경우의 수를 계산하는 프로그램**을 구현한 과제입니다.  

트리의 각 노드를 순회하며 현재까지의 누적 합을 기록하고,  
해시맵(`unordered_map`)을 이용해 동일한 합이 발생한 경로의 수를 효율적으로 계산합니다.  

<br>

## 📄 프로젝트 보고서  
구체적인 설계 과정과 실행 결과는 [보고서](/files/ds_project123_report.pdf)를 참고하세요!

<br>

## ⚙️ 주요 기능 및 구조
| 구성 요소 | 설명 |
|------------|-------|
| `insertNode()` | 주어진 키를 BST 규칙에 따라 삽입 |
| `deleteNode()` | 삭제 시 후계자 노드(`findMin`)를 사용하여 트리 구조를 유지 |
| `countPathsWithSum()` | 누적 합이 X가 되는 모든 경로의 개수를 재귀적으로 계산 |
| `findMin()` | 오른쪽 서브트리에서 가장 작은 값을 가진 노드를 반환 |
| `unordered_map` | 경로 합 빈도를 저장하여 중복 계산을 방지 |

<br>

## 🧠 알고리즘 요약
- **탐색 방식:** DFS(깊이 우선 탐색, Depth-First Search)  
- **핵심 아이디어:**  
  - 루트부터 시작하는 모든 경로의 누적 합을 계산  
  - 현재 합(`currentSum`)에서 목표 합(`targetSum`)을 뺀 값이 이전에 등장했는지를 해시맵에서 확인  
  - 중복 경로를 효율적으로 카운트  
- **시간 복잡도:** O(n)  
- **공간 복잡도:** O(n) (경로 합을 저장하는 해시맵 사용)

<br>

## 🧩 사용 기술
- **언어:** C++  
- **자료구조:** Binary Search Tree  
- **알고리즘:** DFS + 누적 합(Partial Sum) + Hash Map  
- **입출력 방식:** 표준 입력(`scanf`) / 표준 출력(`printf`)  

<br>

## 💡 배운 점
- 이진 탐색 트리에서의 **재귀적 순회와 누적 합 계산의 관계**를 이해하게 되었습니다.  
- 경로 합 문제를 해결하기 위해 **해시맵을 이용한 누적 합 기록법** 을 공부하였습니다.  
- 이 과제를 통해 트리 탐색 과정에서 **시간 효율성과 공간 효율성의 균형**을 생각해 봐야한다는 중요성을 배웠습니다.  

<br>

## 📘 결론
이번 과제를 통해 단순한 이진 탐색 트리 구조를 넘어, **누적 합(prefix sum)** 과 **DFS 탐색 기법**을 결합하여 문제를 효율적으로 해결할 수 있는 방법을 배웠습니다.

<dr>