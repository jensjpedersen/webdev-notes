
# Autocomplete in d3 is not working 

## CDN modules with d3
* Autocomplete is not working with d3

Current fix: 
```javascript
import * as d3 from "https://cdn.jsdelivr.net/npm/d3@7/+esm";
select = d3.select;
```



## FIX


* Autocomplete is not working with this import
```javascript
import * as d3 from "https://cdn.jsdelivr.net/npm/d3@7/+esm";
```



**FIX**

* this works: 
```html
<script src="https://d3js.org/d3.v7.min.js"></script>
```

* maybe need to install???: 
```bash
npm install @types/d3
```




    





