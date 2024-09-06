---
# Leave the homepage title empty to use the site title
title: ""
date: 2024-09-01
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      #button:
      #  text: Download CV
      #  url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: amu2.jpg
          filters:
            brightness: 0.9
          size: cover
          position: center
          parallax: false
---

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Markmap Example</title>
  <script src="https://cdn.jsdelivr.net/npm/markmap-autoloader"></script>
</head>
<body>
  <pre>
  # Exemple
  - Node 1
    - Subnode 1.1
  - Node 2
    - Subnode 2.1
  </pre>
</body>
</html>