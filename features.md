# Jekyll Garden Features

## Core Features (Implemented)

### 1. Obsidian Integration
- Publish Obsidian vault notes as a Jekyll static website
- Automatic front matter processing
- Support for `_notes` collection

### 2. Wiki-style Linking
- `[[note title]]` syntax for internal links
- `[[link text::https://example.com]]` for external links
- Automatic link conversion and validation
- Tooltips on hover for internal links (configurable)
- Stale link detection for broken wiki links

### 3. Search Functionality
- Full-text search powered by Lunr.js
- Search through titles and content
- Real-time search results with highlighting
- Keyboard shortcuts (Shift+S to focus search)
- Configurable search toggle

### 4. Navigation & Layout
- Responsive navigation with hamburger menu
- Dynamic menu from config
- Static homepage with custom HTML
- Notes listing page with search
- About page and 404 page

### 5. Theme & Design
- Dark/light theme toggle with persistent preference
- Clean, minimal design inspired by hiran.in
- CSS custom properties for easy customization
- Responsive design for all devices
- Typography-focused layout

### 6. Content Features
- Backlinks showing which notes link to current note (configurable)
- Math rendering with KaTeX support
- Markdown support with extended syntax
- Code syntax highlighting
- Tables, blockquotes, and other markdown elements

### 7. Technical Features
- RSS feed generation (jekyll-feed)
- Sitemap generation (jekyll-sitemap)
- SEO optimization (jekyll-seo-tag)
- Docker support for easy deployment
- Subdomain and subdirectory support

## Configuration Options (Implemented)

### Site Configuration
- Site title, heading, description, and bio
- URL and baseurl for subdomain/subdirectory support
- Email for contact functionality
- Copyright information

### Menu & Navigation
- Dynamic menu items from config
- Responsive navigation structure
- Logo and favicon support

### Preferences (Feature Toggles)
- Homepage enabled/disabled
- Search functionality toggle
- Backlinks display toggle
- Page preview tooltips toggle
- Wiki-style link processing toggle

### Content Management
- Notes collection with custom permalinks
- Front matter defaults for notes
- Feed visibility control per note
- List format support for notes

### Assets & Branding
- SVG favicon and Open Graph image
- PWA icons (192x192, 512x512)
- Brand color customization via CSS variables

## Technical Implementation

### Jekyll Setup
- Jekyll 4.0+ compatibility
- Collections for notes management
- Liquid templating for dynamic content
- YAML front matter processing

### Frontend
- Custom CSS with CSS custom properties
- JavaScript for search functionality
- Theme toggle with localStorage
- Responsive design with CSS Grid/Flexbox

### Search Implementation
- Lunr.js for client-side search
- SearchData.json generation
- Real-time search with debouncing
- Keyboard navigation support

### Deployment Options
- GitHub Pages support
- Docker containerization
- Local development server
- Static site generation

## Features Removed/Not Implemented

### Removed for Simplicity
- Related posts display
- Bulma CSS framework (replaced with custom CSS)
- Flashcards feature
- Boxed callouts
- Sidenotes feature
- Newsletter subscription
- Contact form integration
- Social media integration
- Analytics integration
- Comment system integration
- PWA features (except icons)
- Performance optimization settings
- Security headers
- Accessibility features
- Print styles

### Configuration Removed
- Featured sections (replaced with menu)
- Call-to-action buttons
- Navigation array (replaced with menu)
- All optional features (analytics, comments, etc.)

## Design Philosophy

- **Minimal**: Focus on content over features
- **Fast**: Lightweight and performant
- **Customizable**: Easy to modify and extend
- **Obsidian-friendly**: Works seamlessly with Obsidian workflow
- **Static-first**: No server-side dependencies