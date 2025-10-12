---
title: ""
type: landing
sections:
  # 메인 Hero 섹션
  - block: hero
    content:
      title: "안수빈의 포트폴리오"
      text: |
        인공지능, 데이터베이스, 파이썬을 중심으로 한 다양한 프로젝트를 소개합니다.  
        아래에서 각 프로젝트를 확인해보세요!
      image:
        filename: "main.png"
      # 이미지 위에 반투명 오버레이 적용
      overlay_color: "#000"
      overlay_filter: 0.3
    design:
      alignment: center
      background:
        color: "#000000"
      spacing:
        padding: ["60px", "0", "60px", "0"]      
sections:
  - block: slider
    content:
      slides:
        - image:
            filename: "uploads/slide-ai.png"
            alt: "AI 프로젝트"
          title: "AI Project"
          text: "탐색 알고리즘과 휴리스틱 평가를 활용한 오목 인공지능"
        - image:
            filename: "uploads/slide-db.jpg"
            alt: "Database 프로젝트"
          title: "Database Project"
          text: "애견인을 위한 정보 제공 및 용품 거래 웹사이트 DB 설계"
        - image:
            filename: "uploads/slide-py.jpg"
            alt: "Python 프로젝트"
          title: "Python Project"
          text: "파이썬을 이용한 게임 구현"
    design:
      slide_interval: 4000 
      alignment: center
      background:
        color: "#ffffff"

  

  # 프로젝트 카드 9개
  - block: collection
    content:
      title: "📂 주요 프로젝트"
      subtitle: "AI, Database, Python 프로젝트 모음"
      count: 9
      filters:
        folders:
          - ai
          - database
          - python
    design:
      view: card
      columns: 3

  # 자기소개 요약 (About 요약)
  - block: markdown
    content:
      title: "👋 About Me"
      text: |
        전북대학교 **컴퓨터인공지능학부** 재학 중이며,  
        **AI·데이터베이스·웹 서비스 개발**을 중심으로 다양한 학습과 프로젝트를 수행했습니다.  
        문제 해결을 위한 알고리즘 설계와 시스템 구조화를 좋아합니다.  
        <br><br>
        📫 **Email:** sooobin0304@naver.com  
        🌐 **GitHub:** [sooobin34](https://github.com/sooobin34)
    design:
      alignment: center
      background:
        color: "#f9f9f9"
---

