


# Style
* Way to write css in d3




## Example


* Styling in html - BAD!
```html
<svg height="60" width="120">
  <rect width="10" x="10" height="20" y="15" style="fill: red;"></rect>
  <rect width="10" x="40" height="20" y="15" style="fill: green;"></rect>
  <rect width="10" x="70" height="20" y="15" style="fill: blue;"></rect>
</svg>
```


* Styling with attr - Better
```javascript: 
d3.selectAll("rect").attr('style' 'fill: red;');
```

* **styling with style - Best**
```javascript:
d3.selectAll("rect").style('fill', 'red');
```




