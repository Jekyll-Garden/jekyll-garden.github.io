---
title: Markdown Examples
feed: show
date: 2024-01-15
---

# Complete Markdown Reference

This page shows all the markdown features supported by Jekyll Garden. Use this as a reference when writing your notes.

## Table of Contents

* TOC
{:toc}

## Headings

```markdown
# H1 Heading
## H2 Heading
### H3 Heading
#### H4 Heading
##### H5 Heading
###### H6 Heading
```

# H1 Heading
## H2 Heading
### H3 Heading
#### H4 Heading
##### H5 Heading
###### H6 Heading

## Text Formatting

### Emphasis

```markdown
*Italic text* or _italic text_
**Bold text** or __bold text__
***Bold italic*** or ___bold italic___
~~Strikethrough text~~
```

*Italic text* or _italic text_
**Bold text** or __bold text__
***Bold italic*** or ___bold italic___
~~Strikethrough text~~

### Inline Code

```markdown
Use `code` for inline code snippets.
```

Use `code` for inline code snippets.

## Lists

### Unordered Lists

```markdown
- First item
- Second item
  - Nested item
  - Another nested item
- Third item

* Alternative bullet
+ Another alternative
```

- First item
- Second item
  - Nested item
  - Another nested item
- Third item

* Alternative bullet
+ Another alternative

### Ordered Lists

```markdown
1. First item
2. Second item
   1. Nested item
   2. Another nested item
3. Third item
```

1. First item
2. Second item
   1. Nested item
   2. Another nested item
3. Third item

### Task Lists

```markdown
- [x] Completed task
- [ ] Pending task
- [ ] Another pending task
```

- [x] Completed task
- [ ] Pending task
- [ ] Another pending task

## Links

### Standard Links

```markdown
[Link text](https://example.com)
[Link with title](https://example.com "Title text")
```

[Link text](https://example.com)
[Link with title](https://example.com "Title text")

### Wiki Links (Jekyll Garden Special)

```markdown
[[Note Title]]
[[Link Text::Note Title]]
[[External Link::https://example.com]]
```

[[Getting Started]]
[[this guide::Getting Started]]
[[external site::https://example.com]]

### Reference Links

```markdown
[Reference link][ref]
[Another reference][ref2]

[ref]: https://example.com "Optional title"
[ref2]: https://example2.com
```

[Reference link][ref]
[Another reference][ref2]

[ref]: https://example.com "Optional title"
[ref2]: https://example2.com

## Images

```markdown
![Alt text](/assets/img/image.jpg)
![Alt text](/assets/img/image.jpg "Image title")
![Alt text](https://example.com/image.jpg)
```

![Example Image](https://via.placeholder.com/400x200?text=Example+Image)

## Code Blocks

### Fenced Code Blocks

````markdown
```javascript
function hello() {
    console.log("Hello, World!");
}
```

```python
def hello():
    print("Hello, World!")
```

```html
<div class="example">
    <p>HTML code</p>
</div>
```
````

```javascript
function hello() {
    console.log("Hello, World!");
}
```

```python
def hello():
    print("Hello, World!")
```

```html
<div class="example">
    <p>HTML code</p>
</div>
```

### Indented Code Blocks

```markdown
    This is an indented code block.
    It uses 4 spaces for indentation.
```

    This is an indented code block.
    It uses 4 spaces for indentation.

## Blockquotes

```markdown
> This is a blockquote.
> 
> It can span multiple lines.
> 
> > And can be nested.
```

> This is a blockquote.
> 
> It can span multiple lines.
> 
> > And can be nested.

## Tables

```markdown
| Header 1 | Header 2 | Header 3 |
|----------|:--------:|----------:|
| Left     | Center   | Right     |
| Content  | Content  | Content   |
```

| Header 1 | Header 2 | Header 3 |
|----------|:--------:|----------:|
| Left     | Center   | Right     |
| Content  | Content  | Content   |

### Simple Tables

```markdown
Header 1 | Header 2
---------|---------
Content  | Content
```

Header 1 | Header 2
---------|---------
Content  | Content

## Horizontal Rules

```markdown
---

***

___
```

---

***

___

## Math Expressions (KaTeX)

### Inline Math

```markdown
The quadratic formula is $x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$
```

The quadratic formula is $x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$

### Block Math

```markdown
$$
\int_{-\infty}^{\infty} e^{-x^2} dx = \sqrt{\pi}
$$
```

$$
\int_{-\infty}^{\infty} e^{-x^2} dx = \sqrt{\pi}
$$

## HTML Support

Jekyll Garden supports inline HTML for advanced formatting:

```html
<details>
<summary>Click to expand</summary>
<p>This content is hidden by default.</p>
</details>
```

<details>
<summary>Click to expand</summary>
<p>This content is hidden by default.</p>
</details>

### Definition Lists

```html
<dl>
  <dt>Term</dt>
  <dd>Definition</dd>
  <dt>Another Term</dt>
  <dd>Another definition</dd>
</dl>
```

<dl>
  <dt>Term</dt>
  <dd>Definition</dd>
  <dt>Another Term</dt>
  <dd>Another definition</dd>
</dl>

## Special Features

### Footnotes

```markdown
Here's a sentence with a footnote[^1].

[^1]: This is the footnote content.
```

Here's a sentence with a footnote[^1].

[^1]: This is the footnote content.

### Abbreviations

```markdown
*[HTML]: HyperText Markup Language
*[CSS]: Cascading Style Sheets

HTML and CSS are web technologies.
```

*[HTML]: HyperText Markup Language
*[CSS]: Cascading Style Sheets

HTML and CSS are web technologies.

## Best Practices

### Writing Style

- Use clear, descriptive headings
- Keep paragraphs short and focused
- Use lists for related items
- Link to related notes liberally

### Wiki Links

- Use descriptive note titles
- Link to related concepts
- Don't worry about over-linking
- Keep titles consistent

### Code Examples

- Use syntax highlighting when possible
- Keep examples simple and clear
- Include comments for complex code
- Test your examples

---

*This reference covers all the markdown features you need to create rich, connected notes in your digital garden.* 