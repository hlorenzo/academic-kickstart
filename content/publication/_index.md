---
# Page title
title: My page
# Page type - we want a landing page (such as a homepage)
type: landing

# Your landing page sections - add as many different content blocks as you like
sections:
  # A section to display blog posts
  - block: collection
    id: section-1
    content:
      count: 0
      title: Published articles
      text: I mainly work on dimension reduction questions in link with the SIR and the PLS approaches, recently I started to explore their behaviors in the extremes context. I also work on solutions to missing data problems.
      # Display content from the `content/publication/` folder
      filters:
        folders:
          - publication
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: citation
      background:
        # Choose a color such as from https://html-color-codes.info
        color: '#E0F8E0'
        # Text color (true=light, false=dark, or remove for the dynamic theme color).
        #text_color_light: true
---