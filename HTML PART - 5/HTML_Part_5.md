# HTML_Part_5

---

## **HTML Id & Classes**

HTML offers multiple ways to select and style elements. Two of the most commonly used selectors are IDs and Classes. This blog explores what they are, how to use them, and their differences.

- An `ID` is an attribute, a unique identifier assigned to only one HTML element within a page. It is often used for unique styling and JavaScript manipulations.

```html
<div id="myUniqueID">This is a div with an ID.</div>
```

- The `class` attribute lets you give the same name to multiple HTML elements. That way, you can easily change their look or behavior all at once. Classes are not unique and can be assigned to multiple elements. They are generally used for applying the same styles or behaviors to a group of elements.

```html
<div class="myClass">This is a div with a class.</div>
<p class="myClass">This is a paragraph with the same class.</p>
```

---

## **Pre Tag**

- The <pre> tag preserves the original formatting of text, making it an excellent choice for displaying code where spacing and indentation are key.
- The <pre> tag maintains both spaces and line breaks, ensuring that text appears exactly as it was originally formatted.

```html
<pre>
    <!-- code snippet in any programming language -->
</pre>
```

---

## **HTML Meta Tags**

The `<meta>` tags in HTML provide metadata about the HTML document. Metadata is data (information) about data. `<meta>` tags always go inside the document's `<head>` tag and are typically used to specify the character set, page description, keywords, author, and other metadata.

```html
<meta charset="UTF-8"> <!-- Character encoding -->
<meta name="viewport" content="width=device-width, initial-scale=1.0"> <!-- Responsive design -->
<meta http-equiv="X-UA-Compatible" content="ie=edge"> <!-- Internet Explorer compatibility -->
<meta name="description" content="This is a description of the web page"> <!-- Description for search engines -->
<meta name="keywords" content="HTML, CSS, JavaScript"> <!-- Keywords for search engines -->
<meta name="author" content="Your Name"> <!-- Author name -->
```

### **Explanation of each meta tag:**

1. **Character Encoding (`charset`)**: `<meta charset="UTF-8">` sets the character encoding for the webpage. UTF-8 is the most common and recommended.
2. **Viewport**: `<meta name="viewport" content="width=device-width, initial-scale=1.0">` sets the viewport to scale the page to the screen width, useful for responsive design.
3. **IE Compatibility**: `<meta http-equiv="X-UA-Compatible" content="ie=edge">` specifies that the page should be rendered using the latest rendering engine available on Internet Explorer.
4. **Description**: `<meta name="description" content="This is a description of the web page">` provides a brief description of the webpage, which search engines may use in search results.
5. **Keywords**: `<meta name="keywords" content="HTML, CSS, JavaScript">` specifies keywords for the webpage, which were historically used by search engines but are less relevant today.
6. **Author**: `<meta name="author" content="Your Name">` indicates the name of the author of the webpage.

---

## Video Tag

The `<video>` tag is used to embed video files in an HTML document. It supports multiple attributes to control the video playback.

```html
<video src="video.mp4" controls></video>
```

### **Attributes for `<video>` Tag**

- **src**: Specifies the path to the video file.
- **controls**: Adds video controls, like play, pause, and volume.
- **autoplay**: Automatically starts playing the video when the page loads.
- **loop**: Repeats the video once it ends.
- **muted**: Mutes the video by default.
- **poster**: Specifies an image to be displayed before the video starts playing.
- **width** and **height**: Specifies the dimensions of the video.

---

## Audio Tag

The `<audio>` tag is used to embed audio files in an HTML document. It also supports multiple attributes for control.

```html
<audio src="audio.mp3" controls></audio>
```

### **Attributes for `<audio>` Tag**

- **src**: Specifies the path to the audio file.
- **controls**: Adds audio controls, like play, pause, and volume.
- **autoplay**: Automatically starts playing the audio when the page loads.
- **loop**: Repeats the audio once it ends.
- **muted**: Mutes the audio by default.
- **preload**: Specifies if and how the audio should be loaded when the page loads ('auto', 'metadata', 'none').

The "preload" attribute can have the following values:

1. `none`: This is the default value. It indicates that the browser should not preload the audio file at all. The audio file will only start downloading when the user initiates playback.
2. `metadata`: This value tells the browser to preload only the metadata of the audio file, such as its duration and basic information about the audio. This can be useful if you want to display the audio duration to the user without fully loading the audio data.
3. `auto`: This value instructs the browser to preload the entire audio file as much as possible without delaying the loading of other important page content. The browser will try to load the audio file in the background so that it's ready to play when the user decides to start it.

---

## **How to add favicon in HTML?**

nsert the following code in the `<head>` section of your `.html` file

```html
<link rel="icon" href="favicon.ico" type="image/x-icon">
```

---