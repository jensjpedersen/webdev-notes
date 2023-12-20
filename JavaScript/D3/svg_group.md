
# Svg group elements
* Usful for grouping elements together


Use the `<g>` element to group SVG shapes together. Once grouped you can
transform the whole group of shapes as if it was a single shape. This is useful
when you want to apply the same property to multiple shapes.

```xml
<svg width="400" height="400">
    <g>
    
    <--! Elements inside ere kan be targeted by selectAll in d3 -->
    
    </g>
</svg>
```


* The d3 selectAll method is restricted to the children of the `<g>` element

