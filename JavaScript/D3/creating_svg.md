


# Create SVG


## Vanilla JS
```javascript
const svg = document.createElementNS('http://www.w3.org/2000/svg', 'svg');

svg.setAttribute('width', '100');
svg.setAttribute('height', '100');
document.body.appendChild(svg);
```

## D3 without method chaining
```javascript
const svg = d3.select('body').append('svg')

svg.attr('width', '100')
svg.attr('height', '100');
```

## D3 with medthod chaining

```javascript
const svg = d3.select('body')
  .append('svg')
  .attr('width', '100')
  .attr('height', '100');
```

