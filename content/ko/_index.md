---
title: ""
type: landing

sections:
  - block: hero
    content:
      title: "안수빈의 포트폴리오"
      text: |
        인공지능, 데이터베이스, 파이썬을 중심으로 한 다양한 프로젝트를 소개합니다.  
        아래에서 각 프로젝트를 확인해보세요!
      image:
        slides:               
          - filename: "slide-ai.png"
          - filename: "slide-db.jpg"
          - filename: "slide-py.jpg"
      overlay_color: "#000"    
      overlay_filter: 0.3      
    design:
      alignment: center
      background:
        color: "#000000"
      spacing:
        padding: ["150px", "0", "150px", "0"]

  # 프로젝트 카드 9개 섹션
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

  # 자기소개 요약 (About)
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
        color: "#cfc9acc0"
---
