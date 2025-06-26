---
title: Getting Started
feed: show
date: 2024-01-15
---

# Getting Started with Jekyll Garden

Jekyll Garden makes it incredibly easy to publish your Obsidian vault as a beautiful website. Here's how to get started in just a few steps.

## Step 1: Get the Theme

You have three options:

### Option A: Fork the Repository
1. Visit the [Jekyll Garden repository](https://github.com/Jekyll-Garden/jekyll-garden.github.io)
2. Click "Use this template" or "Fork"
3. Name your repository `yourusername.github.io` for GitHub Pages

### Option B: Clone and Customize
```bash
git clone https://github.com/Jekyll-Garden/jekyll-garden.github.io.git
cd jekyll-garden.github.io
```

### Option C: Use as a Jekyll Theme
Add to your `Gemfile`:
```ruby
gem "jekyll-garden"
```

## Step 2: Configure Your Site

Edit `_config.yml` with your information:

```yaml
# Site Configuration
title: "Your Digital Garden"
heading: "Your Name"
description: "A brief description of your site"
bio: "A longer bio about yourself and what you do."
url: "https://yoursite.com"
email: "hello@yoursite.com"

# Menu Items
menu:
  - title: "Notes"
    url: "/notes"
  - title: "About"
    url: "/about"
  - title: "Blog"
    url: "/blog"
```

## Step 3: Add Your Notes

1. **Create notes** in the `_notes` folder
2. **Add front matter** to each note:

```yaml
---
title: "Your Note Title"
date: 2024-01-15
feed: "show"  # or "hide" to exclude from feeds
---
```

3. **Use wiki links** to connect ideas: `[[Another Note]]`

## Step 4: Deploy

### GitHub Pages (Recommended)
1. Push your changes to GitHub
2. Go to repository Settings → Pages
3. Set source to "Deploy from a branch"
4. Choose your main branch

### Local Development
```bash
bundle install
bundle exec jekyll serve
```

### Other Platforms
- **Netlify**: Connect your repository
- **Vercel**: Import your repository
- **Any static hosting**: Run `bundle exec jekyll build`

## What's Next?

- Learn about [[Wiki Links Explained]]
- See [[Markdown Examples]] for formatting
- Explore [[Customization Guide]] for theming
- Check out [[Search and Navigation]] features

## Tips for Success

- **Start small**: Add a few notes first to see how it works
- **Use descriptive titles**: They become your URLs and link targets
- **Link liberally**: The more connections, the better your garden grows
- **Keep it simple**: Focus on content, not complex formatting

---

*Your digital garden is ready to grow! 🌱* 