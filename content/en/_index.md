---
title: ""
type: landing
view: compact

sections:
  # Main Image Slider
  - block: slider
    content:
      slides:
        - title: "AI Project"
          content: "Omok Artificial Intelligence using Alpha-Beta Search"
          align: center
          background:
            image:
              filename: slide-ai.png 
              filters:
                brightness: 0.6
            position: center
            color: "#ffffffff"

        - title: "Database Project"
          content: "Database Design for a Pet Information & Product Trading Platform"
          align: center
          background:
            image:
              filename: slide-db.jpg 
              filters:
                brightness: 0.45
            position: center
            color: "#ffffffff"

        - title: "Python Project"
          content: "Solving the 8-Puzzle Problem Using Search Algorithms"
          align: center
          background:
            image:
              filename: slide-py.png
              filters:
                brightness: 0.5
            position: center
            color: "#ffffffff"

        - title: "DS Project"
          content: "Data Structure Projects Using Binary Search Trees"
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

  # Project Cards
  #- block: collection
  #  content:
  #    title: "Featured Projects"
  #    subtitle: "AI · Database · Python Projects"
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
  
  # Custom View 1
  - block: collection
    content:
      title: "AI, Ds Projects"
      count: 6
      filters:
        folders:
          - ai
          - ds
    design:
      view: compact
      columns: 3


  # Custom View 2
  - block: collection
    content:
      title: "DB, PY Projects"
      count: 6
      filters:
        folders:
          - database
          - python
    design:
      view: overlay
      columns: 3

  # About Me Summary
  - block: markdown
    content:
      title: "About Me"
      text: |
        I am a student in the **Department of Computer and Artificial Intelligence at Jeonbuk National University**,  
        and I have worked on various projects focused on **AI, Database Systems, and Web Service Development**.  
        I enjoy **algorithm design and system structuring** to solve real-world problems.  
        <br><br>
        📫 **Email:** sooobin0304@naver.com  
        🌐 **GitHub:** [sooobin34](https://github.com/sooobin34)
    design:
      alignment: center
      background:
        color: "#a8c1caff"
---
