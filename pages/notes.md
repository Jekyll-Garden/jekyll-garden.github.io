---
layout: Post
permalink: /notes
feedformat: card
title: "Notes"
---

# Digital Garden Notes

Welcome to the digital garden. Here you'll find interconnected notes that grow and evolve over time. Unlike traditional blogs, these notes are organized by connections rather than chronology.

## Featured Notes

- [[Welcome to the garden]] - Introduction to Jekyll Garden
- [[Getting Started]] - How to set up your own digital garden
- [[Wiki Links Explained]] - Understanding wiki-style linking
- [[Markdown Examples]] - Complete markdown reference
- [[Search and Navigation]] - How to find and organize content
- [[Customization Guide]] - Personalizing your garden

## All Notes

{% raw %}
{% for note in site.notes %}
{% if note.feed == "show" %}
- [{{ note.title }}]({{ note.url }}) - {{ note.date | date: "%B %d, %Y" }}
{% endif %}
{% endfor %}
{% endraw %}

## About Digital Gardens

A digital garden is a collection of interconnected notes that grow and evolve over time. Think of it as your personal Wikipedia - a living knowledge base that you can share with the world.

### Key Features

- **Wiki-style Links**: Use `[[note title]]` to connect ideas
- **Automatic Backlinks**: See which notes link to the current one
- **Evergreen Content**: Knowledge that doesn't expire
- **Searchable**: Find content quickly across all notes

### How to Navigate

- **Browse chronologically**: See notes in the order they were created
- **Follow links**: Click any `[[wiki link]]` to explore related content
- **Use search**: Find specific content with the search feature
- **Check backlinks**: See what other notes reference the current one

### Writing Your Own Notes

To add notes to your garden:

1. Create a new markdown file in the `_notes` folder
2. Add front matter with title, date, and feed settings
3. Use wiki links to connect to other notes
4. Deploy to see your changes live

Example:
```markdown
---
title: "My New Note"
date: 2024-01-15
feed: "show"
---

# My New Note

This note relates to [[Getting Started]] and [[Wiki Links Explained]].
```

---

*Explore the garden by following links and discovering connections between ideas.*