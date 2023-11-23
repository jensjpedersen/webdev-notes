

# Source js file in html
* in head add: 

```html
<script src="script.js" defer></script>
```
* Remeber to add defer attribute to script tag, so that the script is executed
  after the page has finished parsing.

# Get element by id

```javascript
document.getElementById("demo").innerHTML =
"Hello Dolly!";
```





