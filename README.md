# 🌐 HTML Best Practices — Full Guide (Based on W3Schools & Modern Standards)
A complete guide to modern HTML best practices, including syntax rules, semantic elements, accessibility tips, SEO guidelines, and clean code formatting — based on W3Schools + professional standards.

---

## 📑 Table of Contents
- [Introduction](#introduction)
- [General Syntax Rules](#general-syntax-rules)
- [HTML Elements](#html-elements)
- [Attributes](#attributes)
- [Quotations](#quotations)
- [HTML Comments](#html-comments)
- [HTML Head Best Practices](#html-head-best-practices)
- [File Structure](#file-structure)
- [Code Formatting Tips](#code-formatting-tips)
- [Accessibility Tips](#accessibility-tips)
- [SEO Best Practices](#seo-best-practices)
- [Performance Tips](#performance-tips)
- [Full Example](#full-example)

---
<a id="introduction"></a>
## 🧩 Introduction
This document provides clean, modern best practices for writing HTML.  
It expands on the guidelines from W3Schools and adds professional standards used in production websites.

---
<a id="general-syntax-rules"></a>
## 📏 General Syntax Rules

### ✔ Use lowercase for tags
```html
<p>This is correct</p>
<P>This is NOT recommended</P>
```

### ✔ Close all tags
Even void elements should follow consistent style.
```html
<br>
<img src="img.jpg" alt="Description">
```

### ✔ Always indent properly
Use **2 or 4 spaces**, but never tabs.

VSCode can automatically insert spaces when you press the Tab key.

---
<a id="html-elements"></a>
## 🧱 HTML Elements

### ✔ Nest elements properly
Incorrect nesting breaks HTML parsers.
```html
<!-- Correct -->
<p><strong>Important text</strong></p>

<!-- Incorrect -->
<p><strong>Important text</p></strong>
```

### ✔ Avoid unnecessary `<div>` usage (Semantic HTML)
Use:
- `<header>`
- `<main>`
- `<footer>`
- `<nav>`
- `<section>`
- `<article>`
- `<aside>`

Instead of endless `<div class="header">…</div>`.

<p style="font-size:1.1em;">Read more: <b><a href="https://github.com/elyas-saberi/semantic-html-cheatsheet.git">Stop Using &lt;div&gt; Everywhere</a></b></p>

---
<a id="attributes"></a>
## 🔤 Attributes

### ✔ Always use lowercase
```html
<a href="page.html">Link</a>
```

### ✔ Use quotes around attribute values
```html
<input type="text" value="John">
```

### ✔ Include required attributes (like `alt` for images)
```html
<img src="cat.jpg" alt="A cute cat">
```

---
<a id="quotations"></a>
## 💬 Quotations

Use double quotes `" "`.

✔ Recommended:
```html
<input type="text" placeholder="Enter name">
```

---
<a id="html-comments"></a>
## 💬 HTML Comments

### ✔ Use comments to describe code meaningfully
```html
<!-- Navigation bar -->
<nav>...</nav>
```

### ✘ Avoid over-commenting trivial code.

---
<a id="html-head-best-practices"></a>
## 🧠 HTML Head Best Practices

Always include:
```html
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Your Page Title</title>
```

Recommended additions:
```html
<meta name="description" content="Short SEO-friendly description.">
<link rel="stylesheet" href="style.css">
```

---
<a id="file-structure"></a>
## 📁 File Structure

Recommended GitHub-friendly project layout:
```
project/
│ README.md
│ index.html
│ style.css
│ script.js
└── assets/
    ├── images/
    ├── icons/
    └── fonts/
```

---
<a id="code-formatting-tips"></a>
## ✨ Code Formatting Tips

### ✔ Use consistent indentation  
### ✔ Write readable line lengths  
### ✔ Keep one element per line  
### ✔ Use blank lines between logical sections  
### ✔ Format attributes on new lines for long tags  

Example:
```html
<img 
  src="large-photo.jpg" 
  alt="Mountain landscape" 
  loading="lazy"
/>
```

---
<a id="accessibility-tips"></a>
## ♿ Accessibility Tips

### ✔ Add `alt` text to images  
### ✔ Use `<label>` for every `<input>`  
### ✔ Use semantic HTML  
### ✔ Ensure color contrast  
### ✔ Add ARIA roles only when necessary (never replace semantic tags)

Example:
```html
<label for="email">Email</label>
<input id="email" type="email">
```

---
<a id="seo-best-practices"></a>
## 🔍 SEO Best Practices

### ✔ Use meaningful headings (`h1` → `h6`)
```html
<h1>Main page title</h1>
<h2>Section title</h2>
```

### ✔ Use metadata
```html
<meta name="description" content="HTML best practices guide.">
```

### ✔ Use descriptive link text
Good:
```
<a href="/pricing">View pricing plans</a>
```

Bad:
```
<a href="#">Click here</a>
```

---
<a id="performance-tips"></a>
## 🚀 Performance Tips

### ✔ Use `loading="lazy"` on images
```html
<img src="photo.jpg" alt="" loading="lazy">
```

### ✔ Compress images  
### ✔ Minimize CSS & JS  
### ✔ Use `<link rel="preload">` for critical assets  
### ✔ Avoid huge DOM trees  

---
<a id="full-example"></a>
## 🧩 Full Example

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="A clean HTML5 example following best practices.">
  <title>HTML Best Practices</title>
  <link rel="stylesheet" href="style.css">
</head>

<body>
  <header>
    <h1>Welcome</h1>
    <nav>
      <a href="#intro">Intro</a>
      <a href="#content">Content</a>
    </nav>
  </header>

  <main id="content">
    <section>
      <h2>Why Semantic HTML?</h2>
      <p>It improves accessibility, SEO, and readability.</p>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 HTML Best Practices</p>
  </footer>
</body>
</html>
```

---

