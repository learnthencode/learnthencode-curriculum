# Working with Content

## Overview

In the previous lessons, you learned how the web works, how HTML structures webpages, and how browsers interpret and display HTML documents.

So far, the webpages you have created contain only basic content such as headings, paragraphs, lists, links, and images.

Real-world websites, however, contain much richer content. They display data in tables, collect information through forms, present multimedia such as audio and video, and organize information using semantic HTML elements.

In this lesson, you will learn how to build webpages that communicate information more effectively and provide meaningful interactions for users.

You will continue improving the **LearnThenCode Café** website by adding menus, contact forms, multimedia, and a professional page structure.

The goal is not simply to learn new HTML elements.

The goal is to understand how different types of content should be organized so that webpages are informative, accessible, and easy to maintain.

---

## Learning Objectives

By the end of this lesson, you should be able to:

- Create tables to organize structured data.
- Build forms that collect user information.
- Use common form controls.
- Understand the purpose of form labels.
- Embed multimedia such as audio and video.
- Embed external content using iframes.
- Organize webpages using semantic HTML elements.
- Build webpages that are easier to understand and maintain.

---

## Why This Matters

Professional websites do much more than display text.

Consider some common websites:

- An online store displays products in organized layouts.
- A school website collects student applications.
- A restaurant website displays menus and accepts reservations.
- A news website presents articles, videos, and images.
- A business website allows visitors to submit enquiries.

As a web developer, you need to understand how to present different types of information in ways that are both useful and accessible.

Learning how to organize content effectively prepares you to build professional websites that meet the needs of real users.

---

# Sub-lessons

## Why Content Organization Matters

Imagine walking into a library where every book has been placed randomly on the shelves.

Finding a specific book would be frustrating and time-consuming.

Webpages work in a similar way.

If information is not organized properly, users struggle to find what they need.

Good content organization helps users:

- Read information more easily.
- Navigate webpages efficiently.
- Understand relationships between different sections.
- Complete tasks such as filling out forms.

Good organization also helps developers maintain and improve websites over time.

---

## HTML Tables

Some information is easier to understand when it is organized into rows and columns.

HTML provides the `<table>` element for displaying structured data.

Examples of information commonly presented in tables include:

- Product prices
- Class timetables
- Restaurant menus
- Employee records
- Examination results

Tables should only be used for **tabular data**.

They should **not** be used to control the layout of a webpage.

Modern webpage layouts are created using CSS, which you will learn later in this course.

---

## Creating a Simple Table

A basic HTML table consists of rows and cells.

Example:

```html
<table>
    <tr>
        <td>Tea</td>
        <td>KES 150</td>
    </tr>

    <tr>
        <td>Coffee</td>
        <td>KES 200</td>
    </tr>
</table>
```

In this example:

- `<table>` creates the table.
- `<tr>` creates a table row.
- `<td>` creates a table cell.

The browser displays the information as a grid.

---

## Table Headers

Tables become easier to understand when they include headings.

HTML provides the `<th>` element for header cells.

Example:

```html
<table>
    <tr>
        <th>Item</th>
        <th>Price</th>
    </tr>

    <tr>
        <td>Tea</td>
        <td>KES 150</td>
    </tr>

    <tr>
        <td>Coffee</td>
        <td>KES 200</td>
    </tr>
</table>
```

Header cells describe the information contained in each column.

Browsers typically display header cells in bold text to distinguish them from regular table cells.

---

## Table Sections

Large tables are easier to understand when they are divided into logical sections.

HTML provides three elements for organizing tables:

- `<thead>`
- `<tbody>`
- `<tfoot>`

Example:

```html
<table>
    <thead>
        <tr>
            <th>Item</th>
            <th>Price</th>
        </tr>
    </thead>

    <tbody>
        <tr>
            <td>Tea</td>
            <td>KES 150</td>
        </tr>

        <tr>
            <td>Coffee</td>
            <td>KES 200</td>
        </tr>
    </tbody>

    <tfoot>
        <tr>
            <td colspan="2">
                Prices subject to change.
            </td>
        </tr>
    </tfoot>
</table>
```

These elements improve readability and help browsers and assistive technologies better understand the structure of the table.

---

## Table Captions

A table should clearly describe the information it contains.

HTML provides the `<caption>` element for this purpose.

Example:

```html
<table>
    <caption>LearnThenCode Café Drinks Menu</caption>

    <tr>
        <th>Drink</th>
        <th>Price</th>
    </tr>

    <tr>
        <td>Tea</td>
        <td>KES 150</td>
    </tr>
</table>
```

