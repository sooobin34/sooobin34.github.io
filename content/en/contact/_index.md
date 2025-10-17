---
title: Contact
summary: "Ways to get in touch (email, phone, and map)"

image:
  filename: "contact.jpg"

date: 2025-10-16

type: landing

sections:
  - block: contact
    content:
      title: Contact
      email: sooobin0304@naver.com
      phone: +82-10-6206-1173
      address:
        street: 109 Yeoul-ro
        city: Jeonju-si
        region: Jeollabuk-do
        postcode: '54944'
        country: Republic of Korea
        country_code: KR
      coordinates:
        latitude: '35.837016'
        longitude: '127.113356'
      office_hours:
        - 'Monday: 10:00 AM – 1:00 PM'
        - 'Thursday: 10:00 AM – 2:00 PM'
      
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
      text:
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
