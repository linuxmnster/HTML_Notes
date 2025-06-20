# HTML_Part_1

---

## **Introduction to HTML**

HTML, or HyperText Markup Language, was established in 1991 as a standard language for creating web pages. It serves as the backbone of web content by structuring and formatting elements such as headings, paragraphs, links, and images.

Key points about HTML:

- It is the language of the web, used to create websites.
- It defines the barebone structure or layout of web pages.
- HTML documents consist of a set of tags and typically have either a “.html” or “.htm” extension.
- HTML has several versions, with HTML5 being the most current.

---

## **Understanding the Term HyperText & Markup Language**

"HyperText" refers to the linking of text with other documents. "Markup Languages" utilize a specific set of tags to display elements like text, graphics, audio, video etc. Hence, HTML is the practice of representing such elements.

---

## **How Websites Work**

Accessing information on the internet involves using a web browser to retrieve content from web servers, where it is stored in the form of HTML documents. An HTML document is created by writing code with specific tags in a code editor of your choice. Once the document is saved with the “.html” extension, the browser interprets, reads, and renders the web page.

![how html homeworks.png](how_html_homeworks.png)

---

## **HTML Tags**

HTML tags serve as containers for content or other HTML tags. They are words enclosed within `<` and `>` angle brackets. These tags serve as keywords that guide the web browser in formatting and displaying the content.

Components used to design the structure of websites are called HTML tags.

---

## **HTML Elements**

An HTML element is a complete set that includes a start tag (or opening tag), content, and an end tag (or closing tag). The structure is as follows:

- HTML Element = Start Tag + Content + End Tag

For example:

`<h1>This is our first heading</h1>`

---

## **Boilerplate Code**

Boilerplate code refers to the standard format or skeleton of writing HTML code. Here is an example of an HTML5 document structure:

```html
<!DOCTYPE html> --> Defines Document type as HTML5
<html> --> Root Element of an HTML (consists head and body)
    <head> --> Contains meta information (data about data)
        <title></title>
    </head>
    <body> --> Display content of web page (for UI/UX)
        <p>This is a paragraph</p>
    </body>
</html>
```

---

## Paragraph Element

- The paragraph `<p>` tag defines a paragraph
- A paragraph always starts on a new line and browser automatically add some white space before and after a paragraph

**Example** : 

```html
<p> This is a paragraph </p>

<p> This is another paragraph </p>
```

---

## Heading Element

- The `<h1>` to `<h6>` HTML tags represent 6 levels of section heading.
- `<h1>` is the highest section level and `<h6>` is the lowest.

**Note** : the primary `<h1>` tag is used only for once in a web page

Example : 

```html
<h1> heading </h1>

<h2> heading 2 </h2>
```

---

## Nested HTML Elements

- HTML elements can be nested (this means that element can be placed inside other elements)
- All HTML documents consists of nested HTML elements

**Example :**

<p> This is <b> Bold Text </b> </p>

---

### Note Points

- HTML is not a programming language
- HTML is not a case sensitive language (but it is recomended to use lower cases)

Resource : MDN ([https://developer.mozilla.org/en-US/](https://developer.mozilla.org/en-US/)) for further information

---