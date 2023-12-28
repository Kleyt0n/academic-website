---
# Leave the homepage title empty to use the site title
title: ' '
date: 2023-12-09
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: About
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Machine Learning Researcher
          company: Holistic AI
          company_url: 'https://holisticai.com'
          company_logo: 
          location: London, UK
          date_start: '2021-08-01'
          date_end: ''
          description: Building tools and methods to make AI more responsible in main two areas - bias measuring & mitigation and explainability     
        - title: Researcher
          company: ExACTa (PUC-Rio)
          company_url: 'https://www.exacta.inf.puc-rio.br/'
          company_logo: 
          location: Rio de Janeiro, Brazil
          date_start: '2023-03-01'
          date_end: ''
          description: Implementing anomaly detection in oil wells using unsupervised algorithms
        - title: Data Scientist
          company: State Government of Rio de Janeiro
          company_url: 'https://www.rj.gov.br/'
          company_logo: 
          location: Rio de Janeiro, Brazil
          date_start: '2022-01-01'
          date_end: '2023-03-01'
          description: Advising the State Government of Rio de Janeiro on data science projects
    design:
      columns: '2'
  - block: collection
    id: research
    content:
      title: Research
      text: ''
      count: 4
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: posts
    content:
      title: Posts
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 4
      # Filter on criteria
      filters:
        folders:
          - post
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
      columns: '2'
  - block: portfolio
    id: projects
    content:
      title: Open-source
      subtitle: 'Our research has the goal of being open-source and reproducible. Check out some of individial and co-authored projects. I am pythonist, so most of them are written in Python.'
      text: 'Filter by tags:'
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
        - name: Graph Neural Networks
          tag: Graph Neural Networks
        - name: Responsible AI
          tag: Responsible AI
        - name: Optimization
          tag: Optimization
        - name: Computational Geometry
          tag: Computational Geometry
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
---
