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
      text: I mainly work on dimension reduction questions in link with the SIR and the PLS approaches. Recently I started to explore their behaviors in the extremes context.
      # Display content from the `content/publication/` folder
      filters:
        folders:
          - publication
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: citation
---