The caption gives users context before they begin reading the table.

---

## Merging Table Cells

Sometimes a table cell needs to span multiple columns or rows.

HTML provides two attributes:

- `colspan`
- `rowspan`

Example:

```html
<tr>
    <td colspan="2">
        Weekend Special Menu
    </td>
</tr>
```

`colspan` allows one cell to occupy multiple columns.

Similarly, `rowspan` allows one cell to occupy multiple rows.

These attributes should be used only when they improve the clarity of the information being presented.

---

## When Should You Use Tables?

Tables are designed for presenting structured data.

Good examples include:

- Restaurant menus
- Product catalogues
- School timetables
- Financial reports
- Sports standings

Tables should **not** be used to position content on a webpage.

In the early days of the web, developers often used tables to create webpage layouts.

Today, this is considered poor practice.

Modern layouts are created using CSS technologies such as Flexbox and Grid, which you will learn later in this course.

---

## Practical Example

As you continue building the **LearnThenCode Café** website, you can use a table to display the café menu.

For example:

```html
<table>
    <caption>Hot Drinks</caption>

    <thead>
        <tr>
            <th>Drink</th>
            <th>Price</th>
        </tr>
    </thead>

    <tbody>
        <tr>
            <td>Tea</td>
            <td>KES 150</td>
        </tr>

        <tr>
            <td>Coffee</td>
            <td>KES 200</td>
        </tr>

        <tr>
            <td>Hot Chocolate</td>
            <td>KES 250</td>
        </tr>
    </tbody>
</table>
```

This provides visitors with a clear and organized view of the café's offerings.

---

## HTML Forms

Many websites do more than present information.

They also allow users to interact with the website by submitting information.

Some common examples include:

- Logging into an account.
- Creating a new account.
- Searching for products.
- Booking a hotel.
- Making a restaurant reservation.
- Sending a contact message.
- Completing an online application.

HTML provides **forms** to collect information from users.

A form acts as a container for different types of input fields that allow users to enter data.

---

## The `<form>` Element

Every HTML form begins with the `<form>` element.

Example:

```html
<form>

</form>
```

All form controls, such as text fields, checkboxes, and buttons, are placed inside the form element.

In real-world applications, forms usually send information to a server for processing.

Later in the bootcamp, when you learn backend development, you will understand exactly how this process works.

For now, our focus is on creating well-structured forms.

---

## Form Controls

A form can contain many different types of controls.

Some of the most common include:

- Text fields
- Email fields
- Password fields
- Number fields
- Checkboxes
- Radio buttons
- Drop-down lists
- Text areas
- Buttons

Each control is designed to collect a specific type of information.

---

## Text Inputs

The most common form control is the text input.

Example:

```html
<input type="text">
```

This creates a field where users can type text.

For example:

- First name
- Last name
- City
- Occupation

---

## Email Inputs

When collecting email addresses, use the `email` input type.

Example:

```html
<input type="email">
```

Modern browsers can recognize whether the entered value resembles an email address.

This helps reduce user mistakes.

---

## Password Inputs

Passwords should use the `password` input type.

Example:

```html
<input type="password">
```

Instead of displaying the actual characters, browsers hide the entered text for privacy.

---

## Number Inputs

To collect numerical information, use the `number` input type.

Example:

```html
<input type="number">
```

Examples include:

- Age
- Quantity
- Number of guests
- Number of tickets

---

## Date Inputs

Many forms ask users to choose a date.

HTML provides a built-in date picker.

Example:

```html
<input type="date">
```

Browsers usually display a calendar interface, making it easier for users to select a date.

---

## Checkboxes

Checkboxes allow users to select zero, one, or multiple options.

Example:

```html
<label>
    <input type="checkbox">
    Receive promotional emails
</label>
```

Checkboxes are useful when multiple selections are allowed.

---

## Radio Buttons

Radio buttons allow users to choose **only one** option from a group.

Example:

```html
<label>
    <input
        type="radio"
        name="drink"
        value="tea">
    Tea
</label>

<label>
    <input
        type="radio"
        name="drink"
        value="coffee">
    Coffee
</label>
```

Because both radio buttons share the same `name`, only one can be selected at a time.

---

## Drop-down Lists

When users should choose from a predefined list, use a drop-down menu.

Example:

```html
<label for="branch">
    Preferred Branch
</label>

<select id="branch">
    <option>Mombasa</option>
    <option>Nairobi</option>
    <option>Kisumu</option>
</select>
```

