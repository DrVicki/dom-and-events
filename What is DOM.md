# The HTML DOM (Document Object Model)

When a web page is loaded, the browser creates a Document Object Model of the page.

The **HTML DOM** model is constructed as a tree of Objects:

![](https://www.w3schools.com/js/pic_htmltree.gif)
## What is the DOM?

The DOM is a W3C (World Wide Web Consortium) standard.

The DOM defines a standard for accessing documents:

 > "The W3C Document Object Model (DOM) is a platform and language-neutral interface that allows programs and scripts to dynamically access and update the content, structure, and style of a document."

The W3C DOM standard is separated into 3 different parts:

  1. Core DOM - standard model for all document types
  2. XML DOM - standard model for XML documents
  3. HTML DOM - standard model for HTML documents
  
## What is the HTML DOM?
The HTML DOM is a standard object model and **programming interface** for HTML. It defines:

  - The HTML elements as objects
  - The properties of all HTML elements
  - The methods to access all HTML elements
  - The events for all HTML elements

In other words: **The HTML DOM is a standard for how to get, change, add, or delete HTML elements.**

# JavaScript - HTML DOM Methods

HTML DOM methods are **actions** you can perform (on HTML Elements).

HTML DOM properties are **values** (of HTML Elements) that you can set or change.

## The DOM Programming Interface

The HTML DOM can be accessed with JavaScript (and with other programming languages).

In the DOM, all HTML elements are defined as **objects**.

The programming interface is the properties and methods of each object.

 - A **property** is a value you can get or set (like changing the content of an HTML element).

 - A **method** is an action you can do (like add or deleting an HTML element).

### Example

The following example changes the content (the `innerHTML`) of the `<p>` element with `id="demo":`

```
<html>
<body>

<p id="demo"></p>

<script>
document.getElementById("demo").innerHTML = "Hello World!";
</script>

</body>
</html>
```

[Let's Try It](https://www.w3schools.com/js/tryit.asp?filename=tryjs_dom_method)

In the example above, `getElementById` is a **method**, while `innerHTML` is a **property**.

## The getElementById Method

The most common way to access an HTML element is to use the `id` of the element.

 - In the example above the `getElementById` method used `id="demo"` to find the element.

## The innerHTML Property

The easiest way to get the content of an element is by using the `innerHTML` property.

 - The `innerHTML` property is useful for getting or replacing the content of HTML elements.

 > The innerHTML property can be used to get or change any HTML element, including <html> and <body>.

## Finding HTML Elements

Often, with JavaScript, you want to manipulate HTML elements.

To do so, you have to find the elements first. There are several ways to do this:

 - Finding HTML elements by id
 - Finding HTML elements by tag name
 - Finding HTML elements by class name
 - Finding HTML elements by CSS selectors
 - Finding HTML elements by HTML object collections

### Finding HTML Element by Id

The easiest way to find an HTML element in the DOM, is by using the element id.

This example finds the element with ```id="intro":```

**Example**

```
const element = document.getElementById("intro");
 ```
[Let's Try It](https://www.w3schools.com/js/tryit.asp?filename=tryjs_dom_getelementbyid)
 
If the element is found, the method will return the element as an object (in element).

If the element is not found, element will contain `null`.
 
### Finding HTML Elements by Tag Name

 This example finds all `<p>` elements:

**Example**

```
const element = document.getElementsByTagName("p");
```
[Let's Try It](https://www.w3schools.com/js/tryit.asp?filename=tryjs_dom_getelementsbytagname2)
 
This example finds the element with `id="main"`, and then finds all `<p>` elements inside `"main"`:

**Example**

```
const x = document.getElementById("main");
const y = x.getElementsByTagName("p");
```
 
[Let's Try It](https://www.w3schools.com/js/tryit.asp?filename=tryjs_dom_getelementsbytagname)
 
## Finding HTML Elements by Class Name

If you want to find all HTML elements with the same class name, use `getElementsByClassName()`.

This example returns a list of all elements with `class="intro"`.

**Example**
```
const x = document.getElementsByClassName("intro");
```
[Let's Try It](https://www.w3schools.com/js/tryit.asp?filename=tryjs_dom_getelementsbyclassname)

## Finding HTML Elements by CSS Selectors

If you want to find all HTML elements that match a specified CSS selector (id, class names, types, attributes, values of attributes, etc), use the `querySelectorAll()` method.

This example returns a list of all `<p>` elements with `class="intro"`.
 
**Example**

```
const x = document.querySelectorAll("p.intro");
```
[Let's Try It](https://www.w3schools.com/js/tryit.asp?filename=tryjs_dom_queryselectorall)
