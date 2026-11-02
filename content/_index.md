---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      username: admin
      text: ''
      button:
        text: Download CV
        url: /uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      css_class: hbx-bg-gradient
      avatar:
        size: medium
        shape: circle

  - block: markdown
    content:
      title: '🏛️ My Mission'
      subtitle: ''
      text: |-
        My mission is to **lead and build AI systems that are ethical, explainable, and impactful**, transforming how organizations use data to make better, more responsible decisions.  

        As an **educator and international speaker**, I’m passionate about **democratizing technology** through inclusion and knowledge-sharing. I'm also committed to bringing high-quality data science and machine learning education to Portuguese speakers.  

        Through my talks and collaborations, I aim to **bridge the gap between complex AI systems and human understanding**, inspiring teams and audiences to use data for good.  

        📩 *Open to collaboration, speaking engagements, and initiatives that drive ethical innovation.*  

        **So, what can data do for you?**
    design:
      columns: '1'

  - block: collection
    id: talks
    content:
      title: Featured & Upcoming Talks
      filters:
        folders:
          - events
    design:
      view: article-grid
      columns: 2

  - block: markdown
    content:
      title: "💬 What People Say"
      subtitle: ""
      text: |-
        <div class="testimonials">
          <figure>
            <blockquote>
              “Debs’ wisdom and authenticity at the SHPE Convention were truly inspiring.  
              Her insights on career growth and navigating challenges resonated deeply.  
              This is a talk that stays with you.”
            </blockquote>
            <figcaption>— <strong>Darwing Vargas</strong>, Career Assistant, RPI</figcaption>
          </figure>

          <figure>
            <blockquote>
              “Debs’ talk at the RTC Summit was deeply inspiring. Her authenticity and insights on finding your niche in tech resonated with me, showing how aligning strengths with purpose leads to a more meaningful career in tech.”  
            </blockquote>
            <figcaption>— <strong>Vaishnavi Rajendra Dhotargavi</strong>, Machine Learning Engineer, BulkMagic</figcaption>
          </figure>
        </div>

        <style>
          .testimonials { 
            max-width: 52rem; 
            margin: 2rem auto; 
            padding: 1rem 1.25rem; 
            text-align: center; 
          }
          .testimonials figure { 
            margin: 2rem 0; 
          }
          .testimonials blockquote { 
            font-size: 1.1rem; 
            line-height: 1.7; 
            margin: 0 0 0.75rem; 
            font-style: italic; 
          }
          .testimonials figcaption { 
            font-size: 0.95rem; 
            color: var(--muted, #555); 
          }
        </style>
    design:
      columns: '1'

  - block: cta-card
    content:
      title: "📩 Book a Talk"
      text: "Bring this session to your organization or event."
      button:
        text: "Email Debs for Speaking Engagements"
        url: "mailto:missdmaia@gmail.com"
    design:
      card:
        css_class: 'bg-primary-100 cta-fix'

  - block: collection
    id: publications
    content:
      title: Publications
      filters:
        folders:
          - publications
    design:
      view: article-grid
      columns: 2
---
