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

  # Volunteering – added as its own block
  - block: resume-experience
    content:
      title: Volunteering
      username: admin
      sections:
        - volunteering

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
