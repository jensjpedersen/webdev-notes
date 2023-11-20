
# Links
* [Flexbox Froggy - A game for learning CSS flexbox](https://flexboxfroggy.com/)
* [Flexbox Defense](http://www.flexboxdefense.com/)

# Trouble shooting 
## To small container
* Problem: body dekker ikke hele høyden, derfor vil ikke flex boxen bli sentrert på høyden.
* bruk derfor min-height: 100vh; på body




# Flex container
* used for css positioning
* need to spesifcy flex container
* **flex properties are applied to the element's in the flex container.**
* The Flexible Box Layout Module, makes it easier to design flexible responsive layout structure without using float or positioning.


```html
<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>
</div>
```

# Flex container properties
* flex-direction - direction to stack items - reverse order is possible
    * row-reverse - reverse order of items and place at end
* flex-wrap - wrap items to new line - values: wrap, wrap-reverse, nowrap
* flex-flow - shorthand for flex-direction and flex-wrap: `flex-flow: row wrap;`  

**Justify-content and align-itmes** - same values but differnet axis. 
* justify-content - align items along the main axis. Does not affect spacing between items. - Only spacing along the 
    * values: flex-start, flex-end (end of container), center, space-between (between items) , space-around (between and around items), space-evenly

* align-items - align items along the cross axis:
    * values: 

* align-content - aligns lines of content along the cross axis. Only works if there are multiple lines of content. 
    * values: flex-start, flex-end, center, space-between, space-around, stretch

## align-content - 
* **how multiple lines are spaced apart from each other.**
* VS: align-items and justify-content - works on individual items
* **Does affect spacing between lines (rows/columns).**

Values: 
* flex-start (alias = start): Lines are packed at the top of the container.
* flex-end (alias = end): Lines are packed at the bottom of the container.
* center: Lines are packed at the vertical center of the container.
* space-between: Lines display with equal spacing between them.
* space-around: Lines display with equal spacing around them.
* stretch: Lines are stretched to fit the container.




# Flex elemnt
Består av:
* flex-container 
* flex-items



# Assign properties to flex items

## flex: value
* endre størrelse på et spesifikt flex item
* sett `flex: 50%` for at et bestem item skal ta 50% av bredden til flex containeren (parent).

## Order
* order - values (default 0) - Can use to reorder items
    * value: 1 - less priority, higher value lower priority - place to the right
    * value: -1 - higher priority - place to the left

## Align-self
* align induvidual items
* Same values as align-items
* Overides align-items


```css
#pond {
  display: flex;
  align-items: flex-start;
}

.yellow {
align-self: end; 
}
```

