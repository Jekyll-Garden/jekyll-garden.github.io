---
title: Wiki Links Explained
feed: show
date: 2024-01-15
---

# Wiki Links: The Heart of Your Digital Garden

Wiki links are what make Jekyll Garden special. They allow you to create a connected web of knowledge, just like in Obsidian, but on the web.

## What are Wiki Links?

Wiki links use double brackets `[[note title]]` to create internal links between your notes. They're the foundation of a digital garden - connecting ideas and creating a web of knowledge.

## How to Use Wiki Links

### Basic Syntax
```markdown
This note relates to [[Getting Started]] and [[Markdown Examples]].
```

### With Custom Text
```markdown
Check out [[this guide::Getting Started]] for setup instructions.
```

### External Links
```markdown
Read more at [[this article::https://example.com/article]].
```

## See Wiki Links in Action

This note links to:
- [[Getting Started]] - How to set up Jekyll Garden
- [[Markdown Examples]] - Complete markdown reference
- [[Welcome to the garden]] - Introduction to the theme

## Automatic Backlinks

When you create a wiki link to another note, that note automatically shows a "Backlinks" section. For example, if you visit [[Getting Started]], you'll see this note listed there because we linked to it.

## Best Practices

### 1. Use Descriptive Titles
```markdown
# Good
[[How to Deploy to GitHub Pages]]

# Avoid
[[Deploy]]
```

### 2. Link Liberally
Don't worry about over-linking. The more connections, the better your garden grows.

### 3. Create Hubs
Some notes can serve as central hubs that link to many related topics.

### 4. Use Consistent Naming
Keep note titles consistent to avoid broken links.

## Common Patterns

### Topic Clusters
Create notes that group related concepts:
- [[Programming Basics]]
- [[Web Development]]
- [[Design Principles]]

### Process Notes
Document workflows and processes:
- [[How to Write a Blog Post]]
- [[Code Review Process]]
- [[Meeting Notes Template]]

### Reference Notes
Build collections of useful information:
- [[Useful Commands]]
- [[Book Notes]]
- [[Project Ideas]]

## Troubleshooting

### Broken Links
If a wiki link appears red or broken:
1. Check the exact spelling of the note title
2. Make sure the note exists in the `_notes` folder
3. Verify the note has `feed: "show"` in its front matter

### Missing Backlinks
If backlinks aren't showing:
1. Ensure the target note is published (`feed: "show"`)
2. Check that the link syntax is correct
3. Rebuild your site

## Advanced Features

### Link Previews
Hover over wiki links to see a preview of the linked note's content.

### Search Integration
Wiki links work seamlessly with the search feature - you can search for note titles and find all references.

### Automatic URL Generation
Note titles automatically become URLs, so `[[My Note]]` links to `/notes/my-note`.

---

*Wiki links transform your notes from isolated documents into a living, connected knowledge base.* 