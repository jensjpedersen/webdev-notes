
# Example on svg mask
* Is used to hide and show parts of SVG elements


Remember: 
* url and id 
```html
<svg viewBox="-10 -10 120 120">

  <!-- Image to be masked -->
  <circle cx="50" cy="50" r="50" fill="purple" mask="url(#myMask)" />
  
  <mask id="myMask">
    <!-- Everything under a white pixel will be visible -->
    <!-- big rectangele -->
    <rect x="10" y="0" width="100" height="100" fill="white" />

    <!-- Everything under a black pixel will be hidden -->
    <!-- samll rectangele -->
    <rect x="25" y="25" width="50" height="50" fill="black" />

  </mask>

</svg>
```


![SVG mask](Figures/svg_mask.png)

