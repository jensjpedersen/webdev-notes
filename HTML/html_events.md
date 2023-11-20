
# Onclick
* call a js function when a button is clicked
```html
<button onclick="myFunction()">Click me</button>
```

syntax:
* onclick value = js code



# Mouse events
onclick - The user clicks on an element
oncontextmenu - The user right-clicks on an element
ondblclick - The user double-clicks on an element
onmousedown - A mouse button is pressed over an element
onmouseenter - The pointer is moved onto an element
onmouseleave - The pointer is moved out of an element
onmousemove - The pointer is moving over an element
onmouseout - The mouse pointer moves out of an element
onmouseover - The mouse pointer is moved over an element
onmouseup - The mouse button is released over an element



# Examples
## Onclick - Set element value in html
Click a <button> to display the date:


* onclick value = js code
```html
<button onclick="getElementById('demo').innerHTML=Date()">What is the time?</button>
<p id="demo"></p>
```

## Inline js 
* `document ` refers to the current html document
```html
<h3 id="demo" onclick="myFunction()">Click me to change my color.</h3>

<script>
function myFunction() {
  document.getElementById("demo").style.color = "red";
}
</script>
```


