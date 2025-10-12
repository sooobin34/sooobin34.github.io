---
title: ""
type: landing

sections:
  # 메인 이미지
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
            color: '#ffffffff'

        - title: "Database Project"
          content: "애견인을 위한 정보 제공 및 용품 거래 DB 설계"
          align: center
          background:
            image:
              filename: slide-db.jpg
              filters:
                brightness: 0.45
            position: center
            color: '#ffffffff'

        - title: "Python Project"
          content: "탐색 알고리즘을 이용한 8퍼즐 문제 해결"
          align: center
          background:
            image:
              filename: slide-py.png
              filters:
                brightness: 0.5
            position: center
            color: '#ffffffff'

    design:
      slide_height: '430px'
      is_fullscreen: false
      loop: true
      interval: 3000
#    advanced:
#      css_style: |
#        .slick-dots li button:before { color: #6c63ff !important; font-size: 12px; }
#        .slick-dots li.slick-active button:before { color: #ff6584 !important; }
#       .slick-prev, .slick-next { display: none !important; }

  # 프로젝트 카드 9개 (3×3)
  - block: collection
    content:
      title: "주요 프로젝트"
      subtitle: "AI · Database · Python 다양한 프로젝트를 한눈에"
      count: 9
      page_type: post
      filters:
        folders:
          - ai
          - ai/ai_info
          - database
          - python
    design:
      view: card
      columns: 3
    advanced:
      css_style: |
        .block-collection .card-grid {
          display: grid !important;
          grid-template-columns: repeat(3, 1fr) !important;
          gap: 20px !important;
          justify-items: center !important;
        }
        .block-collection .card {
          width: 100% !important;
          max-width: 350px !important;
        }

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
        color: "#a8c1caff"
---
