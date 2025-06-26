# Jekyll Garden

A clean, minimal Jekyll theme that makes publishing your Obsidian vault as a static website incredibly easy. Jekyll Garden bridges the gap between private knowledge management and public sharing.

## What is Jekyll Garden?

Jekyll Garden is a Jekyll theme designed for digital gardening - a way to publish interconnected notes that grow and evolve over time. Think of it as your personal Wikipedia on the web.

### Key Features

- **Wiki-style Links**: Use `[[note title]]` syntax just like in Obsidian
- **Automatic Backlinks**: See which notes link to the current one
- **Full-text Search**: Find content quickly across all notes
- **Clean Design**: Minimal, typography-focused design
- **Dark/Light Theme**: Toggle between themes with persistent preference
- **Traditional Blogging**: Support for chronological blog posts
- **Math Expressions**: KaTeX support for mathematical content
- **Responsive**: Works beautifully on all devices

## Quick Start

1. **Fork or clone** this repository
2. **Configure** your site in `_config.yml`
3. **Add your notes** to the `_notes` folder
4. **Deploy** to GitHub Pages, Netlify, or any static hosting

## Configuration

### Basic Setup

```yaml
# Site Configuration
title: "Your Digital Garden"
heading: "Your Name"
description: "A brief description of your site"
bio: "A longer bio about yourself and what you do."
url: "https://yoursite.com"
email: "hello@yoursite.com"
```

### Menu Items

```yaml
# Menu Items
menu:
  - title: "Notes"
    url: "/notes"
  - title: "Blog"
    url: "/blog"
  - title: "About"
    url: "/about"
```

### Preferences

```yaml
# Preferences (controls template behavior)
preferences:
  homepage:
    enabled: true
  search:
    enabled: true
  backlinks:
    enabled: true
  pagepreview:
    enabled: true
  wiki_style_link:
    enabled: true
```

## Writing Notes

### Front Matter

Each note should have YAML front matter:

```yaml
---
title: "Your Note Title"
date: 2024-01-15
feed: "show"  # or "hide" to exclude from feeds
---
```

### Wiki Links

Use `[[note title]]` to create internal links:

```markdown
This note relates to [[Another Note]] and [[Yet Another Note]].
```

### External Links

Use `[[link text::https://example.com]]` for external links:

```markdown
Check out [[this article::https://example.com/article]] for more info.
```

## Content Types

### Digital Garden Notes (`_notes/`)

- **Evergreen content**: Knowledge that doesn't expire
- **Interconnected**: Linked through wiki-style connections
- **Backlinks**: Automatic discovery of related content
- **Searchable**: Full-text search across all notes

### Blog Posts (`_posts/`)

- **Chronological**: Time-sensitive content
- **Categories and tags**: Traditional blog organization
- **Standard Jekyll**: Follows Jekyll conventions
- **Hybrid linking**: Can link to garden notes

## Features in Detail

### Wiki-style Linking
- Use `[[note title]]` syntax for internal links
- Automatic URL generation from note titles
- Link previews on hover
- Support for custom link text: `[[custom text::note title]]`

### Search and Navigation
- Full-text search powered by Lunr.js
- Instant search results as you type
- Keyboard navigation support
- Search across titles and content

### Backlinks
- Automatic discovery of incoming links
- See which notes reference the current one
- Configurable display options
- Helps discover related content

### Math Rendering
- KaTeX support for mathematical expressions
- Inline math: `$x = y$`
- Block math: `$$\int_{-\infty}^{\infty} e^{-x^2} dx = \sqrt{\pi}$$`

### Responsive Design
- Mobile-first approach
- Touch-friendly navigation
- Adaptive layouts for all screen sizes
- Fast loading on all devices

## Deployment

### GitHub Pages

1. Push your site to a GitHub repository
2. Enable GitHub Pages in repository settings
3. Set source to "Deploy from a branch"
4. Choose your main branch

### Netlify

1. Connect your repository to Netlify
2. Build command: `bundle exec jekyll build`
3. Publish directory: `_site`

### Vercel

1. Import your repository
2. Framework preset: Jekyll
3. Deploy automatically

### Docker

```bash
# Build and run with Docker
docker-compose up -d
```

### Local Development

```bash
# Install dependencies
bundle install

# Start local server
bundle exec jekyll serve

# Build for production
bundle exec jekyll build
```

## Customization

### Visual Customization

The theme uses CSS custom properties for easy theming. Edit `assets/css/style.css`:

```css
:root {
  --primary-color: #007acc;
  --text-color: #333;
  --background-color: #fff;
  --font-family: -apple-system, BlinkMacSystemFont, sans-serif;
}
```

### Layout Customization

- Create custom layouts in `_layouts/`
- Modify existing templates
- Add custom JavaScript and CSS
- Extend with Jekyll plugins

## Use Cases

### Personal Knowledge Base
Share your research, notes, and insights with the world.

### Documentation Site
Create interconnected documentation for projects or organizations.

### Educational Content
Build courses and tutorials with linked concepts.

### Portfolio
Showcase your work and thoughts in a connected way.

### Blog and Garden Hybrid
Combine traditional blogging with digital gardening.

## Examples and Documentation

- **Getting Started**: [[Getting Started]] - Step-by-step setup guide
- **Wiki Links**: [[Wiki Links Explained]] - How to use wiki-style linking
- **Markdown**: [[Markdown Examples]] - Complete markdown reference
- **Search**: [[Search and Navigation]] - Navigation and search features
- **Customization**: [[Customization Guide]] - Theming and configuration

## Contributing

Jekyll Garden is open source and welcomes contributions:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

MIT License - see LICENSE file for details.

## Credits

See [[Credits]] for acknowledgments and contributors.

---

*Jekyll Garden - Where knowledge grows and connects.*
