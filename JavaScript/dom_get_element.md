

## Finding HTML Elements
* document.getElementById(id)	Find an element by element id
* document.getElementsByTagName(name)	Find elements by tag name
* document.getElementsByClassName(name)	Find elements by class name

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
