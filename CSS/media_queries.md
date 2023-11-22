TODO: 
* not|only 
* meta tag -  

# Tips
* use clamp for responsive sizing
* resize margin with media queries

# Viewport meta tag
* Include in the `<head>` section of the HTML document
XXX?? - what does it do 
* Include viewport meta tag to make media queries work on mobile devices 
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
The viewport meta tag is crucial for making web pages responsive on different
devices. It helps ensure that the content adapts to the screen size and
provides a consistent user experience across various devices, such as desktops,
tablets, and smartphones.


# Media Queries
* It uses the @media rule to include a block of CSS properties only if a certain condition is true.
* Media queries allow you to apply CSS styles depending on a device's general
  type (such as **print** vs. **screen**) or other characteristics such as screen
  resolution or browser viewport width.


# Syntax

```css
@media not|only mediatype and (media feature) {
    CSS-Code;
}
```
* only (default): Not necessary. Mainly used to prevent older browsers that don't
  support media queries from applying the styles within the @media rule. In
  modern browsers, removing only won't have a significant impact.
* mediatype: all, print, screen, speech
* media feature: width, height, orientation, aspect-ratio, resolution, etc.


## Common example
* Feature is applied until when size >= 481px
```css
$media screen and (min-width: 481px) {
    // css code
}
```
# Media features
**Media features**
* min-width
* orientation: portrait or landscape
* min-aspect-ratio: min width / min height
* etc. 

# Operators
* `not | and | only` - Logical operators can be used to compose a complex media query
* `,` - You can also combine multiple media queries into a single rule by
separating them with commas.

# Targeting
## Targeting media types
* target multiple devices - `$media screen, print { ... }` 

## Targeting media features
* "min-" or "max-" prefix can be used to target range features: `max-width, min-width` 

## Targeting examples
* `and` - To combine multiple features - `@media (min-width: 30em) and (orientation: landscape) {}` 
* To limit the styles to devices with a screen, you can chain the media
    features to the screen media type: 
    `@media screen and (min-width: 30em) and (orientation: landscape) { }` 
* `,` - to match any of various media types, features, or states: 
    `@media (min-height: 680px), screen and (orientation: portrait) { }` 


# Example - Responsive Web Design
* Mobile first - Design from small to large. Hence, use `min-width`  instead of
  `max-width`. 


```css
/* For mobile phones: */
[class*="col-"] {
  width: 100%;
}

@media only screen and (min-width: 768px) {
  /* For desktop: */
  .col-1 {width: 8.33%;}
  .col-2 {width: 16.66%;}
  .col-3 {width: 25%;}
}

@media only screen and (min-width: 600px) {
  /* For tablets: */
  .col-s-1 {width: 8.33%;}
  .col-s-2 {width: 16.66%;}
  .col-s-3 {width: 25%;}
}

@media only screen and (min-width: 768px) {
  /* For desktop: */
  .col-1 {width: 8.33%;}
  .col-2 {width: 16.66%;}
  .col-3 {width: 25%;}
}
```


# How to decide on breakpoints
**Typical device breakpoints**
```css
/* Extra small devices (phones, 600px and down) */
@media only screen and (max-width: 600px) {...}

/* Small devices (portrait tablets and large phones, 600px and up) */
@media only screen and (min-width: 600px) {...}

/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (min-width: 768px) {...}

/* Large devices (laptops/desktops, 992px and up) */
@media only screen and (min-width: 992px) {...}

/* Extra large devices (large laptops and desktops, 1200px and up) */
@media only screen and (min-width: 1200px) {...}
```


