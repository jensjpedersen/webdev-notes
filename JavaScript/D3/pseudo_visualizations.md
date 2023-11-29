

# EP2 - Pseudo visualisations - Aproximating visualisations




# Sudo plots
## Sudo scatter plot
1. comprised of circles
2. position circles in a frame 
3. Can export svg file and copy svg code into html file

## Sudo bar chart
* place rectangles in a frame

## Line chart 





# Precedence of SVG attributes and Styles 
* Attribute: 
```html
<rect x="0" y="0" width="100" height="100" fill="red" stroke="black"/>
```

All css (inline, internal and external style sheet) takes precedence over SVG attributes.

* Inline css: 
```html
<rect x="0" y="0" width="100" height="100" style="fill: blue;" stroke="black"/>
```


This rect is blue, not red: 
```html
<rect x="0" y="0" width="100" height="100" style="fill: blue;" fill="red" stroke="black"/>
```

