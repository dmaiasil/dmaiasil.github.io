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
          Leads workshops on career growth and professional development in tech.

        - **Mentor**, *HIT (Hispanics in Tech) Mentorship cohorts*  
          *2024–2026*

        - **Mentor**, *OutFront Mentorship Cohort*  
          *2024–2026*

        - **Educator**, *Data Science & Machine Learning for Portuguese Speakers*  
          *2020–Present*  
          Creates educational content to bring high-quality data science and machine learning to Portuguese speakers.

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
