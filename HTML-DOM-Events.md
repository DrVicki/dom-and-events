HTML DOM allows JavaScript to react to HTML events.

## Reacting to Events

A JavaScript can be executed when an event occurs, like when a user clicks on an HTML element.

To execute code when a user clicks on an element, add JavaScript code to an HTML event attribute:

`onclick=JavaScript`

Examples of HTML events:

  - When a user clicks the mouse
  - When a web page has loaded
  - When an image has been loaded
  - When the mouse moves over an element
  - When an input field is changed
  - When an HTML form is submitted
  - When a user strokes a key

In this example, the content of the `<h1>` element is changed when a user clicks on it:

**Example**

```
<!DOCTYPE html>
<html>
<body>

<h1 onclick="this.innerHTML = 'Ooops!'">Click on this text!</h1>

</body>
</html>
```

[Let's Try It](https://www.w3schools.com/js/tryit.asp?filename=tryjs_event_onclick2)

In this example, a function is called from the event handler:

**Example**

```
<!DOCTYPE html>
<html>
<body>

<h1 onclick="changeText(this)">Click on this text!</h1>

<script>
function changeText(id) {
  id.innerHTML = "Ooops!";
}
</script>

</body>
</html>
```

[Let's Try it](https://www.w3schools.com/js/tryit.asp?filename=tryjs_event_onclick3)

### HTML Event Attributes

To assign events to HTML elements you can use event attributes.

**Example**

Assign an `onclick` event to a `button` element:

`<button onclick="displayDate()">Try it</button>`

[Let's Try It](https://www.w3schools.com/js/tryit.asp?filename=tryjs_events1)

In the example above, a function named `displayDate` will be executed when the button is clicked.

### Assign Events Using the HTML DOM

The HTML DOM allows you to assign events to HTML elements using JavaScript:

**Example**

Assign an `onclick` event to a `button` element:

```
<script>
document.getElementById("myBtn").onclick = displayDate;
</script>
```
[Let's Try It](https://www.w3schools.com/js/tryit.asp?filename=tryjs_events2)

### The onload and onunload Events

The `onload` and `onunload` events are triggered when the user enters or leaves the page.

The `onload` event can be used to check the visitor's browser type and browser version, and load the proper version of the web page based on the information.

The `onload` and `onunload` events can be used to deal with cookies.

**Example**

`<body onload="checkCookies()">`

[Let's Try It](https://www.w3schools.com/js/tryit.asp?filename=tryjs_events_onload)

