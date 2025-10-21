---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: /uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      # Apply a gradient background
      css_class: hbx-bg-gradient
      # Avatar customization
      avatar:
        size: medium   # small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle  # circle (default), square, rounded

  - block: markdown
    content:
      title: '🏛️ My Mission'
      subtitle: ''
      text: |-
    
        My mission is to **lead and build AI systems that are ethical, explainable, and impactful**, transforming how organizations use data to make better, more responsible decisions.  

        As an **educator and international speaker**, I’m passionate about **democratizing technology** through inclusion and knowledge-sharing. I founded **Vem ser Dev** to empower Portuguese-speaking learners in Python and data science.

        Through my talks and collaborations, I aim to **bridge the gap between complex AI systems and human understanding**, inspiring teams and audiences to use data for good.  

        📩 *Open to collaboration, speaking engagements, and initiatives that drive ethical innovation.*  

        **So, what can data do for you?**
    design:
      columns: '1'

  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - events
    design:
      view: card

#  - block: markdown
#  content:
#    title: "💬 What People Say"
#    subtitle: ""
#    text: |-
#      > “Debs’ wisdom and authenticity at the SHPE Convention were truly inspiring.  
#      > Her insights on career growth and navigating challenges resonated deeply. This is a talk that stays with you.”  
#      >
#      > — *"Darwing Vargas, SHPE 2024 Attendee"*
#  design:
#    columns: '1'

- block: testimonial
  content:
    title: "What People Say"
    items:
      - text: "Debs’ wisdom and authenticity at the SHPE Convention were truly inspiring. Her insights on career growth and navigating challenges resonated deeply. This is a talk that stays with you."
        author: "Darwing Vargas, SHPE 2024 Attendee"
        organization:  "Career Assistant,  Rensselaer Polytechnic Institute"



  - block: collection
    id: publications
    content:
      title: Publications
      filters:
        folders:
          - publications
        # featured_only: true   # uncomment if you only want featured items
    design:
      view: article-grid
      columns: 2
---
