# Fundamentals of HTML and CSS

## Table of Contents
1. [Introduction](#introduction)
2. [HTML Basics](#html-basics)
    1. [What is HTML?](#what-is-html)
    2. [Basic Structure of an HTML Document](#basic-structure-of-an-html-document)
    3. [Semantic HTML](#semantic-html)
3. [CSS Basics](#css-basics)
    1. [What is CSS?](#what-is-css)
    2. [CSS Selectors](#css-selectors)
    3. [CSS Box Model](#css-box-model)
    4. [Flexbox](#flexbox)
4. [Conclusion](#conclusion)

## Introduction
Welcome to the fundamentals of HTML and CSS. This guide is designed for first-time learners to understand the basics of web development.

## HTML Basics

### What is HTML?
HTML (HyperText Markup Language) is the standard language for creating web pages. It describes the structure of a webpage.

### Basic Structure of an HTML Document
An HTML document has a defined structure that includes elements such as `<!DOCTYPE html>`, `<html>`, `<head>`, and `<body>`.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Page Title</title>
</head>
<body>
    <h1>This is a Heading</h1>
    <p>This is a paragraph.</p>
</body>
</html>
```

### Basic HTML Body Tags
The body of an HTML document contains the content that is displayed on the web page. Here are some basic HTML body tags:

- `<h1>` to `<h6>`: Heading tags, with `<h1>` being the highest (or most important) level and `<h6>` the least.
    ```html
    <h1>Main Heading</h1>
    <h2>Subheading</h2>
    <h3>Sub-subheading</h3>
    ```

- `<p>`: Paragraph tag, used for blocks of text.
    ```html
    <p>This is a paragraph of text.</p>
    ```

- `<a>`: Anchor tag, used to create hyperlinks.
    ```html
    <a href="https://www.example.com">Visit Example.com</a>
    ```

- `<img>`: Image tag, used to embed images.
    ```html
    <img src="image.jpg" alt="Description of image">
    ```

- `<ul>`, `<ol>`, and `<li>`: Unordered list, ordered list, and list item tags, used to create lists.
    ```html
    <ul>
        <li>Item 1</li>
        <li>Item 2</li>
    </ul>
    <ol>
        <li>First item</li>
        <li>Second item</li>
    </ol>
    ```

- `<div>`: Division tag, used as a container for other HTML elements.
    ```html
    <div>
        <h2>Section Title</h2>
        <p>Some content here.</p>
    </div>
    ```

- `<span>`: Span tag, used to group inline-elements in a document.
    ```html
    <p>This is a <span style="color: red;">red</span> word.</p>
    ```

### Semantic HTML
Semantic HTML introduces meaning to the web page rather than just presentation. It helps search engines and other user devices determine the importance and context of web pages. Using semantic elements also makes the code more readable and easier to maintain.

#### Examples of Semantic HTML Elements

- `<header>`: Represents a container for introductory content or a set of navigational links.
    ```html
    <header>
        <h1>Welcome to My Website</h1>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>
    ```

- `<footer>`: Represents a footer for its nearest sectioning content or sectioning root element.
    ```html
    <footer>
        <p>&copy; 2023 My Website. All rights reserved.</p>
    </footer>
    ```

- `<article>`: Represents a self-contained composition in a document, page, application, or site, which is intended to be independently distributable or reusable.
    ```html
    <article>
        <h2>Understanding Semantic HTML</h2>
        <p>Semantic HTML introduces meaning to the web page rather than just presentation...</p>
    </article>
    ```

- `<section>`: Represents a standalone section which doesn't have a more specific semantic element to represent it.
    ```html
    <section>
        <h2>About Us</h2>
        <p>We are a company dedicated to providing the best services...</p>
    </section>
    ```

- `<aside>`: Represents a portion of a document whose content is only indirectly related to the document's main content.
    ```html
    <aside>
        <h2>Related Articles</h2>
        <ul>
            <li><a href="#article1">Article 1</a></li>
            <li><a href="#article2">Article 2</a></li>
        </ul>
    </aside>
    ```

- `<nav>`: Represents a section of a page that links to other pages or to parts within the page.
    ```html
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#services">Services</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>
    ```

Using these semantic elements improves the accessibility of web pages, making it easier for screen readers to navigate and understand the content. It also enhances SEO (Search Engine Optimization) by providing clearer structure and meaning to the content.


## CSS Basics

### What is CSS?
CSS (Cascading Style Sheets) is used to style and layout web pages. It controls the color, font, spacing, and positioning of HTML elements.

### CSS Selectors
CSS selectors are used to select the HTML elements you want to style. Examples include element selectors, class selectors, and ID selectors.

```css
/* Element Selector */
p {
    color: blue;
}

/* Class Selector */
.intro {
    font-size: 20px;
}

/* ID Selector */
#main {
    margin: 10px;
}
```

### CSS Box Model
The CSS box model describes the rectangular boxes generated for elements in the document tree and consists of margins, borders, padding, and the actual content.

```css
div {
    width: 300px;
    padding: 10px;
    border: 5px solid black;
    margin: 20px;
}
```

### Flexbox
Flexbox is a layout model that allows you to design complex layouts with ease. It provides an efficient way to align and distribute space among items in a container.

#### Basic Flexbox Example
To start using Flexbox, you need to set the `display` property of a container element to `flex`.

```css
.container {
    display: flex;
}
```

This will make all direct children of the container flexible items.

#### Aligning Items
You can align items along the main axis using `justify-content` and along the cross axis using `align-items`.

```css
.container {
    display: flex;
    justify-content: center; /* Center items horizontally */
    align-items: center;     /* Center items vertically */
}
```

#### Direction of Flex Items
You can change the direction of the flex items using the `flex-direction` property.

```css
.container {
    display: flex;
    flex-direction: column; /* Arrange items vertically */
}
```

#### Wrapping Flex Items
By default, flex items will try to fit into one line. You can allow them to wrap onto multiple lines using the `flex-wrap` property.

```css
.container {
    display: flex;
    flex-wrap: wrap; /* Allow items to wrap onto multiple lines */
}
```

#### Complex Layout Example
Combining these properties, you can create more complex layouts. For example, a responsive navigation bar:

```html
<nav class="navbar">
    <div class="logo">Logo</div>
    <ul class="nav-links">
        <li>Home</li>
        <li>About</li>
        <li>Services</li>
        <li>Contact</li>
    </ul>
</nav>
```

```css
.navbar {
    display: flex;
    justify-content: space-between; /* Space out items */
    align-items: center;            /* Center items vertically */
    padding: 10px;
    background-color: #333;
    color: white;
}

.nav-links {
    display: flex;
    list-style: none;
}

.nav-links li {
    margin: 0 10px;
}
```

This example demonstrates a navigation bar with a logo on the left and navigation links on the right, spaced out evenly.

#### Flexbox Properties Summary
- `display: flex;` - Defines a flex container.
- `justify-content` - Aligns items horizontally.
- `align-items` - Aligns items vertically.
- `flex-direction` - Defines the direction of the flex items.
- `flex-wrap` - Allows items to wrap onto multiple lines.

Flexbox is a powerful tool for creating responsive and flexible layouts. Experiment with these properties to see how they can simplify your web design process.


## Conclusion
This guide has introduced the basics of HTML and CSS. With these fundamentals, you can start building and styling your own web pages. Happy coding!