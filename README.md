# Fundamentals of HTML and CSS

## Table of Contents
1. [Introduction](#introduction)
2. [Browser DevTools](#browser-devtools)
    1. [Accessing DevTools](#accessing-devtools)
    2. [Key Features](#key-features)
3. [HTML Basics](#html-basics)
    1. [What is HTML?](#what-is-html)
    2. [Basic Structure of an HTML Document](#basic-structure-of-an-html-document)
    3. [Basic HTML Body Tags](#basic-html-body-tags)
    4. [Semantic HTML](#semantic-html)
        1. [Examples of Semantic HTML Elements](#examples-of-semantic-html-elements)
4. [CSS Basics](#css-basics)
    1. [What is CSS?](#what-is-css)
    2. [CSS Selectors](#css-selectors)
    3. [Important CSS Units](#important-css-units)
    4. [CSS Box Model](#css-box-model)
    5. [Flexbox](#flexbox)
        1. [Basic Flexbox Example](#basic-flexbox-example)
        2. [Aligning Items](#aligning-items)
        3. [Direction of Flex Items](#direction-of-flex-items)
        4. [Wrapping Flex Items](#wrapping-flex-items)
        5. [Complex Layout Example](#complex-layout-example)
        6. [Flexbox Properties Summary](#flexbox-properties-summary)
    6. [Defining Colors, Fonts, and Other Styles](#defining-colors-fonts-and-other-styles)
        1. [Colors](#colors)
        2. [Fonts](#fonts)
5. [Conclusion](#conclusion)

## Introduction
Welcome to the fundamentals of HTML and CSS. This guide is designed for first-time learners to understand the basics of web development.

## Browser DevTools
Browser Developer Tools (DevTools) are a set of web authoring and debugging tools built into most modern web browsers. They allow you to inspect and edit HTML, CSS, and JavaScript in real-time.

### Accessing DevTools
You can open DevTools in most browsers by right-clicking on a webpage and selecting "Inspect" or by pressing `F12` or `Ctrl+Shift+I` (Windows/Linux) or `Cmd+Opt+I` (Mac).

### Key Features
- **Elements Panel**: Inspect and edit HTML and CSS.
- **Console Panel**: View and debug JavaScript.
- **Network Panel**: Monitor network requests.
- **Performance Panel**: Analyze page performance.
- **Sources Panel**: Debug JavaScript with breakpoints.

Using DevTools can greatly enhance your web development workflow by allowing you to test changes in real-time and debug issues more efficiently.

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

![](https://media.geeksforgeeks.org/wp-content/uploads/20231217130922/Screenshot-2023-12-17-130848.png)

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

- `<ul>`, `<ol>`, and `<li>`: Unordered list (bulleted), ordered list (numbered), and list item tags, used to create lists.
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

- `<div>`: Division tag (almost always just called 'div'), used as a container for other HTML elements.
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
Basic HTML blocks can be used to create nearly all of the content on the web! However, these basic blocks offer very little info about the content! Semantic HTML introduces meaning to the web page rather than just presentation. It helps search engines and other user devices determine the importance and context of web pages. Using semantic elements also makes the code more readable and easier to maintain.

#### Examples of Semantic HTML Elements

- `<em>`: Represents inline content that should be *emphasized*. Browsers render it as italics by default.

    ```html
    <p>This is an <em>important</em> piece of information!<p>
    ```

- `<strong>`: Represent inline content that should receive **strong** emphasis. Browsers render this as bold font by default.

    ```html
    <p>This is a <strong>very important</strong> piece of information!<p>
    ```
    

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

- `<article>`: Represents a self-contained composition in a document, page, application, or site, which is intended to be independently distributable or reusable. For example, for a blog post, the post's content would be in `<article>`, and related posts or navigation links before or after the post would be in other sections. 

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

### Important CSS Units
CSS units are used to define the size of elements, spacing, and other properties. Some of the most important units include:

- `px` (pixels): A fixed unit that represents a single dot on the screen. Pixel based measurements are familiar, but may not translate well to mobile devices.
    ```css
    .box {
        width: 100px;
        height: 100px;
    }
    ```

- `%` (percentage): A relative unit that is based on the size of the parent element. Percentage based widths are also useful but can be rigid. For relative positioning, learn about flexbox below!
    ```css
    .box {
        width: 50%;
    }
    ```

- `em`: A relative unit that is based on the font size of the element. By default this is 16 pixels. This is a great default unit to pick!
    - For example, it might be nice for a button with large text to have large padding.
    - This is also useful to accomodate 
    ```css
    .text {
        font-size: 2em; /* 2 times the current font size */
        max-width: 30em; /* Stop the container from growing wider than 30 * 16 = 480px (for a font size of 16) */
    }
    ```

- `rem`: A relative unit that is based on the font size of the root element (`<html>`).
    ```css
    .text {
        font-size: 1.5rem; /* 1.5 times the root font size */
    }
    ```

- `vh` (viewport height): A relative unit that is based on the height of the viewport. The viewport is the part of the screen where the webpage is visible.
    ```css
    .full-height {
        height: 100vh; /* 100% of the viewport height */
    }
    ```

- `vw` (viewport width): A relative unit that is based on the width of the viewport. The viewport is the part of the screen where the webpage is visible. 
    ```css
    .full-width {
        width: 100vw; /* 100% of the viewport width */
    }
    ```

**Note:** viewport-relative units are easy to overuse and create unexpected behavior. For example, try zooming in and out on [Professor Lewis's course schedule](https://www.cs.wm.edu/~rml/teaching/csci303/schedule_fall.html)! Then, use developer tools to find out what styles are causing this behavior.

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

![](https://www.simplilearn.com/ice9/free_resources_article_thumb/CSS-Box-Model.png)

### Flexbox
The default layout in HTML content block is the `block` display model, which relies on careful usage 

Flexbox (`display: flex`) is a layout model that allows you to design complex layouts with ease. It provides an efficient way to align and distribute space among items in a container.

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

![](https://miro.medium.com/v2/resize:fit:1080/1*y9RuktkbVshp7lmVmZrbeQ.png)

#### Direction of Flex Items
You can change the direction of the flex items using the `flex-direction` property.

```css
.container {
    display: flex;
    flex-direction: column; /* Arrange items vertically */
}
```

![](https://samanthaming.gumlet.io/flexbox30/9-flex-direction.jpg.gz)

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
<nav>
    <a href="#home">Home</a>
    <a href="#workshop">Workshop</a>
    <a href="#contact">Contact</a>
</nav>
```

```css
nav {
    background-color: #333;
    color: white;
    display: flex;
    justify-content: center;
    gap: 1em;
}

nav a {
    color: white;
    text-decoration: none;
}
```

Does this example look familiar?

#### Flexbox Properties Summary
- `display: flex;` - Defines a flex container.
- `justify-content` - Aligns items horizontally.
- `align-items` - Aligns items vertically.
- `flex-direction` - Defines the direction of the flex items.
- `flex-wrap` - Allows items to wrap onto multiple lines.

Flexbox is a powerful tool for creating responsive and flexible layouts. Experiment with these properties to see how they can simplify your web design process.

### Defining Colors, Fonts, and Other Styles

#### Colors
You can define colors in CSS using color names, HEX values, RGB, or HSL.

```css
/* Color Names */
h1 {
    color: red;
}

/* HEX Values */
p {
    color: #00ff00;
}

/* Red, Green, Blue */
div {
    background-color: rgb(0, 0, 255);
}

/* Hue, Saturation, Lightness */
span {
    color: hsl(120, 100%, 50%);
}
```

#### Fonts
To use custom fonts from Google Fonts, you need to include the font in your HTML and then apply it in your CSS.

```html
<!-- Include Google Font -->
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
```

```css
/* Apply Google Font */
body {
    font-family: 'Roboto', sans-serif;
}
```

## Conclusion
This guide has introduced the basics of HTML and CSS. With these fundamentals, you can start building and styling your own web pages. Happy coding!

