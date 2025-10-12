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

  # 프로젝트 카드 (3×3)
  - block: collection
    content:
      title: "주요 프로젝트"
      subtitle: "AI · Database · Python 분야의 다양한 프로젝트를 한눈에"
      count: 9
      page_type: post
      filters:
        folders:
          - ai
          - database
          - python
          - my-skills/my-skills-info
          - contact/contact-info
    design:
      view: projects
      columns: 3
      spacing:
        padding: ["10px", "20px", "20px", "20px"]
    advanced:
      css_style: |
        /* 카드 전체 레이아웃 */
        .block-collection .projects-grid {
          display: grid !important;
          grid-template-columns: repeat(3, 1fr) !important;
          gap: 30px !important;
          justify-items: center !important;
        }

        /* 개별 카드 스타일 */
        .block-collection .project-card {
          border-radius: 12px !important;
          overflow: hidden !important;
          box-shadow: 0 4px 12px rgba(0,0,0,0.1) !important;
          transition: all 0.2s ease-in-out !important;
          background: #fff !important;
        }

        /* hover 효과 */
        .block-collection .project-card:hover {
          transform: translateY(-6px) scale(1.02) !important;
          box-shadow: 0 8px 16px rgba(0,0,0,0.2) !important;
        }

        /*카드 내 텍스트 */
        .block-collection .project-card h3 {
          color: #0044cc !important;
          font-weight: 700 !important;
        }

        .block-collection .project-card p {
          color: #555 !important;
          font-size: 0.95rem !important;
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
