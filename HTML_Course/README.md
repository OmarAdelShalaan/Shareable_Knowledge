# HTML (HyperText Markup Language)

## Breakdown
- **"\<!DOCTYPE html>\":** Declares the document type as HTML5.
- **"\<html>\":** The root element that wraps all the HTML content.
- **"\<!-- -->"**: write comments in HTML that won't be displayed on the webpage.
- **"\<head>\":** Contains metadata, including the title of the document 
- **"\<title>\":** Specifies the title for the document.
- **"\<body>\":** Contains the content of the webpage that is visible to the user, like text, images, and more.
- **"\<h1>\":** A heading tag. In this case, it's the largest heading (h1 is for main headings, and h2 to h6 are for smaller subheadings).
- **"\<p>\":** A paragraph of text.
- **"\<a href="">\":**	Anchor (hyperlink), used to link to other pages or locations
- **"\<img>\":**	Embeds an image
- **"\<ul>\":** and **"\<li>\"**	Unordered list and list items
- **"\<ol>\":** and **"\<li>\"**	Ordered list and list items
- **"\<div>\":**	Generic container for content (often used for layout)
- **"\<span>\":**	Inline container for text or other inline elements
- **"\<strong>\":**	Bold text
- **"\<em>\":**	Italicized text
- **"\<table>\":**, **"\<tr>\"**, **"\<td>\"**	Tables, rows, and table data cells
- **"\<form>\":** collect user input using various input elements like text fields, radio buttons, checkboxes
- **"\<class>\":** used to assign one or more class names to an element. Classes are often used for styling with CSS or for manipulating elements with JavaScript.
- **"\<style>\":**  used to define internal CSS styles for a web page. It allows you to include CSS directly within your HTML document
- **"\<link>\":** used to link external resources to your document, most commonly for including external CSS stylesheets. It’s placed inside the <head> section of your HTML document.
- **"\<video>\":** add a video to your HTML page
- **"\<iframe>\":** used to embed another HTML document within the current document. This is often used to include content from other websites or to display media like videos.





## Example

### \<!DOCTYPE html>\: Declares the document type as HTML5.
```html
<!DOCTYPE html>
```

### \<html>: The root element that wraps all the HTML content.
```html
<html>
  <!-- All content goes here -->
</html>
```

### \<head>: Contains metadata, including the title of the document.
```html
<head>
  <title>My Webpage</title>
</head>
```

### \<title>: Specifies the title for the document.
```html
<title>My Webpage</title>
```

### \<body>: Contains the content of the webpage that is visible to the user, like text, images, and more.
```html
<body>
  <h1>Welcome to My Page</h1>
  <p>This is where all the visible content goes.</p>
</body>
```
<body>
  <h1>Welcome to My Page</h1>
  <p>This is where all the visible content goes.</p>
</body>


### \<h1>: A heading tag. In this case, it's the largest heading (h1 is for main headings, and h2 to h6 are for smaller subheadings).
```html
<h1>Main Heading</h1>
<h2>Subheading</h2>
```
<h1>Main Heading</h1>
<h2>Subheading</h2>

### \<p>: A paragraph of text.
```html
<p>This is a paragraph of text.</p>
```

<p>This is a paragraph of text.</p>


### \<a href="">: Anchor (hyperlink), used to link to other pages or locations.
```html
<a href="https://www.example.com">Click here to visit Example.com</a>
```
<a href="https://www.example.com">Click here to visit Example.com</a>

### \<img>: Embeds an image.
```html
<img src="image.jpg" alt="An example image">
```
<img src="OIP.jpg" alt="El-Araby">

### \<ul> and \<li>: Defines an unordered list and list items.
```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>

### \<ol> and \<li>: Defines an ordered list and list items.
```html
<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
</ol>
```
<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
</ol>

### \<div>: Generic container for content (often used for layout).
```html
<div>
  <p>This is inside a div element.</p>
</div>
```
<div>
  <p>This is inside a div element.</p>
</div>

### \<span>: Inline container for text or other inline elements.
```html
<p>This is a <span>highlighted</span> word in a sentence.</p>
```
<p>This is a <span>highlighted</span> word in a sentence.</p>

### \<strong>: Makes text bold.
```html
<p>This is <strong>bold</strong> text.</p>
```
<p>This is <strong>bold</strong> text.</p>

### \<em>: Italicizes text.
```html
<p>This is <em>italicized</em> text.</p>
```
<p>This is <em>italicized</em> text.</p>

### \<table>, \<tr>, \<td>: Defines tables, table rows, and table data cells.
```html
<table>
  <tr>
    <td>Row 1, Cell 1</td>
    <td>Row 1, Cell 2</td>
  </tr>
  <tr>
    <td>Row 2, Cell 1</td>
    <td>Row 2, Cell 2</td>
  </tr>
</table>
```
<table>
  <tr>
    <td>Row 1, Cell 1</td>
    <td>Row 1, Cell 2</td>
  </tr>
  <tr>
    <td>Row 2, Cell 1</td>
    <td>Row 2, Cell 2</td>
  </tr>
</table>


### \<form> collect user input using various input elements like text fields, radio buttons, checkboxes, etc. The \<form> element wraps all the form inputs.
```html
<form action="/submit" method="POST">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name">
  
  <label for="email">Email:</label>
  <input type="email" id="email" name="email">
  
  <input type="submit" value="Submit">
</form>
```

<form action="/submit" method="POST">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name">
  
  <label for="email">Email:</label>
  <input type="email" id="email" name="email">
  
  <input type="submit" value="Submit">
</form>


### \<class> attribute in HTML is used to assign one or more class names to an element. Classes are often used for styling with CSS or for manipulating elements with JavaScript.
```html
<p class="my-class">This is a paragraph with a class.</p>
<!-------OR ----->
<p class="class-one class-two">This paragraph has two classes.</p>
```

### \<style> used to define internal CSS styles for a web page. It allows you to include CSS directly within your HTML document
```html
<head>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f0f0f0;
    }
    h1 {
      color: navy;
      text-align: center;
    }
    p {
      color: darkgreen;
      line-height: 1.6;
    }
  </style>
</head>
<body>
  <h1>Welcome to My Webpage</h1>
  <p>This is a paragraph with some styling.</p>
</body>
```

<head>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f0f0f0;
    }
    h1 {
      color: navy;
      text-align: center;
    }
    p {
      color: darkgreen;
      line-height: 1.6;
    }
  </style>
</head>
<body>
  <h1>Welcome to My Webpage</h1>
  <p>This is a paragraph with some styling.</p>
</body>



### \<link> used to link external resources to your document, most commonly for including external CSS stylesheets. It’s placed inside the <head> section of your HTML document.
```html
<link rel="stylesheet" href="styles.css">
```

### \<video> add a video to your HTML page
```html
<video width="640" height="360" controls>
    <source src="video.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>
```
<video width="640" height="360" controls>
    <source src="https://youtu.be/WWj2VkQiVo4" type="video/mp4">
    Your browser does not support the video tag.
</video>


###  \<iframe> tag in HTML is used to embed another HTML document within the current document. This is often used to include content from other websites or to display media like videos.
```html
<iframe width="640" height="360" src="https://www.youtube.com/embed/WWj2VkQiVo4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
```
<iframe width="640" height="360" src="https://www.youtube.com/embed/WWj2VkQiVo4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


\
```html

```

\
```html

```

\
```html

```

\
```html

```
