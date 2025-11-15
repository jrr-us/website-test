---
# Leave the homepage title empty to use the site title
title: 'My Title'
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: jrr
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      # Apply a gradient background
      css_class: hbx-bg-gradient
      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: resume-biography
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: 'Esto es otra prueba'
      # Show a call-to-action button under your biography? (optional)
      headings:
        about: 'Prueba de about'
        education: 'Prueba de education'
        interests: ''
    design:
      # Apply a gradient background
      css_class: hbx-bg-gradient
      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: markdown
    content:
      title: '📚 My Research v2'
      subtitle: 'Test de bloque markdown'
      text: |-
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. In sit amet varius ex. Aenean vel lacus aliquet, ultricies eros non, ultricies lorem. Nam vel libero sed justo pharetra bibendum ut vitae neque. Duis vel libero nulla. Mauris mollis vitae ipsum eu fermentum. Nullam tempor purus eget suscipit varius. Donec gravida tellus a quam porta, non tempor nisi faucibus. Fusce non nibh sapien. In a convallis erat, sit amet euismod mauris. Pellentesque vitae commodo mi. Proin sed justo enim. Nullam interdum nulla eget quam vehicula egestas. Aenean eleifend nisi in mattis iaculis. Maecenas cursus massa quis ipsum congue, dapibus suscipit tortor hendrerit. Sed vestibulum congue auctor. Ut ut tortor molestie, euismod ligula in, cursus mauris.

        Vestibulum eleifend, mauris at tincidunt ullamcorper, nisl arcu facilisis libero, at efficitur libero elit at lorem. Phasellus tempor dapibus risus aliquet commodo. Vivamus egestas elementum ante pellentesque consequat. Mauris tellus augue, suscipit id euismod vitae, molestie nec augue. Fusce tempor velit eu sem bibendum, ac faucibus arcu aliquet. Morbi vestibulum, tellus eu dapibus ultrices, ante dolor viverra arcu, nec sodales metus mi id neque. Vestibulum ex ante, tristique fringilla facilisis non, finibus id odio. Morbi a augue sit amet erat faucibus auctor eu vel lectus. Nunc non mollis sapien. Quisque laoreet est eget ligula suscipit, et mollis magna efficitur.

        |-
        Aenean luctus fringilla ultricies. Curabitur tincidunt, libero non vehicula accumsan, enim orci ultrices dui, a cursus massa libero non odio. Aenean tincidunt convallis condimentum. Nam volutpat quam imperdiet, laoreet tortor et, euismod nibh. Proin volutpat urna nibh, fermentum auctor nisl consequat ut. Nullam sed rutrum lorem. Vivamus eu enim dignissim, tempor risus at, placerat metus. In non porttitor turpis, id accumsan eros. Quisque ornare nec turpis sit amet pharetra. Morbi in rutrum lacus. Integer tempor, lectus quis convallis maximus, lectus purus eleifend est, id tristique elit purus ut arcu. Interdum et malesuada fames ac ante ipsum primis in faucibus.
    design:
      columns: '2'
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Recent Publications
      text: ''
      filters:
        folders:
          - publication
        year: 2022
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - events
    design:
      view: card
  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: blog
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: card
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
  - block: cta-card
    demo: true # Only display this section in the Hugo Blox Builder demo site
    content:
      title: 👉 Build your own academic website like this
      text: |-
        This site is generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 250,000+ academics like you.

        <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">Star</a>

        Easily build anything with blocks - no-code required!

        From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.
      button:
        text: Get Started
        url: https://hugoblox.com/templates/
    design:
      card:
        # Card background color (CSS class)
        css_class: 'bg-primary-300 dark:bg-primary-700'
        css_style: ''
---
