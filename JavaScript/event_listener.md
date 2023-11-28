
# Event listener

* The addEventListener() method attaches an event handler to the specified element.
* Can attach many event handlers to one element.
* Can add many event handlers of the same type to one element, i.e two "click" events.
* You can add event listeners to any DOM object not only HTML elements. i.e the window object.


**Syntax**
```javascript
element.addEventListener(event, function, useCapture);
```

**Parameters:**
* event - type of the event (like "click" or "mousedown" or any other HTML DOM Event.)
* function - the function we want to call when the event occurs.
* useCapture - The third parameter is a boolean value specifying whether to use
  event bubbling (`default = false`) or event capturing. This parameter is optional.


## Example
```javascript
document.getElementById("myBtn").addEventListener("click", displayDate);
```

## Event Bubbling or Event Capturing?
Defines the order of event firing when an element is nested inside another
element, and both elements have registered a handler for the same event.

### Example
* Example: div_inner inside div_outer

**Event Bubbling**
* If you click on the inner element (div_inner), the click event fires first on
  the inner element, then on the outer element (div_outer).

**Event Capturing**
* If you click on the inner element (div_inner), the click event fires first on
  the outer element (div_outer), then on the inner element (div_inner).




# Register key press

```javascript
document.addEventListener("key)

document.addEventListener("keydown", function(e) {
        if (e.key === "ArrowUp") {
            // Do something

        
        }
    }
    
```


# Common events
* list of alle dom events: [HTML DOM Event Object](https://www.w3schools.com/jsref/dom_obj_event.asp)
* Click Event - Triggered when a mouse or pointing device button is pressed and released on an element.
* Mouseover and Mouseout Events - Triggered when the mouse pointer enters or leaves an element.
* Keydown, Keypress, and Keyup Events - Triggered when a keyboard key is pressed, held down, or released, respectively.
* Change Event - Triggered when the value of an <input>, <select>, or <textarea> element changes.
* Submit Event - Triggered when a form is submitted.
* Load Event - Triggered when a resource and its dependent resources have finished loading.


# Remove event Listener
* old event listeners is not overwritten by new event listeners. To Remove an event listener, use: 
`removeEventListener()` 
