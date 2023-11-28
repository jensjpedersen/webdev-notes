

## Finding HTML Elements
* document.getElementById(id)	Find an element by element id
* document.getElementsByTagName(name)	Find elements by tag name
* document.getElementsByClassName(name)	Find elements by class name
* document.querySelector(selector) - Find the first element that matches a CSS selector
* document.querySelectorAll(selector) - Find all elements that match a CSS selector

# getElementById
* Kan hente et element fra et html dokument
* Id må først kjøres og defineres i html dokument

`const text = document.getElementById("text")` 


* skriv defer (kjører script etter at html er lastet inn)
```html
<script src=script.js defer></script>
```


# getElementsByTagName
`document.getElementsByTagName("tag")` 


# querySelector 
* returns the first element that matches a specified CSS selector(s) in the document.

## Complex Selectors
* Match `<input name="login"/> ` 
* located inside `<div class="user-panel main">` 

```javascript
const el = document.querySelector("div.user-panel.main input[name='login']");
```

## Select multiple elements
* select the first h3 and h4 element
```javascript 
document.querySelector("h3, h4").style.backgroundColor = "red";
```


# querySelectorAll
* Select all elements with class="example"
```javascript
document.querySelectorAll(".example");
```
