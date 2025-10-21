---
title: 'Experience'
date: 2023-10-24
type: landing

design:
  spacing: '5rem'

sections:
  # Experience (work/education) – your existing block
  - block: resume-experience
    content:
      title: Experience
      username: admin
      sections:
        - work
        - education
    design:
      date_format: 'January 2006'
      is_education_first: false

  # Skills & Hobbies
  - block: resume-skills
    content:
      title: Skills & Hobbies
      username: admin
    design:
      show_skill_percentage: false

  # Volunteering (markdown block)
  - block: markdown
    content:
      title: 'Volunteering'
      text: |-
        - **Workshop Presenter and Moderator**, *Women in Tech / Latinas in Tech*  
          *2023–Present*  
          Facilitates sessions that promote inclusion and professional growth in tech.

        - **Founder**, *Vem ser Dev — Python direto ao ponto*  
          *2020–Present*  
          Created an education initiative to teach Python and data science to Portuguese-speaking learners.

        - **Internship Program Lead**, *Capital One Data Science Program*, **LAUNCH Program**  
          *2022–Present*  
          Mentors students and early-career professionals; designs applied AI learning experiences.
    design:
      columns: '1'

  # Awards
  - block: resume-awards
    content:
      title: Awards
      username: admin

  # Languages
  - block: resume-languages
    content:
      title: Languages
      username: admin
---
