---
title: "AI Projects Overview"
type: landing
date: 2025-10-12
draft: false

sections:
  - block: markdown
    content:
      title: "🧠 인공지능 프로젝트 소개"
      text: |
        전북대학교 **인공지능(Artificial Intelligence)** 수업에서 수행한 프로젝트들을 소개합니다.  
        각 프로젝트에서는 탐색 알고리즘과 휴리스틱 평가 함수를 직접 구현하며,  
        **게임 인공지능 및 탐색 문제 해결 능력**을 향상시키는 데 중점을 두었습니다.

  - block: collection
    content:
      title: "📂 프로젝트 목록"
      text: ""
      filters:
        folders:
          - ai
        exclude_folders:
          - ai/ai_info
    design:
      view: card
      columns: 2
      spacing:
        padding: ["20px", "20px", "20px", "20px"]

  - block: markdown
    content:
      title: "🔗 프로젝트 바로가기"
      text: |
        [Project 1 – Alpha-Beta 탐색 기반 오목 인공지능](../ai_project1/)  
        [Project 2 – 휴리스틱을 이용한 8퍼즐 문제 해결](../ai_project2/)
---
