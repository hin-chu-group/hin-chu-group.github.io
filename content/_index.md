---
title: ''
summary: 'Researching emerging viruses at the University of Hong Kong'
date: 2026-09-26
type: landing
sections:
  - block: dev-hero
    id: hero
    content:
      username: group
      greeting: 'Welcome to the'
      show_status: false
      show_scroll_indicator: true
      typewriter:
        enable: true
        prefix: 'Understanding'
        strings:
          - 'emerging viruses'
          - 'virus–host interactions'
          - 'viral pathogenesis'
          - 'new antiviral strategies'
        type_speed: 58
        delete_speed: 32
        pause_time: 2600
      cta_buttons:
        - text: Explore our research
          url: '#projects'
          icon: arrow-down
        - text: Meet the people
          url: 'people/'
          icon: users
    design:
      style: centered
      avatar_shape: circle
      animations: true
      background:
        color:
          light: '#f7faf9'
          dark: '#081016'
      spacing:
        padding: ['6rem', '0', '4rem', '0']
  - block: portfolio
    id: projects
    content:
      title: 'Research at the virus–host interface'
      subtitle: 'From mechanisms of infection to strategies for intervention'
      count: 3
      filters:
        folders:
          - projects
      buttons:
        - name: All themes
          tag: '*'
        - name: Virus entry
          tag: Virus entry
        - name: Pathogenesis
          tag: Pathogenesis
        - name: Antivirals
          tag: Antivirals
      default_button_index: 0
    design:
      columns: 3
      background:
        color:
          light: '#ffffff'
          dark: '#0c151a'
      spacing:
        padding: ['4rem', '0', '4rem', '0']
  - block: collection
    id: news
    content:
      title: 'Latest research highlights'
      subtitle: 'Selected updates from HKU and HKUMed'
      filters:
        folders:
          - blog
        exclude_featured: false
      count: 3
      order: desc
    design:
      view: card
      columns: 3
      background:
        color:
          light: '#f2f7f6'
          dark: '#081016'
      spacing:
        padding: ['4rem', '0', '4rem', '0']
  - block: contact-info
    id: contact
    content:
      title: 'Join the conversation'
      subtitle: 'Collaborations and opportunities'
      text: |-
        We welcome enquiries from prospective postdoctoral fellows, MPhil/PhD students,
        research assistants and collaborators. Applicants can send a cover letter
        describing their research interests and a CV to Professor Hin Chu.
      email: hinchu@hku.hk
      autolink: true
    design:
      columns: '1'
      background:
        color:
          light: '#ffffff'
          dark: '#0c151a'
      spacing:
        padding: ['4rem', '0', '5rem', '0']
---
