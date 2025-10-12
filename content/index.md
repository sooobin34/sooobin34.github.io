---
title: "SB_Portfolio"
type: landing
date: 2025-10-12

sections:
  - block: hero
    content:
      title: "안수빈의 개발 포트폴리오"
      text: |
        전북대학교 컴퓨터인공지능학부  
        AI · Database · Web Development  
      image:
        filename: main.jpg
        filters:
          brightness: 0.4
      align: center

  # 슬라이더

  - block: carousel
    content:
      slides:
        - image:
            filename: slide-ai.jpg
          title: "AI 프로젝트"
          text: "탐색 알고리즘을 이용한 퍼즐 AI 구현"
        - image:
            filename: slide-db.jpg
          title: "Database 프로젝트"
          text: "애견인 커뮤니티 DB 설계 및 구현"
        - image:
            filename: slide-py.jpg
          title: "파이썬 개발"
          text: "파이썬을 이용한 게임 개발 및 알고리즘 구현"
    design:
      interval: 3500
      height: "medium"
      show_caption: true

  
  # 프로젝트 카드 9개 (3×3)

  - block: collection
    content:
      title: "📂 주요 프로젝트"
      subtitle: "AI · Database · Web 등 다양한 작업물"
      count: 9
      filters:
        folders:
          - project
      order: desc
    design:
      view: card
      columns: '3'
---