Drop-down lists help reduce typing and improve consistency.

---

## Text Areas

Some information requires more than a single line of text.

For longer responses, use a `<textarea>`.

Example:

```html
<label for="message">
    Message
</label>

<textarea
    id="message"
    rows="5"
    cols="40">
</textarea>
```

Text areas are commonly used for:

- Feedback
- Reviews
- Comments
- Contact messages

---

## Buttons

Buttons allow users to submit forms or perform actions.

Example:

```html
<button type="submit">
    Submit
</button>
```

The `submit` button sends the completed form for processing.

Later in the bootcamp, you will learn how servers receive and process submitted form data.

---

## Labels

Every form control should have a descriptive label.

Example:

```html
<label for="name">
    Full Name
</label>

<input
    type="text"
    id="name">
```

Labels improve:

- Accessibility
- Usability
- Readability

Users immediately understand what information each field requires.

Screen readers also rely on labels to help visually impaired users navigate forms.

---

## Placeholder Text

Inputs may also include placeholder text.

Example:

```html
<input
    type="text"
    placeholder="Enter your full name">
```

Placeholder text provides a helpful example of the expected input.

However, placeholders should **not** replace labels.

Labels identify the purpose of a field, while placeholders provide additional guidance.

---

## Required Fields

Some information is mandatory.

HTML allows developers to indicate required fields using the `required` attribute.

Example:

```html
<input
    type="email"
    required>
```

If the user attempts to submit the form without completing this field, the browser displays a validation message.

---

## Basic Form Validation

Modern browsers perform some validation automatically.

For example:

```html
<input
    type="email"
    required>
```

The browser checks whether:

- The field is empty.
- The value resembles an email address.

If either check fails, the form cannot be submitted until the issue is corrected.

This is called **client-side validation**.

Later in the bootcamp, you will learn why servers must also validate submitted data.

---

## Practical Example

As you continue improving the **LearnThenCode Café** website, you can add a reservation form.

Example:

```html
<form>

    <label for="name">
        Full Name
    </label>

    <input
        type="text"
        id="name"
        required>

    <br><br>

    <label for="email">
        Email Address
    </label>

    <input
        type="email"
        id="email"
        required>

    <br><br>

    <label for="guests">
        Number of Guests
    </label>

    <input
        type="number"
        id="guests"
        min="1"
        required>

    <br><br>

    <label for="date">
        Reservation Date
    </label>

    <input
        type="date"
        id="date"
        required>

    <br><br>

    <button type="submit">
        Book Table
    </button>

</form>
```

Although this form does not yet send information to a server, it demonstrates how professional forms are structured.

In later courses, you will learn how to process submitted data and store it in databases.

---

## Multimedia

Modern websites use more than text.

They often include:

- Images
- Audio
- Video
- Maps
- Interactive content

Multimedia makes webpages more engaging and helps communicate information in different ways.

HTML provides several elements for embedding multimedia directly into webpages.

---

## Images Revisited

Earlier in this course, you learned how to display images using the `<img>` element.

Example:

```html
<img
    src="cafe.jpg"
    alt="Customers enjoying coffee at LearnThenCode Café">
```

Remember that the `alt` attribute serves two important purposes:

- It describes the image for users who cannot see it.
- It provides alternative text if the image cannot be displayed.

Writing meaningful alternative text is an important part of building accessible websites.

---

## Audio

HTML allows developers to embed audio without requiring additional software or plugins.

The `<audio>` element is used for this purpose.

Example:

```html
<audio controls>
    <source src="background-music.mp3" type="audio/mpeg">

    Your browser does not support the audio element.
</audio>
```

The `controls` attribute displays built-in playback controls such as:

- Play
- Pause
- Volume
- Progress bar

If the browser cannot play the audio, the fallback message is displayed instead.

---

## Video

Videos can also be embedded directly into webpages.

Example:

```html
<video controls width="640">
    <source src="cafe-tour.mp4" type="video/mp4">

    Your browser does not support the video element.
</video>
```

Like the audio element, the `controls` attribute displays playback controls.

Depending on the browser, users can usually:

- Play and pause the video.
- Adjust the volume.
- Enter full-screen mode.
- Skip forward or backward.

---

## Embedded Content

Sometimes the content you want to display is hosted on another website.

Instead of recreating it yourself, you can embed it into your webpage.

HTML provides the `<iframe>` element for embedding external content.

Examples include:

- Google Maps
- YouTube videos
- Online documents
- Interactive applications

---

## Using an `<iframe>`

