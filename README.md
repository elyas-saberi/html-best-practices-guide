# 🌐 HTML Best Practices --- Full Guide (Based on W3Schools & Modern Standards)

A complete guide to modern HTML best practices, including syntax rules,
semantic elements, accessibility tips, SEO guidelines, and clean code
formatting --- based on W3Schools + professional standards.

------------------------------------------------------------------------

## 📑 Table of Contents

-   [Introduction](#introduction)
-   [General Syntax Rules](#general-syntax-rules)
-   [HTML Elements](#html-elements)
-   [Attributes](#attributes)
-   [Boolean Attributes](#boolean-attributes)
-   [Quotations](#quotations)
-   [HTML Comments](#html-comments)
-   [HTML Head Best Practices](#html-head-best-practices)
-   [File Structure & Naming](#file-structure--naming)
-   [Code Formatting Tips](#code-formatting-tips)
-   [Avoid Deprecated Tags](#avoid-deprecated-tags)
-   [Wrap Block Elements Correctly](#wrap-block-elements-correctly)
-   [Keep CSS & JS External](#keep-css--js-external)
-   [Validate HTML](#validate-html)
-   [Accessibility Tips](#accessibility-tips)
-   [SEO Best Practices](#seo-best-practices)
-   [Performance Tips](#performance-tips)
-   [Summary Table](#summary-table)

------------------------------------------------------------------------

<a id="introduction"></a>
## 🧩 Introduction
This document provides clean, modern best practices for writing HTML.\
It expands on the guidelines from W3Schools and adds professional
standards used in production websites.

------------------------------------------------------------------------

<a id="general-syntax-rules"></a>
## 📏 General Syntax Rules

### ✔ Use lowercase for tags

``` html
<p>This is correct</p>
<P>This is NOT recommended</P>
```

### ✔ Close all tags

``` html
<br>
<img src="img.jpg" alt="Description">
```

### ✔ Always indent properly

Use **2 or 4 spaces**, but never tabs.

VSCode can automatically insert spaces when you press the Tab key.

------------------------------------------------------------------------

<a id="html-elements"></a>
## 🧱 HTML Elements

### ✔ Nest elements properly

Correct:

``` html
<p><strong>Important text</strong></p>
```

Incorrect:

``` html
<p><strong>Important text</p></strong>
```

\### ✔ Avoid unnecessary
```{=html}
<div>
```
usage

Use semantic tags such as `<header>`, `<main>`, `<footer>`, `<nav>`,
`<section>`, `<article>`, `<aside>`.

<p style="font-size:1.1em;">Read more: <b><a href="https://github.com/elyas-saberi/semantic-html-cheatsheet.git">Stop Using &lt;div&gt; Everywhere</a></b></p>

------------------------------------------------------------------------

<a id="attributes"></a>
## 🔤 Attributes

``` html
<a href="page.html">Link</a>
<input type="text" value="John">
<img src="cat.jpg" alt="A cute cat">
```

------------------------------------------------------------------------

<a id="boolean-attributes"></a>## 
🔘 Boolean Attributes

Correct:

``` html
<input type="checkbox" checked>
```

Avoid:

``` html
<input type="checkbox" checked="checked">
```

------------------------------------------------------------------------

<a id="quotations"></a>
## 💬 Quotations 

Use **double quotes** for attributes.

------------------------------------------------------------------------

<a id="html-comments"></a>
## 💬 HTML Comments

``` html
<!-- Navigation bar -->
<nav>...</nav>
```

------------------------------------------------------------------------

<a id="html-head-best-practices"></a>
## 🧠 HTML Head Best Practices

``` html
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Your Page Title</title>
```

------------------------------------------------------------------------

<a id="file-structure--naming"></a>
## 📁 File Structure & Naming

    project/
    │ README.md
    │ index.html
    │ style.css
    │ script.js
    └── assets/
        ├── images/
        ├── icons/
        └── fonts/

Lowercase + hyphens:\
`my-website-page.html`

------------------------------------------------------------------------

<a id="code-formatting-tips"></a>
## ✨ Code Formatting Tips

``` html
<img 
  src="large-photo.jpg" 
  alt="Mountain landscape" 
  loading="lazy"
/>
```

------------------------------------------------------------------------

<a id="avoid-deprecated-tags"></a>
## ⚠️ Avoid Deprecated Tags

-   `<center>`
-   `<font>`
-   `<marquee>`

------------------------------------------------------------------------

<a id="wrap-block-elements-correctly"></a>
## 🔲 Wrap Block Elements Correctly

Incorrect:

``` html
<span><div>Invalid</div></span>
```

Correct:

``` html
<div><span>Valid</span></div>
```

------------------------------------------------------------------------

<a id="keep-css--js-external"></a>
## 💻 Keep CSS & JS External

``` html
<link rel="stylesheet" href="styles.css">
<script src="script.js"></script>
```

------------------------------------------------------------------------

<a id="validate-html"></a>
## 🔍 Validate HTML

W3C Validator: https://validator.w3.org/

------------------------------------------------------------------------

<a id="accessibility-tips"></a>
## ♿ Accessibility Tips

``` html
<label for="email">Email</label>
<input id="email" type="email">
```

------------------------------------------------------------------------

<a id="seo-best-practices"></a>
## 🔍 SEO Best Practices

``` html
<h1>Main page title</h1>
<h2>Section title</h2>
```

------------------------------------------------------------------------

<a id="performance-tips"></a>
## 🚀 Performance Tips

-   Lazy-loading\
-   Compression\
-   Minification\
-   Preload\
-   Small DOM

------------------------------------------------------------------------

<a id="summary-table"></a>
## 📋 Summary Table

| Category           | Best Practice               |
|--------------------|-----------------------------|
| Doctype            | Use `<!DOCTYPE html>`       |
| Element Names      | Use lowercase               |
| Attributes         | Use lowercase & quotes      |
| Boolean Attributes | Omit value                  |
| Encoding           | UTF-8                       |
| Semantic Tags      | Use proper structure        |
| Deprecated Tags    | Avoid them                  |
| Comments           | Use proper comments         |
| Block Elements     | Wrap properly               |
| File Names         | lowercase + hyphen          |
| Indentation        | Consistent                  |
| CSS/JS             | External files              |
| Validation         | W3C Validator               |
