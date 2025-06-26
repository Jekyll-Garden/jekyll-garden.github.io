# Subdomain Configuration

## For Subdomains (e.g., notes.example.com)
```yaml
url: "https://notes.example.com"
baseurl: ""
```

## For Subdirectories (e.g., example.com/notes)
```yaml
url: "https://example.com"
baseurl: "/notes"
```

## How it works
- `site.url` is used for absolute URLs (canonical links, RSS feeds, etc.)
- `site.baseurl` is prepended to internal links
- For subdomains, use empty `baseurl`
- For subdirectories, use the path as `baseurl`

## Examples in templates
- Internal links: `{{ site.baseurl }}/notes`
- Absolute URLs: `{{ site.url }}/feed.xml`
- Canonical links: `{{ site.url }}{{ page.url }}` 