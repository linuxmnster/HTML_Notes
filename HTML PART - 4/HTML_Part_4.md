# HTML_Part_4

---

## HTML Tables

HTML tables allow you to arrange data like text, images, and links in rows and columns. You use the `<table>` tag to start and end a table.

## **Key Elements of HTML Table**

- `<table>`: Defines the table itself.
- `<tr>`: Used for table rows.
- `<th>`: Used for table headings.
- `<td>`: Used for table cells (data).
- `<caption>` : Used to set caption for table

```html
<table>
	<captioin>Personal info</caption>
	<tr>
		<th>Name</th>
		<th>Age</th>
	</tr>
	<tr>
		<td>Chandu</td>
		<td>18</td>
	</tr>
</table>
```

---

## Rowspan & Colspan attributes

**Rowspan:** If you want a table cell to span multiple rows, you can use the `rowspan` attribute.
**Colspan:** If you want a table cell to span multiple columns, you can use the `colspan` attribute.

![colspan-rowspan.png](colspan-rowspan.png)

### **Example for Colspan :**

```html
<table border="1">
	<tr>
		<td colspan="2">Merged columns</td>
	</tr>
	<tr>
		<td>column 1</td>
		<td>column 2</td>
	</tr>
</table>
```

### **Example for Rowspan :**

```html
<table border="1">
	<tr>
		<td>row1, column1</td>
		<td rowspan="2">Merged rows</td>
	<tr>
	<tr>
		<td>row2, column2</td>
	<tr>
</table>
```

---

## Column Groups

You can use the <column> and <col> elements to apply styles to an entire column in an HTML table

```html
<style>
    .batman {
        background-color: #d7d9f2;
    }

    .flash {
    background-color: #ffe8d4;
    }
</style>
<table>
    <caption>
      Superheros and sidekicks
    </caption>
    <colgroup>
      <col />
      <col span="2" class="batman" />
      <col span="2" class="flash" />
    </colgroup>
    <tr>
      <td></td>
      <th scope="col">Batman</th>
      <th scope="col">Robin</th>
      <th scope="col">The Flash</th>
      <th scope="col">Kid Flash</th>
    </tr>
    <tr>
      <th scope="row">Skill</th>
      <td>Smarts, strong</td>
      <td>Dex, acrobat</td>
      <td>Super speed</td>
      <td>Super speed</td>
    </tr>
  </table>
```

---

## Table Semantics in HTML

**Table Headers and Footers**

Besides `<th>` for individual header cells, HTML tables allow you to group header or footer content using `<thead>` and `<tfoot>`.

```html
<table>
  <thead>
     <!--  header content -->
  </thead>
  <tfoot>
  <!-- footer content -->
  </tfoot>
  <tbody>
  <!-- body content -->
  </tbody>
</table>
```

---

### Introduction to HTML forms

### Why do we use forms ?

HTML forms are essential for collecting user input on web pages. Whether it's a search bar, a login screen, or a multi-field registration form, HTML forms play a key role in web interactions. They enable users to submit data, which can be processed, stored, or returned by a server.

orms serve as the gateway between the user and the server, allowing for dynamic, interactive web experiences. They are crucial for tasks such as user authentication, data submission, feedback collection, and more. Simply put, forms make websites more engaging and functional.

---

## <form> Elemennt

The HTML `<form>` element is used to create an HTML form for user input

The `<form>` element is a container for different types of input elements, such as: text fields, checkboxes, radio buttons, submit buttons, etc.

```html
<form>
	<!-- form elements -->
</form>
```

## The action attribute

The `action` attribute defines the action to be performed when the form is submitted.

`action attribute` is used to define what action need to be performed when a form is submitted or where the form data should be sent.

```html
<form acitoin="/action.php">
	<!-- form elements -->
</form>
```

**Tip:** If the `action` attribute is omitted, the action is set to the current page.

---

## Input Elements

Input types in HTML forms are the backbone of interactive web applications. They allow users to send information to web servers for various purposes like searching, logging in, or providing feedback. In this blog, we'll explore common HTML input types: text, password, radio, and checkbox.

## The type attribute

The type attribute is used to define the type of input that is taken from the user

By default the type is set to text area

```html
<form action="/action.php">
	<input type="text">Text area</input>
</form>
```

| text | Allows the user to type a single line of text. |
| --- | --- |
| password | Allows the user to type a password. |
| submit | Represents a button that, when pressed, submits the form. |
| reset | Represents a button that, when pressed, resets all the form controls to their initial values. |
| radio | Represents an option in a set of options that are mutually exclusive with each other. |
| checkbox | Represents an option in a set that may be selected independently of other options. |
| button | Represents a clickable button. |
| color | Allows the user to select a color. |
| date | Allows the user to select a date. |
| datetime-local | Allows the user to select a date and time with no time zone. |
| email | Allows the user to enter an email address. |
| file | Allows the user to select one or more files from their device storage. |
| hidden | Represents a value that is not displayed but is submitted to the server. |
| image | Defines an image that acts as a submit button. |
| month | Allows the user to select a month and year. |
| number | Allows the user to enter a number. |
| range | Allows the user to select a number from a range. |
| search | Allows the user to enter a search query string. |
| tel | Allows the user to enter a telephone number. |
| time | Allows the user to select a time. |
| url | Allows the user to enter a URL. |
| week | Allows the user to select a week. |

