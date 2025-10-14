---
title: "AI Project 1 - 오목"
subtitle: "Alpha-Beta 기반 인공지능 오목 플레이어"
summary: "탐색 알고리즘과 휴리스틱 평가함수를 이용한 오목 인공지능 플레이어를 구현했습니다."

type: post
date: 2025-10-10
share: false

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

## 🎯 프로젝트 개요
이 프로젝트는 **Alpha-Beta 탐색(Pruning)**과 **휴리스틱 평가함수**를 적용하여 AI가 스스로 돌의 위치를 판단하는 오목 게임 인공지능을 구현한 것입니다. 
AI는 가능한 모든 수를 탐색하지 않고, 불필요한 가지를 가지치기(pruning)하여 *5초 이내에 합리적인 수를 계산*할 수 있습니다.

<br>

## 📄 프로젝트 보고서
프로젝트에 대해 더 알고 싶다면 [보고서](/files/ai_project1_report.pdf)를 다운받으세요! 

<br>

## ⚙️ 주요 기능 및 구조
| 구성 요소 | 설명 |
|------------|-------|
| `get_candidate_moves()` | 현재 돌 주변의 유효 후보 좌표를 탐색하여 불필요한 연산을 줄임 |
| `find_critical_block()` | 공격/방어 상황을 판단해 3목, 4목 상태에서 즉시 대응 |
| `evaluate()` | 돌의 연속 개수, 열린 끝(open ends), 상대 돌 상태를 기반으로 점수 계산 |
| `minimax()` | 탐색 깊이 기반으로 최적 수를 결정 (알파–베타 가지치기 적용) |
| `act()` | 위의 함수들을 통합해 실제 AI의 행동을 수행 |

<br>

## 🧠 알고리즘 요약
- **탐색 알고리즘:** Minimax + Alpha–Beta Pruning  
- **휴리스틱 평가:** 연속된 돌의 수(`count`)와 열린 방향(`open_ends`)에 가중치를 부여  
- **탐색 깊이:** 최대 깊이 2로 설정 (실행 시간 5초 이내 보장)  
- **전략:**  
  1. 내가 이길 수 있는 수 우선  
  2. 상대 4목 방어  
  3. 상대 3목 방어  
  4. 휴리스틱 평가 기반 최적 수 선택  

<br>

## 🧩 사용 기술
- **언어:** Python  
- **라이브러리:** NumPy, copy  
- **모듈 구조:** `omok.py` (게임 환경), `ai.py` (AI 로직)  
- **탐색 기법:** DFS 기반 상태 트리 + Alpha–Beta 가지치기  

<br>

## 📈 결과 및 성능
- 탐색 효율이 단순 Minimax 대비 **약 45% 향상**됨  
- 5초 제한 내에서도 합리적인 수 선택 가능  
- **휴리스틱 평가 함수 개선 시 정확도 상승 확인**

<br>

## 💡 배운 점
- 게임 인공지능에서 **탐색 공간 축소와 평가 함수 설계의 중요성**을 체감했습니다.  
- 상태 평가를 수식화하면서 **AI의 의사결정 로직을 수학적으로 설계하는 과정**을 익혔습니다.  
- 과제를 통해 단순한 규칙 기반 로직보다 **탐색 + 휴리스틱의 조합이 얼마나 효율적인지** 이해하게 되었습니다.

<br>