---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: About
      username: shahzaib-kashif

  - block: collection
    content:
      title: Publications
      text: |-
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
      
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: RISC-V
          tag: RISC-V
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
    
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Research Assistant
          company: Microelectronics Research Lab (MERL)
          company_url: 'https://merledupk.org/'
          date_start: '2022-09-01'
          date_end: ''
        - title: RISC-V CPU Logic Implementor (CHISEL)
          company: Intensivate
          company_url: 'http://intensivate.com/'
          date_start: '2022-10-01'
          date_end: ''
        - title: Research Intern
          company: Microelectronics Research Lab (MERL)
          company_url: 'https://merledupk.org/'
          date_start: '2019-09-01'
          date_end: '2022-09-01'
    design:
      columns: '2'
  
---
