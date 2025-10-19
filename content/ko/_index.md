---
title: ""
type: landing
view: compact

sections:
  # 메인 이미지 슬라이더
  - block: slider
    content:
      slides:
        - title: "AI Project"
          content: "Alpha-Beta 탐색 기반 오목 인공지능"
          align: center
          background:
            image:
              filename: slide-ai.png 
              filters:
                brightness: 0.6
            position: center
            color: "#ffffffff"

        - title: "Database Project"
          content: "애견인을 위한 정보 제공 및 용품 거래 DB 설계"
          align: center
          background:
            image:
              filename: slide-db.jpg 
              filters:
                brightness: 0.45
            position: center
            color: "#ffffffff"

        - title: "Python Project"
          content: "탐색 알고리즘을 이용한 8퍼즐 문제 해결"
          align: center
          background:
            image:
              filename: slide-py.png
              filters:
                brightness: 0.5
            position: center
            color: "#ffffffff"

        - title: "Ds Project"
          content: "이진 탐색 트리를 활용한 다양한 자료구조 프로젝트 모음"
          align: center
          background:
            image:
              filename: slide-ds.jpg
              filters:
                brightness: 0.5
            position: center
            color: "#ffffffff"

    design:
      slide_height: "430px"
      is_fullscreen: false
      loop: true
      interval: 3000
    advanced:
      css_style: |
        .slick-prev, .slick-next { display: none !important; }

  #프로젝트 카드 
  #- block: collection
  #  content:
  #    title: "주요 프로젝트"
  #    subtitle: "AI · Database · Python 프로젝트"
  #    count: 9
  #    filters:
  #      folders:
  #        - ai
  #        - database
  #        - python
  #        - ds
  #  design:
  #    view: card 
  #    columns: 3
  #    spacing:
  #      padding: ["20px", "20px", "20px", "20px"]
  
  # 커스텀 뷰1
  - block: collection
    content:
      title: "AI, DS 프로젝트"
      count: 9
      filters:
        folders:
          - ai
          - ds
    design:
      view: compact
      columns: 3

  # 커스텀 뷰2
  - block: collection
    content:
      title: "DB, PY 프로젝트"
      count: 9
      filters:
        folders:
          - database
          - python  
    design:
      view: overlay
      columns: 3



  # 자기소개 요약
  - block: markdown
    content:
      title: "About Me"
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
        color: "#e2f7ffff"
---
