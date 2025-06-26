---
title: Customization Guide
feed: show
date: 2024-01-15
---

# Customizing Your Jekyll Garden

Jekyll Garden is designed to be simple yet flexible. Here's how to make it your own.

## Basic Configuration

### Site Settings
Edit `_config.yml` to customize your site:

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
Customize your navigation menu:

```yaml
menu:
  - title: "Notes"
    url: "/notes"
  - title: "About"
    url: "/about"
  - title: "Projects"
    url: "/projects"
  - title: "Blog"
    url: "/blog"
```

## Theme Preferences

### Feature Toggles
Control which features are enabled:

```yaml
preferences:
  homepage:
    enabled: true      # Show custom homepage
  search:
    enabled: true      # Enable search
  backlinks:
    enabled: true      # Show backlinks
  pagepreview:
    enabled: true      # Show link previews
  wiki_style_link:
    enabled: true      # Enable wiki links
```

### Homepage Options
- **Enabled**: Shows content from `pages/index.md`
- **Disabled**: Shows notes feed as homepage

## Visual Customization

### CSS Variables
The theme uses CSS custom properties for easy theming. Edit `assets/css/style.css`:

```css
:root {
  /* Colors */
  --primary-color: #007acc;
  --text-color: #333;
  --background-color: #fff;
  --link-color: #007acc;
  
  /* Typography */
  --font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
  --font-size: 16px;
  --line-height: 1.6;
  
  /* Spacing */
  --container-width: 800px;
  --spacing: 1rem;
}
```

### Dark Mode
The theme includes automatic dark mode support. Users can toggle between light and dark themes, and their preference is saved.

### Custom Fonts
Add custom fonts by modifying the CSS:

```css
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600&display=swap');

:root {
  --font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
}
```

## Layout Customization

### Custom Layouts
Create custom layouts in `_layouts/`:

```html
<!-- _layouts/custom.html -->
---
layout: Post
---
<div class="custom-layout">
  {{ content }}
</div>
```

### Page Templates
Use different layouts for different types of content:

```yaml
---
title: "My Note"
layout: Post          # Default note layout
# layout: custom      # Custom layout
---
```

## Content Organization

### Note Categories
Organize notes using folders:

```
_notes/
├── Guides/           # How-to guides
├── Projects/         # Project notes
├── Reference/        # Reference material
└── Personal/         # Personal notes
```

### Front Matter Options
Control how notes appear:

```yaml
---
title: "Note Title"
date: 2024-01-15
feed: "show"          # Show in feed
# feed: "hide"        # Hide from feed
permalink: "/custom-url"  # Custom URL
format: "list"        # List layout
---
```

## Advanced Customization

### Custom JavaScript
Add custom scripts in `assets/js/`:

```javascript
// assets/js/custom.js
document.addEventListener('DOMContentLoaded', function() {
  // Your custom code here
});
```

### Custom CSS
Add custom styles:

```css
/* assets/css/custom.css */
.custom-class {
  /* Your styles */
}
```

### Plugin Integration
Jekyll Garden supports standard Jekyll plugins:

```yaml
plugins:
  - jekyll-feed
  - jekyll-sitemap
  - jekyll-seo-tag
  - jekyll-paginate
```

## Deployment Options

### GitHub Pages
1. Push to GitHub repository
2. Enable Pages in repository settings
3. Set source to main branch

### Netlify
1. Connect your repository
2. Build command: `bundle exec jekyll build`
3. Publish directory: `_site`

### Vercel
1. Import your repository
2. Framework preset: Jekyll
3. Deploy automatically

### Custom Domain
Add your domain in `_config.yml`:

```yaml
url: "https://yourdomain.com"
```

## Performance Optimization

### Image Optimization
- Use WebP format when possible
- Optimize images before uploading
- Consider lazy loading for large images

### Code Optimization
- Minify CSS and JavaScript
- Enable compression on your server
- Use CDN for external resources

## Troubleshooting

### Common Issues
1. **Changes not appearing**: Rebuild your site
2. **Broken links**: Check wiki link syntax
3. **Styling issues**: Clear browser cache
4. **Search not working**: Check search index

### Debug Mode
Enable debug mode in `_config.yml`:

```yaml
debug: true
```

## Best Practices

### Keep It Simple
- Focus on content over complex styling
- Use consistent naming conventions
- Regular backups of your content

### Performance
- Optimize images and assets
- Minimize external dependencies
- Test on different devices

### Accessibility
- Use semantic HTML
- Provide alt text for images
- Ensure good color contrast

---

*Customization should enhance your content, not distract from it.* 