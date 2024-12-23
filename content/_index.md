---
title: 'Home'
date: 2023-10-24
type: landing

design:
  # Default section spacing
  spacing: "4rem"

# Note: `username` refers to the user's folder name in `content/authors/`

# Page sections
sections:
  - block: biography
    content:
      username: admin
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download Résumé
        url: uploads/resume.pdf
    design:
      #banner:
        # Upload your cover image to the `assets/media/` folder and reference it here
        #filename: IMG20231104165058~2.jpg
      biography:
        # Customize the style of your biography text
        style: 'text-align: justify; font-size: 0.8em;'
  - block: experience
    content:
      username: admin
    design:
      # Hugo date format
      date_format: 'January 2006'
      # Education or Experience section first?
      is_education_first: true
  - block: collection
    id: courses-and-certifications
    content:
      title: Courses and Certifications
      filters:
        folders:
          - courses-and-certifications
    design:
      view: article-grid
      columns: 4
  - block: collection
    id: talks
    content:
      title: Talks
      filters:
        folders:
          - talks
    design:
      view: article-grid
      columns: 2
#  - block: languages
#    content:
#      title: Languages
#      username: admin
---
