---
title: "Welcome to Jekyll Garden"
date: 2024-01-15
categories: [jekyll, digital-garden]
tags: [introduction, setup]
---

# Welcome to Jekyll Garden

Jekyll Garden isn't just for notes - it's also a great platform for traditional blogging. This post demonstrates how you can use Jekyll Garden for both digital gardening and regular blog posts.

## What is Jekyll Garden?

Jekyll Garden is a clean, minimal Jekyll theme that makes publishing your Obsidian vault as a static website incredibly easy. It combines the best of both worlds:

- **Digital Garden features**: Wiki-style linking, backlinks, and connected knowledge
- **Traditional blogging**: Chronological posts, categories, and tags
- **Simple setup**: Just add markdown files and you're ready to go

## Why Use Jekyll Garden for Blogging?

### 1. Simplicity
No complex setup required. Just write markdown and publish.

### 2. Speed
Static sites are fast and reliable. No database or server maintenance needed.

### 3. Flexibility
Use it for notes, blog posts, or both. The choice is yours.

### 4. SEO Friendly
Clean URLs, fast loading, and search engine optimized out of the box.

## Getting Started

1. **Fork the repository** from GitHub
2. **Configure your site** in `_config.yml`
3. **Add your content** to `_notes` (for garden) or `_posts` (for blog)
4. **Deploy** to GitHub Pages, Netlify, or any static hosting

## Blog vs Garden

### Blog Posts (`_posts/`)
- Chronological order
- Categories and tags
- Traditional blog layout
- Good for time-sensitive content

### Garden Notes (`_notes/`)
- Connected by wiki links
- Backlinks and relationships
- Evergreen content
- Perfect for knowledge management

## Features That Work for Both

- **Markdown support**: Write in your favorite format
- **Search functionality**: Find content quickly
- **Responsive design**: Works on all devices
- **Dark/light theme**: User preference support
- **Fast loading**: Optimized for performance

## Example Blog Structure

```
_posts/
├── 2024-01-15-welcome-to-jekyll-garden.md
├── 2024-01-20-how-to-use-wiki-links.md
└── 2024-01-25-customizing-your-garden.md

_notes/
├── Getting Started.md
├── Wiki Links Explained.md
└── Customization Guide.md
```

## Writing Your First Post

Create a new file in `_posts/` with the format `YYYY-MM-DD-title.md`:

```markdown
---
title: "Your Post Title"
date: 2024-01-15
categories: [category1, category2]
tags: [tag1, tag2]
---

# Your Post Title

Your content here...
```

## Linking Between Posts and Notes

You can link between blog posts and garden notes using wiki links:

- Link to a note: `[[Getting Started]]`
- Link to a post: `[[Welcome to Jekyll Garden]]`
- External links: `[[External Site::https://example.com]]`

## Categories and Tags

Organize your blog posts with categories and tags:

```yaml
---
title: "Post Title"
date: 2024-01-15
categories: [jekyll, tutorial]
tags: [setup, guide, beginner]
---
```

## Conclusion

Jekyll Garden gives you the best of both worlds - a powerful digital garden for your knowledge base and a clean blog for your thoughts and updates. Whether you're writing evergreen notes or time-sensitive posts, Jekyll Garden has you covered.

Start building your digital presence today with Jekyll Garden!

---

*This post demonstrates traditional blogging with Jekyll Garden. For more information about digital gardening features, check out the [[Getting Started]] guide.* 