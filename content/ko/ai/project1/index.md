---
title: "AI 오목 — 딥러닝 기반 게임 플레이어"
summary: "오목 게임에 인공지능을 적용하여 상대방 수를 예측하고 자동으로 돌을 두는 AI를 구현했습니다."
type: post
date: 2025-10-10

image:
  filename: "gomoku.png"
  caption: "AI가 둔 수를 시각화한 예시 화면"

tags:
  - AI
  - Game
  - Deep Learning

links:
  - icon: github
    icon_pack: fab
    name: "GitHub Repository"
    url: "https://github.com/sooobin34/ai-gomoku"
---

## 🎯 프로젝트 개요
CNN 모델을 활용하여 오목 게임의 보드 상태를 학습시켰습니다.  
AI가 **상대방의 수를 분석**하고, **다음 수의 승률을 예측**하여 돌을 두도록 설계했습니다.

## ⚙️ 사용 기술
- Python, TensorFlow, OpenCV  
- Alpha-Beta Pruning, Minimax 알고리즘  
- 보드 상태 학습 및 평가 함수 설계  

## 💡 배운 점
딥러닝과 탐색 알고리즘을 결합하여 AI 의사결정 과정을 이해했습니다.  
특히 **시간 복잡도 최적화**와 **데이터 전처리 중요성**을 실감했습니다.
