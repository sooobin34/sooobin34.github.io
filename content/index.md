---
title:
date: 2022-10-24
type: landing

sections:
  - block: hero
    content:
      title: |
        안수빈의 포트폴리오
      image:
        filename: welcome.jpg
      text: |
        <br>
        전북대학교 컴퓨터인공지능학부  
        **Database · Algorithm · AI Project Portfolio**
  
  - block: collection
    content:
      title: 📂 My Projects
      subtitle: "AI, Database, Algorithm Projects"
      text: "학부 프로젝트들을 카드 형태로 정리했습니다."
      count: 9
      filters:
        folders:
          - project        # <- 프로젝트 폴더를 불러옴
        author: ''
        category: ''
        tag: ''
        publication_type: ''
        exclude_featured: false
      order: desc
    design:
      view: card
      columns: '3'         # ✅ 가로 3개 × 세로 3줄 → 총 9개 카드
      background:
        color: 'none'

  - block: markdown
    content:
      title: ''
      text: |
        {{% cta cta_link="./contact/" cta_text="📧 연락하기 →" %}}
    design:
      columns: '1'
---
