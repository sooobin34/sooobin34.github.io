---
title: "DS Project 1 - 이진 탐색 트리 균형 확인"
subtitle: "isBalanced() 함수를 이용한 Balanced Tree 판별 프로그램"
summary: "삽입, 삭제, 검색 기능을 지원하는 이진 탐색 트리에서 트리의 균형 여부를 판별하는 isBalanced() 함수를 구현했습니다."

type: post
date: 2025-10-13
share: false

image:
  filename: "bst_balanced.jpg"

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
    url: "https://github.com/sooobin34/ds_project1"
---

<br>

## 🎯 프로젝트 개요
이 프로젝트는 **이진 탐색 트리(Binary Search Tree, BST)** 의 삽입과 삭제 연산을 구현하고, 트리가 균형(Balanced) 상태인지 판별하는 `isBalanced()` 함수를 작성하는 과제입니다.  
트리의 균형이란, **왼쪽 서브트리와 오른쪽 서브트리의 높이 차이가 1 이하이며**, 각 서브트리 또한 모두 균형 잡혀 있는 상태를 의미합니다.

<br>

## 📄 프로젝트 보고서  
자세한 구현 과정은 [보고서](/files/ds_project123_report.pdf)를 참고하세요!

<br>

## ⚙️ 주요 기능 및 구조
| 구성 요소 | 설명 |
|------------|-------|
| `getHeight()` | 주어진 노드의 서브트리 높이를 재귀적으로 계산 |
| `isBalanced()` | 현재 노드와 양쪽 서브트리의 높이 차이를 비교하여 균형 여부 판별 |
| `insertNode()` | 주어진 키 값을 BST 규칙에 따라 삽입 |
| `deleteNode()` | 삭제 시 후계자 노드(`findMin`)를 사용해 트리 구조를 유지 |
| `findMin()` | 오른쪽 서브트리에서 가장 작은 값을 가진 노드 반환 |

<br>

## 🧠 알고리즘 요약
- **트리 균형 조건:**  
  1. 왼쪽 서브트리가 균형일 것  
  2. 오른쪽 서브트리가 균형일 것  
  3. 두 서브트리 높이 차이가 1 이하일 것  
- **탐색 방식:** 재귀(Recursive) 기반 순회  
- **시간 복잡도:** O(n) (모든 노드를 방문하여 높이 계산)

<br>

## 🧩 사용 기술
- **언어:** C++  
- **자료구조:** Binary Search Tree  
- **핵심 함수:** 재귀 기반 높이 계산 및 균형 판별  
- **입출력 방식:** 표준 입력(`scanf`), 표준 출력(`printf`)  

<br>

## 💡 배운 점
- 재귀 호출을 이용해 트리의 높이와 균형 여부를 동시에 검사하는 로직을 이해했습니다.  
- 이진 탐색 트리의 삽입·삭제 시 구조가 변하는 과정을 직접 구현함으로써  
  **노드 연결 구조와 포인터 관리의 중요성**을 체감했습니다.  
- AVL 트리나 Red-Black 트리와 같은 **자기 균형 트리(Self-Balancing Tree)** 로 발전할 수 있는 개념적인 기반을 쌓았습니다.  

<br>

## 📘 결론
이번 프로젝트를 통해 **트리 구조의 균형 개념과 재귀적 문제 해결 방식**을 실습했습니다.  
단순한 삽입/삭제가 아닌 구조적인 안정성을 판단하는 알고리즘을 구현함으로써 자료구조 이론이 실제 코드에 어떻게 적용되는지를 명확히 이해할 수 있었습니다.

<br>