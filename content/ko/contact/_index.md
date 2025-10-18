---
title: Contact
summary: "연락 방법(이메일,전화번호,지도)"

image:
  filename: "contact.jpg"

date: 2025-10-13

type: landing

sections:
  - block: contact
    content:
      title: Contact
      email: sooobin0304@naver.com
      phone: +82-10-6206-1173
      address:
        street: 여울로 109
        city: 전주시
        region: 전라북도
        postcode: '54944'
        country: 대한민국
        country_code: KO
      coordinates:
        latitude: '35.837016'
        longitude: '127.113356'
      office_hours:
        - '월요일 10:00 to 13:00'
        - '목요일 10:00 to 14:00'
      #contact_links:
      #  - icon: comments
      #    icon_pack: fas
      #    name: Discuss on Forum
      #    link: 'https://discourse.gohugo.io'
    
      # Automatically link email and phone or display as text?
      autolink: true
    
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '1'

  - block: markdown
    content:
      title:
      subtitle: ''
      text: "궁금한 점이 있거나 연락을 원하신다면 아래 정보를 참고해주세요."
    design:
      columns: '1'
      background:
        image: 
          filename: contact.jpg
          filters:
            brightness: 1
          parallax: false
          position: center
          size: cover
          text_color_light: true
      spacing:
        padding: ['20px', '0', '20px', '0']
      css_class: fullscreen
---
