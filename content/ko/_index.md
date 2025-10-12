---
title: ""
type: landing

sections:
  # 🎯 메인 Hero 섹션 (메인 이미지 + 타이틀/텍스트)
  - block: hero
    content:
      title: "안수빈의 포트폴리오"
      text: |
        인공지능, 데이터베이스, 파이썬을 중심으로 한 다양한 프로젝트를 소개합니다.  
        아래에서 각 프로젝트를 확인해보세요!
      image:
        filename: "main.png"     
      overlay_color: "#d8d1d1ff"    
      overlay_filter: 0.3
    design:
      alignment: center
      text_color_light: true
      spacing:
        padding: ["150px", "0", "150px", "0"]

  #이미지 슬라이드 (자동 전환)
  - block: hero
    content:
      slides:
        - filename: "slide-ai.png"
          text: "탐색 알고리즘을 활용한 오목 인공지능"
        - filename: "slide-db.jpg"
          text: "애견인을 위한 정보 제공 및 용품 거래 웹사이트 DB 설계"
        - filename: "slide-py.png"
          text: "파이썬으로 구현한 다양한 알고리즘 프로젝트"
      overlay_color: "#d8d1d1ff"
      overlay_filter: 0.3
    design:
      alignment: center
      text_color_light: true
      spacing:
        padding: ["150px", "0", "150px", "0"]

  # 📂 프로젝트 카드 9개 (3×3)
  - block: collection
    content:
      title: "📂 주요 프로젝트"
      subtitle: "AI · Database · Python 분야의 다양한 프로젝트를 한눈에"
      count: 9
      filters:
        folders:
          - ai
          - database
          - python
    design:
      view: card
      columns: 3

  # 👋 자기소개 요약
  - block: markdown
    content:
      title: "👋 About Me"
      text: |
        전북대학교 **컴퓨터인공지능학부** 재학 중이며,  
        **AI·데이터베이스·웹 서비스 개발**을 중심으로 다양한 프로젝트를 수행했습니다.  
        문제 해결을 위한 **알고리즘 설계와 시스템 구조화**를 좋아합니다.  
        <br><br>
        📫 **Email:** sooobin0304@naver.com  
        🌐 **GitHub:** [sooobin34](https://github.com/sooobin34)
    design:
      alignment: center
      background:
        color: "#f9f9f9"
---
