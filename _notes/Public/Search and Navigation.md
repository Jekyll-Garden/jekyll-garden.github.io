---
title: Search and Navigation
feed: show
date: 2024-01-15
---

# Search and Navigation in Jekyll Garden

Jekyll Garden provides powerful tools to help you find and navigate through your digital garden. Here's how to make the most of them.

## Search Feature

### How to Use Search
1. **Click the search icon** in the navigation bar (or press `Ctrl/Cmd + K`)
2. **Type your query** - search works across note titles and content
3. **Browse results** - see matching notes with highlighted text
4. **Click to visit** any result to jump directly to that note

### Search Tips
- **Partial matches work**: Type "wiki" to find "Wiki Links Explained"
- **Case insensitive**: "Getting" finds "Getting Started"
- **Instant results**: Results update as you type
- **Keyboard navigation**: Use arrow keys and Enter to navigate results

### What Gets Indexed
- Note titles
- Note content
- Wiki link text
- Code comments (in some cases)

## Navigation Options

### 1. Menu Navigation
The main menu (configured in `_config.yml`) provides quick access to key pages:
- **Notes**: Browse all published notes
- **About**: Static information page
- **Blog**: Traditional blog posts (if enabled)

### 2. Notes Feed
The [[Notes]] page shows all your published notes in chronological order. This is your main content hub.

### 3. Wiki Link Navigation
The most powerful navigation method is through wiki links:
- Click any `[[note title]]` to jump to that note
- Use backlinks to discover related content
- Follow link chains to explore topics

### 4. Browser Navigation
- **Back/Forward**: Works normally with wiki links
- **Bookmarks**: Bookmark any note for quick access
- **URLs**: Share direct links to specific notes

## Organizing Your Garden

### Content Structure
```
_notes/
├── Public/           # Published notes
│   ├── Getting Started.md
│   ├── Wiki Links Explained.md
│   └── Markdown Examples.md
├── Private/          # Private notes (not published)
└── Drafts/           # Work in progress
```

### Note Categories
Consider organizing notes by type:
- **Guides**: [[Getting Started]], [[Wiki Links Explained]]
- **References**: [[Markdown Examples]], [[Search and Navigation]]
- **Projects**: [[Project Ideas]], [[Work Notes]]
- **Personal**: [[About Me]], [[Reading List]]

### Front Matter Options
Control how notes appear and behave:

```yaml
---
title: "Your Note"
date: 2024-01-15
feed: "show"          # Show in notes feed
permalink: "/custom-url"  # Custom URL
format: "list"        # List layout for collections
---
```

## Advanced Navigation

### Link Previews
Hover over wiki links to see a preview of the linked note's content. This helps you decide whether to click through.

### Related Notes
Some notes automatically suggest related content based on shared links and topics.

### Search Filters
While the current search is full-text, you can use specific terms to narrow results:
- Search for "guide" to find how-to notes
- Search for "example" to find reference material
- Search for note titles to jump directly to them

## Mobile Navigation

### Touch-Friendly
- Large touch targets for links
- Swipe gestures work normally
- Search is accessible on mobile
- Responsive design adapts to screen size

### Mobile Tips
- Use the search feature for quick navigation
- Bookmark frequently visited notes
- Consider creating hub notes for mobile users

## Customization

### Search Configuration
In `_config.yml`:
```yaml
preferences:
  search:
    enabled: true
```

### Navigation Customization
- Modify menu items in `_config.yml`
- Add custom navigation in layouts
- Create landing pages for topics

## Troubleshooting

### Search Not Working
1. Check that search is enabled in preferences
2. Ensure notes have `feed: "show"`
3. Rebuild your site to update the search index

### Missing Notes
1. Verify notes are in the `_notes` folder
2. Check that `feed: "show"` is set
3. Ensure proper front matter syntax

### Broken Navigation
1. Check wiki link syntax: `[[Note Title]]`
2. Verify note titles match exactly
3. Rebuild site after adding new notes

---

*Good navigation makes your digital garden a joy to explore.* 