## Name attribute

A string specifying a name for the input control. This name is submitted along with the control's value when the form data is submitted.

Consider the `name` a required attribute (even though it's not). If an input has no `name` specified, or `name` is empty, the input's value is not submitted with the form! (Disabled controls, unchecked radio buttons, unchecked checkboxes, and reset buttons are also not sent.)

```html
<form action="https://www.youtube.com/results">
	<label for="youtube"></label>
	<input type="text" placeholder="search" id="youtube" name="search_query"></input>
	<input type="submit" value="search"></input>
</form>
```

## Placeholder attribute

The input `placeholder` attribute specifies a short hint that describes the expected value of an input field (a sample value or a short description of the expected format).

```html
<form>
	<input type="text" placeholder="Username">Username : </input>
	<input type="password" placeholder="Password">Password : </input>
</form>
```

---

## <label> Element

<label> element represents a a caption for an item in a user interface

```html
<form action="action.php">
	<label for="Username">Username</label>
	<input type="text" placehlder="username" id="Username"></input>
	
	<label for="Password">Password</label>
	<input type="password" placeholder="password" id="Username"></input>
	
	<input type="submit"></input>
</form>
```

---

## <button> Element

The `<button>` tag defines a clickable button

**Tip:** Always specify the `type` attribute for a `<button>` element, to tell browsers what type of button it is.

```html
<button type="submit"><button>
```

### type attribute values

| button | sets as a butto |
| --- | --- |
| reset | resets the form |
| submit | default type |

### Input as type button

```html
<form action="action.php">
	<label for="search">Search</label>
	<input type="button" if="search" value="click me!"></input>
</form>
```

---

## Checkbox - Input Element :

The **HTML `<input type=”checkbox”>` tag** is used to define the square boxes. It is a form element which allows users to select one or more options from the given options.

```html
<fieldset>
        <legend>choose your subject</legend>
        <form action="action.php">
            <label for="mat">mat</label>
            <input type="checkbox" id="mat" name="sub" value="mat" checked>
            <br>
            <label for="phy">phy</label>
            <input type="checkbox" id="phy" name="sub" value="phy" checked>
            <br>
            <label for="che">che</label>
            <input type="checkbox" id="che" name="sub" value="che" checked>
            <br>            
            <button type="submit">submit</button>
        </form>
    </fieldset>
```

---

## Radio buttons - Input Element :

HTML **`<input type=”radio”>`** creates a radio button input field allowing users to select one option from multiple choices. Only one radio button in a group can be selected at a time.

```html
<fieldset>
        <legend>choose your Favorite Fruit</legend>
        <form action="action.php">
            <label for="apple">Apple</label>
            <input type="radio" name="fruit" id="apple" value="apple">
            <br>
            <label for="mango">Mango</label>
            <input type="radio" name="fruit" id="mango" value="mango">
            <br>
            <label for="banana">Banana</label>
            <input type="radio" name="fruit" id="banana" value="banana">
            <br>
            <button type="submit">submit</button>
        </form>
    </fieldset>
```

### Note :

if you want to group any sectoin set name attribute value same for all the other options that are belong to the same section or else we can select all the radio buttons

---

## **HTML <select> Tag**

The **<select> tag** in HTML is used to create a drop-down list. The <select> tag contains <option> tag to display the available option of the drop-down list.

```html
<fieldset>
        <legend>choose your Favorite Fruit</legend>
        <form action="action.php">
            <select name="role" id="profession">
                <option>--Select Your Option--</option>
                <option value="stu">Student</option>
                <option value="dev" selected>Developer</option>
            </select>
            <button type="submit">submit</button>
        </form>
    </fieldset>
```

---

## Range - Input Element :

The `<input type="range">` defines a control for entering a number whose exact value is not important (like a slider control).

Default range is 0 to 100. However, you can set restrictions on what numbers are accepted with the attributes below.

- [max](https://www.w3schools.com/tags/att_input_max.asp) - specifies the maximum value allowed
- [min](https://www.w3schools.com/tags/att_input_min.asp) - specifies the minimum value allowed
- [step](https://www.w3schools.com/tags/att_input_step.asp) - specifies the legal number intervals
- [value](https://www.w3schools.com/tags/att_input_value.asp) - Specifies the default value

**Tip:** Always add the [`<label>`](https://www.w3schools.com/tags/tag_label.asp) tag for best accessibility practices!

```html
<form action="server">
	<label for="val">select range</label>
	<input type="range" min="0" max="100" step="10" value="0" name="range">
</form>
```

---

## **Textarea Element :**

The `textarea` element is used when you need multiline text input from the user. This is particularly useful for comments, reviews, or any other type of input where the length is unpredictable.

```html
<label for="story">Tell us your story:</label>

<textarea id="story" name="story" rows="5" cols="33" placeholder="type here!">
</textarea>

```

---