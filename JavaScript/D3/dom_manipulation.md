
# EP3 - DOM manipulation




## Creating SVG from javascript
SVG is XML-based, **therfore**; 
* SVG can not be created with the document.createElement() method. 



```javascript
const svg = docuemnt.createElementNS('http://www.w3.org/2000/svg', 'svg');
svg.setAttribute('width', 500);
svg.setAttribute('height', 500);
document.body.appendChild(svg);
```


* Create a rectange inside the svg element
```javascript
const rect = docuemnt.createElementNS('http://www.w3.org/2000/svg', 'rect');
rect.setAttribute('width', 500);
rect.setAttribute('height', 500);
svg.appendChild(svg);
```


## SVG mask
* defines an alpha mask for compositing the current object into the background


```javascript
const mask = docuemnt.createElementNS('http://www.w3.org/2000/svg', 'mask');
```




