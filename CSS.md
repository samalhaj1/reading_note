

# what is CSS?

* CSS stands for **Cascading Style Sheets**.
* CSS describes how HTML elements are to be displayed on screen, paper, or in other media.
* CSS saves a lot of work. It can control the layout of multiple web pages all at once.
* External stylesheets are stored in CSS files.

# Why Use CSS?
**CSS** is used to define styles for your web pages, including the design, layout and variations in display for different devices and screen sizes.

**CSS Example**

body {

  background-color: lightblue;

}

h1 {

  color: white;

  text-align: center;

}

p {

  font-family: verdana;

  font-size: 20px;

}

# CSS Syntax

A **CSS** rule consists of a selector and a declaration block.

![css](https://www.w3schools.com/css/img_selector.gif)

* The selector points to the HTML element you want to style.

* The declaration block contains one or more declarations separated by semicolons.

* Each declaration includes a CSS property name and a value, separated by a colon.

* Multiple CSS declarations are separated with semicolons, and declaration blocks are surrounded by curly braces.

**Example**

p {

  color: red;

  text-align: center;

}

**Example Explained**

**p** is a selector in **CSS** (it points to the **HTML** element you want to style: <p>).

**color** is a **property**, and **red** is the **property value**

**text-align** is a **property**, and center is the **property value**

A CSS selector selects the HTML element(s) you want to style.


# CSS Selectors

**CSS selectors** are used to "find" (or select) the HTML elements you want to style.

We can divide CSS selectors into **five categories**:

#### Simple selectors
(select elements based on name, id, class)
#### Combinator selectors 
(select elements based on a specific relationship between them)
#### Pseudo-class selectors 
(select elements based on a certain state)
#### Pseudo-elements selectors 
(select and style a part of an element)
#### Attribute selectors 
(select elements based on an attribute or attribute value)

**Example**

Here, all <p> elements on the page will be center-aligned, with a red text color: 

p {

  text-align: center;

  color: red;

}

**The CSS id Selector**

The **id selector** uses the id attribute of an HTML element to select a specific element.

The **id of an element** is unique within a page, so the id selector is used to select one unique element!

To select an element with a specific id, **write a hash (#) character, followed by the id of the element.**

**Example**

The CSS rule below will be applied to the HTML element with id="para1": 

* #para1 {

  text-align: center;

  color: red;

}

**The CSS class Selector**

**The class selector** selects HTML elements with a specific class attribute.

To select elements with a specific class, **write a period (.) character, followed by the class name**.

**Example**

In this example all HTML elements with class="center" will be red and center-aligned: 

.center {

  text-align: center;

  color: red;

}

**The CSS Universal Selector**

**The universal selector** (*) selects all HTML elements on the page.

**Example**

The CSS rule below will affect every HTML element on the page: 

* {

  text-align: center;

  color: blue;

}

**The CSS Grouping Selector**

**The grouping selector** selects all the HTML elements with the same style definitions.

Look at the following CSS code **(the h1, h2, and p elements have the same style definitions)**:

h1 {

  text-align: center;

  color: red;

}


h2 {

  text-align: center;

  color: red;

}

p {

  text-align: center;

  color: red;

}

**It will be better to group the selectors, to minimize the code.**

**To group selectors, separate each selector with a comma.**

**Example**

In this example we have grouped the selectors from the code above: 

h1, h2, p {

  text-align: center;

  color: red;

}

### All CSS Simple Selectors

|Selector|	Example|	Example description|
|------- |   ------ |   -----------|
|#id	|#firstname|	Selects the element with id="firstname"|
|.class	|.intro	|Selects all elements with class="intro"|
|element.class|	p.intro|	Selects only <p> elements with class="intro"|
|*  |	 *  |	Selects all elements|
|element|	p	|Selects all <p> elements|
|element,element,..|	div, p|	Selects all <div> elements and all <p> elements|

# How To Add CSS
**When a browser reads a style sheet, it will format the HTML document according to the information in the style sheet.**

### Three Ways to Insert CSS
There are three ways of inserting a style sheet:

#### 1.  External CSS
#### 2. Internal CSS
#### 3.  Inline CSS


### External CSS

With an external style sheet, you can change the look of an entire website by changing just one file!

Each HTML page must include a reference to the external style sheet file inside the <link> element, inside the head section.

**Example**

***External styles are defined within the <link> element, inside the <head> section of an HTML page:***

* <!DOCTYPE html>


* <html>

* <head>

* <link rel="stylesheet" href="the name of the file">

* </head>

* <body>

* <h1>This is a heading</h1>

* <p>This is a paragraph.</p>

* </body>

* </html>

An external style sheet can be written in any text editor, and must be saved with a .css extension.

The external .css file should not contain any HTML tags.

Here is how the "mystyle.css" file looks:

"mystyle.css"

body {

  background-color: lightblue;

}

h1 {

  color: navy;

  margin-left: 20px;

}

**Note: Do not add a space between the property value and the unit (such as margin-left: 20 px;). The correct way is: margin-left: 20px;**

### Internal CSS

An internal style sheet may be used if one single HTML page has a unique style.


The internal style is defined inside the <style> element, inside the head section.

**Example**

Internal styles are defined within the <style> element, inside the <head> section of an HTML page:

* <!DOCTYPE html>

* <html>

* <head>

* <style>

*body {

  background-color: linen;

}

h1 {

  color: maroon;

  margin-left: 40px;

}

* </style>

* </head>

* <body>

* <h1>This is a heading</h1>

* <p>This is a paragraph.</p>


* </body>

* </html>

### Inline CSS

An inline style may be used to apply a unique style for a single element.

To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.

**Example**

Inline styles are defined within the "style" attribute of the relevant element:

* <!DOCTYPE html>

* <html>

* <body>

* <h1 style="color:blue;text-align:center;">This is a heading</h1>

* <p style="color:red;">This is a paragraph.</p>

* </body>

* </html>

**Tip: An inline style loses many of the advantages of a style sheet (by mixing content with presentation). Use this method sparingly.**






