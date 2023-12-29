
# Import d3

* specify the type as module
```html
<script type="module" src="script.js"></script>
```

* in script.js 
```javascript
import * as d3 from "https://cdn.jsdelivr.net/npm/d3@7/+esm";
```


# Import in node

* `npm install d3` 

* in script.js
```javascript
import * as d3 from "d3";
```
XXX: Canvases are not supported in node.js



