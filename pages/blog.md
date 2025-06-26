---
title: "Blog"
content-type: "static"
---

# Blog

Welcome to the blog section of Jekyll Garden. Here you'll find traditional blog posts alongside the digital garden notes.

## Recent Posts

{% raw %}
{% for post in site.posts limit:5 %}
<div class="post-preview">
  <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
  <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
  {% if post.categories %}
  <p class="post-categories">Categories: {{ post.categories | join: ", " }}</p>
  {% endif %}
  {% if post.tags %}
  <p class="post-tags">Tags: {{ post.tags | join: ", " }}</p>
  {% endif %}
  <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
</div>
{% endfor %}
{% endraw %}

## All Posts

{% raw %}
{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}
{% endraw %}

## Categories

{% raw %}
{% for category in site.categories %}
### {{ category[0] | capitalize }}
{% for post in category[1] %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}
{% endfor %}
{% endraw %}

## About This Blog

This blog demonstrates how Jekyll Garden can be used for traditional blogging alongside digital gardening. Blog posts are stored in the `_posts` folder and follow standard Jekyll conventions.

### Blog vs Garden

- **Blog Posts** (`_posts/`): Chronological, time-sensitive content
- **Garden Notes** (`_notes/`): Evergreen, interconnected knowledge

### Writing Blog Posts

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

### Linking Between Posts and Notes

You can link between blog posts and garden notes using wiki links:

- Link to a note: `[[Getting Started]]`
- Link to a post: `[[Welcome to Jekyll Garden]]`
- External links: `[[External Site::https://example.com]]`

---

*This blog section shows how Jekyll Garden supports both traditional blogging and digital gardening in one platform.* 