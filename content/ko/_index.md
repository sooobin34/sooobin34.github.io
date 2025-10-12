---
title: ""
type: landing

sections:
  # ✅ 메인 이미지 슬라이더
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

    design:
      slide_height: "430px"
      is_fullscreen: false
      loop: true
      interval: 3000
    advanced:
      css_style: |
        .slick-prev, .slick-next { display: none !important; }

  # ✅ 프로젝트 카드 (3×3 그리드 강제)
  - block: collection
    content:
      title: "주요 프로젝트"
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
      spacing:
        padding: ["10px", "20px", "20px", "20px"]
    advanced:
      css_style: |
        /* 전체 카드 레이아웃 강제 (3×3) */
        .block-collection .section-body {
          display: grid !important;
          grid-template-columns: repeat(auto-fill, minmax(300px, 1fr)) !important;
          gap: 28px !important;
          justify-items: center !important;
          padding-top: 20px !important;
        }

        /* 개별 카드 박스 스타일 */
        .block-collection article {
          background: #fff !important;
          border-radius: 14px !important;
          box-shadow: 0 4px 14px rgba(0,0,0,0.1) !important;
          overflow: hidden !important;
          transition: all 0.25s ease !important;
          width: 100% !important;
          max-width: 360px !important;
          display: flex !important;
          flex-direction: column !important;
          justify-content: space-between !important;
        }

        /* 이미지 */
        .block-collection article img {
          width: 100% !important;
          height: 210px !important;
          object-fit: cover !important;
          border-bottom: 1px solid #ddd !important;
        }

        /* hover 효과 */
        .block-collection article:hover {
          transform: translateY(-6px) scale(1.02) !important;
          box-shadow: 0 8px 18px rgba(0,0,0,0.2) !important;
        }

        /* 텍스트 꾸미기 */
        .block-collection article h3 {
          font-size: 1.15rem !important;
          font-weight: 700 !important;
          color: #0044cc !important;
          padding: 14px 18px 6px !important;
        }

        .block-collection article p {
          font-size: 0.95rem !important;
          color: #444 !important;
          padding: 0 18px 18px !important;
        }

        /* 카드 간격 정리 */
        .block-collection .article-style {
          margin: 0 !important;
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
