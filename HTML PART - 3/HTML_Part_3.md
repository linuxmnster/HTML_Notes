# HTML_Part_3

---

## Inline vs Block

- The whole HTML elements are divided into 2 catorigies they are blcok level elements and inline elements
- Every HTML element has a default display value, depending upon what type of element it is
- All HTML tags have specific display behavior: they are either block-level elements or inline elements.

| Block elements | Inline elements |
| --- | --- |
| Takes up the full width available | Takes up only necessary width |
| Always starts from new line | Does not start from new line |
| Example : | Example: |
| <h1> <p> <div> | <a> <img> <span> |

![inline-block-image.jpg](inline-block-image.jpg)

---

## <div> Element

- `<div>` tag is often used as a container for other HTML elements with CSS to style
- It is a block element
- also called as content division element

```html
<div>
	<a href="https://www.google.com" target="_blank">Google</a>
	<a href="https://www.facebook.com" target="_blank">Facebook</a>
</div>
<a href="https://www.instagram.com" target="_blank">Instagram</a>
```

---

# <span> Element

- `<span>` tag is also a generic container used to hold other HTML elements or group elements together
- It is an inline element
- used to style a specific line using CSS

```html
<span>
	<a href="https://www.google.com" target="_blank">Google</a>
	<a href="https://www.facebook.com" target="_blank">Facebook</a>
</span>
<a href="https://www.instagram.com" target="_blank">Instagram</a>
```

---

## <hr> tag

Horizontal rule tag is used to create a horizontal line in a web page

Example :

```html
<h1>This is Heading</h1>
<hr>
<p>This is a paragraph</p>
```

---

## Superscript

- Superscript text appears half a character above the normal line, and is sometimes rendered in a smaller font.
- example for superscript : $(a+b)^2 = a^2 + b^2 +2ab$
- The `<sup>` tag can define superscript text

```html
<p>a<sup>2</sup> + b<sup>2</sup> + 2ab</p>
```

---

## Subscript

- Subscript text appears half a character below the normal line, and is sometimes rendered in a smaller font.
- example for subscript : $H_2O$
- The `<sub>` tan can define superscript text

```html
<p>H<sub>2</sub>O</p>
```

---

## **HTML Semantic Tags**

HTML5 introduced a range of semantic tags that provide meaning to the structure of web content.

### **What are Semantic Tags?**

1. `<header>`: Used to represent the top section of a web page, often containing headings, logos, and navigation.
2. `<nav>`: Signifies a navigation menu on a web page.
3. `<article>`: Indicates a self-contained piece of content, such as a blog post or news article.
4. `<section>`: Represents a thematic grouping of content on a web page.
5. `<aside>`: Typically used for sidebars or content that is tangentially related to the main content.
6. `<footer>`: Represents the footer of a web page, usually containing copyright information and contact details.
7. `<figure>` and `<figcaption>`: Used for embedding images, diagrams, or charts, along with a caption.
8. `<main>`: Signifies the main content area of a web page.
9. `<time>`: Used to represent time-related information, like dates and times.

### Why use semantic tags?

They enhance SEO, improve accessibility, and make your code easier to read and maintain.

**Examples :**

1. **sing the `<header>` tags and `<footer>` tags**

```html
<header>
    <h1>My Website</h1>
    <nav>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Services</a></li>
            <li><a href="#">Contact</a></li>
        </ul>
    </nav>
</header>

<footer>
    <p>Copyright 2024</p>
</footer>
```

1. **Using the `<article>` and `<section>` tags**

```html
<article>
    <h2>Article Title</h2>
    <section>
      <p>Content here</p>
    </section>
</article>
```

1. Using the `<aside>` and `<nav>` tags

```html
<aside>
    <p>This is an aside content</p>
  </aside>
<nav>
    <ul>
      <li>Home</li>
      <li>About</li>
    </ul>
</nav>
```

1. **Using the <figure> and <figcaption> tags**

```html
<figure>
    <img src="image.jpg" alt="An example image">
    <figcaption>This is an example image.</figcaption>
</figure>
```

### Conclusion :

- You may notice that there is no change in web page by using semantic tags this is because semantic tags are used for SEO
- Using HTML's semantic tags can greatly benefit both your website's SEO and the maintainability of your code. They offer a way to structure your HTML in a meaningful manner, making your website more accessible and easier to understand.

---

## **What Are HTML Entities?**

HTML entities are used to represent special characters in a format that the browser can understand. They start with an ampersand (&) and end with a semicolon (;).

### **Why Use HTML Entities?**

Here are some reasons:

- **Reserved Characters**: Characters like <, >, and & are reserved in HTML.
- **Special Symbols**: For symbols like ©, ®, or mathematical symbols.
- **Non-Breaking Spaces**: To create white spaces that won't break into a new line.

```html
<p>Copyright &copy; 2024.</p>
```

**Reference Entities :**

[HTML Standard](https://html.spec.whatwg.org/multipage/named-characters.html#named-character-references)

---

## Emmet

Emmet is a plugin for many popular text editors which greatly improves HTML & CSS workflow

**visit for more shortcuts and usages**

[Cheat Sheet](https://docs.emmet.io/cheat-sheet/)

---