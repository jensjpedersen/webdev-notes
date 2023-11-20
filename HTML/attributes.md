
# Attributes 
* additional information about elements
* is always spesified in the start tag
* usually come in name/value pairs like: name="value"

**Good practices** - but not required
* good partice to use lowercase attributes
* quote attribute values. Also needed when using spaces in value. 

## Examples
**lang** - should always include | tag is <html>
* title - provides additional information about an element
* href - provides address of a link | tag is `<a>`
* width, height in pixels
* alt - alternate text for image -> if image is not displayed
* style - provides inline styling for an element: 
  * `<p style="color:red;">This is a paragraph.</p>`
### Src
* src - provides address of an image | tag is `<img>`

**Abosulte URL**
* full URL to the web page

**Relative URL**
* hosted in same domain as the current page

Use relative URL. They wil not break if you change domain. 

### Lang
* Should always include language attribute
`<html lang="en">`
* Can always inlcude country: 
`<html lang="en-US">`


### Title 
* The title attribute defines some extra information about an element.
* The value of the title attribute will be displayed as a tooltip when you mouse over the element:
