---
title: 'Markdown Format Test'
date: 2026-06-11T00:00:00+08:00
tags: ['markdown', 'test']
categories: ['Blog']
description: 'A comprehensive test of Markdown rendering features including headings, code blocks, math formulas, tables, and more.'
---

This article serves as a comprehensive test of Markdown rendering capabilities and theme features.

## Headings

### Third-level heading

#### Fourth-level heading

##### Fifth-level heading

###### Sixth-level heading

## Text Formatting

**Bold text** *Italic text* ~~Strikethrough~~ `Inline code` [Hyperlink](https://gohugo.io/)

> This is a blockquote. It can span multiple lines and is used to highlight important quotes or references.

## Lists

### Unordered List

- Item A
- Item B
  - Nested item B-1
  - Nested item B-2
- Item C

### Ordered List

1. First step
2. Second step
3. Third step

### Mixed List

- Category 1
  1. Sub-item one
  2. Sub-item two
- Category 2
  - Sub-item alpha
  - Sub-item beta

## Code Blocks

### Python

```python
def fibonacci(n):
    """Generate Fibonacci sequence up to n terms."""
    a, b = 0, 1
    for _ in range(n):
        yield a
        a, b = b, a + b

# Print first 10 Fibonacci numbers
print(list(fibonacci(10)))
```

### JavaScript

```javascript
// Dark/Light mode toggle
const toggleTheme = () => {
  const isDark = document.documentElement.classList.toggle('dark');
  localStorage.setItem('theme', isDark ? 'dark' : 'light');
};

document.getElementById('theme-toggle')
  .addEventListener('click', toggleTheme);
```

### Go

```go
package main

import "fmt"

func main() {
    site := map[string]string{
        "title": "VERNIY.SITE",
        "theme": "void",
    }
    fmt.Printf("Welcome to %s!\n", site["title"])
}
```

### Bash

```bash
#!/bin/bash
# Build the Hugo site
echo "Building site..."
hugo --minify --gc
echo "Site built successfully!"
```

## Tables

| Feature       | Supported | Notes                |
|---------------|-----------|----------------------|
| Dark Mode     | ✅ Yes    | Toggle in header     |
| KaTeX Math    | ✅ Yes    | Inline & display     |
| Code Highlight| ✅ Yes    | HLJS with themes     |
| Tags          | ✅ Yes    | Clickable chips      |
| TOC           | ✅ Yes    | Collapsible sidebar   |
| Comments      | ✅ Yes    | Disqus (lazy-loaded)  |

## KaTeX Math

Inline math: $E = mc^2$

Display math:

$$
\int_{-\infty}^{\infty} e^{-x^2} \, dx = \sqrt{\pi}
$$

Matrix notation:

$$
A = \begin{pmatrix}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23} \\
a_{31} & a_{32} & a_{33}
\end{pmatrix}
$$

## Horizontal Rule

---

## Callouts

{{< callout type="info" >}}
This is an **info** callout — useful for additional context or tips.
{{< /callout >}}

{{< callout type="tip" >}}
Here's a **tip** to help you along the way.
{{< /callout >}}

{{< callout type="warning" >}}
**Warning:** This is important information you should pay attention to.
{{< /callout >}}

{{< callout type="danger" >}}
**Danger:** This indicates a critical issue or potential error.
{{< /callout >}}

## Images

![Test Image](https://via.placeholder.com/800x400?text=Placeholder+Image)
*Caption: This is a sample image caption.*

## HTML (unsafe mode)

<div class="p-4 bg-blue-50 dark:bg-blue-900/20 rounded-lg border border-blue-200 dark:border-blue-800">
  <p class="text-blue-800 dark:text-blue-200">This is a custom HTML block rendered with Tailwind CSS classes. Hugo's <code>unsafe</code> mode allows raw HTML in Markdown.</p>
</div>

## Conclusion

This post demonstrates the key Markdown features supported by the Void theme. All elements should render correctly with proper syntax highlighting, math rendering, and responsive layout.