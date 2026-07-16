# HTML Fundamentals

## Overview

Every website begins with HTML.

Whether you are building a personal portfolio, an online store, a social media platform, or a search engine, every webpage starts with HTML.

HTML provides the structure that tells browsers what content exists on a webpage and how that content is organized.

In this lesson, you will learn the fundamentals of HTML, including how HTML documents are structured, how elements and attributes work, and how to create meaningful, well-organized webpages.

The goal is not to memorize every HTML element.

The goal is to understand how HTML gives structure and meaning to web content.

---

## Learning Objectives

By the end of this lesson, you should be able to:

- Explain what HTML is.
- Describe the purpose of HTML in web development.
- Understand the structure of an HTML document.
- Explain HTML elements and attributes.
- Create headings, paragraphs, and lists.
- Add links and images to webpages.
- Write semantic and well-structured HTML.

---

## Why This Matters

HTML is the foundation of every website.

Without HTML:

- Browsers would have no content to display.
- CSS would have nothing to style.
- JavaScript would have nothing to manipulate.

Professional developers spend far more time organizing information than simply writing code.

Learning to structure content well is one of the most important skills in frontend development.

---

# Sub-lessons

## What Is HTML?

HTML stands for:

```
HyperText Markup Language
```

HTML is the standard language used to structure webpages.

Unlike programming languages such as JavaScript or Python, HTML does not perform calculations or make decisions.

Instead, HTML describes the content of a webpage.

For example, HTML identifies:

- Headings.
- Paragraphs.
- Images.
- Links.
- Lists.
- Tables.
- Forms.

Browsers read HTML documents and display them as webpages.

---

## HTML Is a Markup Language

HTML is called a **markup language** because it marks up content with elements that describe what the content represents.

For example:

```
This is a heading.

This is a paragraph.

This is an image.

This is a navigation menu.
```

Instead of focusing on appearance, HTML focuses on meaning and structure.

CSS will later control how this content looks.

---

## HTML Documents

Every webpage is stored as an HTML document.

A basic HTML document follows this structure:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>LearnThenCode Café</title>
</head>
<body>

</body>
</html>
```

Each part has a specific responsibility.

```
HTML Document
│
├── <!DOCTYPE html>
├── <html>
│   ├── <head>
│   └── <body>
```

---

### The DOCTYPE Declaration

The document begins with:

```html
<!DOCTYPE html>
```

This tells the browser that the document uses HTML5.

---

### The `<html>` Element

The `<html>` element is the root element of every HTML page.

Everything displayed on the webpage exists inside this element.

---

### The `<head>` Element

The `<head>` contains information about the webpage.

Examples include:

- Page title.
- Character encoding.
- Metadata.
- Links to CSS files.

Content inside `<head>` is generally **not displayed** on the webpage.

---

### The `<body>` Element

The `<body>` contains the visible content presented to users.

Examples include:

- Text.
- Images.
- Buttons.
- Navigation.
- Videos.
- Forms.

Everything users see belongs inside the `<body>`.

---

## HTML Elements

HTML is built using elements.

An element usually consists of:

- An opening tag.
- Content.
- A closing tag.

Example:

```html
<h1>Welcome to LearnThenCode Café</h1>
<p>Code. Coffee. Community.</p>
```

Structure:

```
Opening Tag
     ↓
<p>

Content
     ↓
Hello, LearnThenCode!

Closing Tag
     ↓
</p>
```

---

## HTML Attributes

Attributes provide additional information about elements.

Example:

```html
<img src="logo.png" alt="LearnThenCode Logo">
```

In this example:

- `src` specifies the image location.
- `alt` provides alternative text.

Attributes appear inside the opening tag.

---

## Common HTML Elements

### Headings

HTML provides six heading levels.

```html
<h1>Main Heading</h1>
<h2>Section Heading</h2>
<h3>Subsection</h3>
```

`<h1>` represents the most important heading.

`<h6>` represents the least important.

---

### Paragraphs

Paragraphs are created using:

```html
<p>This is a paragraph.</p>
```

Paragraphs are used for blocks of text.

---

### Lists

HTML supports two common list types.

#### Unordered Lists

```html
<ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ul>
```

---

#### Ordered Lists

```html
<ol>
    <li>Plan</li>
    <li>Build</li>
    <li>Test</li>
</ol>
```

---

### Links

Links connect webpages together.

Example:

```html
<a href="https://learnthencode.com">
    Visit LearnThenCode
</a>
```

The `href` attribute specifies the destination.

---

### Images

Images are added using:

```html
<img
    src="profile.jpg"
    alt="Student Profile">
```

The `alt` attribute improves accessibility.

---

## Nesting Elements

HTML elements can contain other elements.

Example:

```html
<article>
    <h2>Welcome</h2>
    <p>Learning HTML is the first step toward web development.</p>
</article>
```

This relationship forms a tree-like structure.

```
article
├── h2
└── p
```

This structure becomes important when learning CSS and JavaScript.

---

## Writing Good HTML

Professional developers write HTML that is:

- Well organized.
- Properly indented.
- Easy to read.
- Semantic.
- Accessible.

Good HTML is easier to maintain and easier for other developers to understand.

---

# Key Takeaways

- HTML structures webpages.
- HTML is a markup language.
- Every webpage begins with an HTML document.
- HTML documents contain a head and a body.
- Elements describe different types of content.
- Attributes provide additional information.
- Well-structured HTML improves maintainability and accessibility.

---

# Summary

In this lesson, you learned:

- What HTML is.
- Why HTML is the foundation of every webpage.
- How HTML documents are organized.
- The purpose of elements and attributes.
- How to create headings, paragraphs, lists, links, and images.
- Why clean, semantic HTML matters.
- How HTML forms the foundation of your LearnThenCode Café website.

Remember:

> **HTML provides the structure of a webpage. A strong structure makes every website easier to style, maintain, and improve.**

---

# Before You Continue

Before moving to the next lesson, make sure you can confidently:

- [ ] Explain what HTML is.
- [ ] Describe the structure of an HTML document.
- [ ] Differentiate between elements and attributes.
- [ ] Create headings, paragraphs, lists, links, and images.
- [ ] Explain why semantic HTML is important.

If you are unsure about any of the above, review this lesson before continuing.

---

# What's Next?

Now that you understand the fundamentals of HTML, the next lesson will explore:

**Browser Fundamentals and Developer Tools**

You will learn how browsers interpret HTML documents, render webpages, and how professional developers inspect and debug websites using built-in browser tools.