A basic iframe looks like this:

```html
<iframe
    src="https://www.example.com"
    width="600"
    height="400">
</iframe>
```

The embedded webpage appears inside the current webpage.

Many online services provide ready-made iframe code that developers can copy and paste into their websites.

---

## Practical Example

Suppose the LearnThenCode Café wants customers to find its location more easily.

Instead of creating a map from scratch, the café can embed a Google Map on its contact page using an iframe provided by Google Maps.

Similarly, the café could embed a promotional video hosted on YouTube instead of storing large video files on its own server.

Embedding external content helps developers create richer websites while reducing the amount of content they need to host themselves.

---

## Semantic Page Structure

As websites become larger, organizing content becomes increasingly important.

Imagine opening a book where every paragraph appears in a random order.

Although all the information exists, the book would be difficult to read.

Webpages are no different.

Professional developers organize webpages into meaningful sections using **semantic HTML elements**.

Semantic elements describe the purpose of the content they contain rather than simply its appearance.

---

## Common Semantic Elements

Some of the most commonly used semantic elements include:

| Element | Purpose |
|---------|----------|
| `<header>` | Introductory content for a page or section |
| `<nav>` | Navigation links |
| `<main>` | The primary content of the webpage |
| `<section>` | A related group of content |
| `<article>` | Independent content such as a blog post or news article |
| `<aside>` | Supporting or secondary content |
| `<footer>` | Information appearing at the bottom of a page or section |

These elements help both developers and browsers understand the organization of a webpage.

---

## Building a Semantic Webpage

Consider the following simplified webpage structure.

```html
<body>

    <header>
        ...
    </header>

    <nav>
        ...
    </nav>

    <main>

        <section>
            ...
        </section>

        <section>
            ...
        </section>

    </main>

    <footer>
        ...
    </footer>

</body>
```

Instead of using many generic `<div>` elements, semantic elements clearly describe the role of each part of the page.

This improves readability and maintainability.

---

## Benefits of Semantic HTML

Using semantic HTML provides many advantages.

### Improved Readability

Developers can quickly understand the purpose of each section of the webpage.

---

### Better Accessibility

Assistive technologies such as screen readers use semantic elements to help users navigate webpages more efficiently.

---

### Improved Search Engine Optimization (SEO)

Search engines analyze webpage structure when indexing websites.

Semantic HTML helps search engines better understand webpage content.

---

### Easier Maintenance

Well-organized webpages are easier to modify as projects grow.

Future developers can understand the structure without reading every line of code.

---

## Continuing the LearnThenCode Café Project

By the end of this lesson, your LearnThenCode Café website may include:

- A semantic page structure.
- A menu displayed using tables.
- A reservation or contact form.
- Images.
- Embedded multimedia.
- Embedded maps or other external content.

Although the website is still simple, it now resembles a real-world website much more closely than the basic HTML page you created earlier in the course.

In the next lesson, you will begin improving its appearance using CSS.

---

# Key Takeaways

- Tables organize structured data into rows and columns.
- Forms collect information from users.
- Labels improve accessibility and usability.
- Built-in HTML validation helps users enter valid information.
- Multimedia such as audio and video can be embedded directly into webpages.
- External content can be embedded using iframes.
- Semantic HTML improves organization, accessibility, and maintainability.
- Well-structured content creates a better experience for both users and developers.

---

# Summary

In this lesson, you learned:

- How to create tables for structured information.
- How to build forms using common form controls.
- The importance of labels and basic validation.
- How to embed audio, video, and external content.
- How to organize webpages using semantic HTML.
- Why thoughtful content organization improves professional websites.

Remember:

> **Professional websites are more than collections of HTML elements. They organize information in meaningful ways that make content easier to understand, easier to maintain, and more accessible to everyone.**

---

# Before You Continue

Before moving to the next lesson, make sure you can confidently:

- [ ] Create tables with rows, headers, and captions.
- [ ] Build forms using common input controls.
- [ ] Explain the purpose of labels and required fields.
- [ ] Embed images, audio, and video.
- [ ] Explain when to use an iframe.
- [ ] Organize a webpage using semantic HTML elements.
- [ ] Explain why semantic HTML is important.

If you are unsure about any of the above, review this lesson before continuing.

---

# What's Next?

Now that you can build well-structured webpages containing meaningful content, the next lesson will explore:

**CSS Fundamentals**

You will learn how CSS transforms plain HTML documents into visually appealing websites by controlling colors, typography, spacing, borders, backgrounds, and many other aspects of presentation.