# Links
* [Grid Garden - A game for learning CSS grid](https://cssgridgarden.com/)


TODO: 
* Checout best practice on website grid-template-areas

# Css grid
* Stucture: grid container and grid items
* All direct children of the grid container automatically become grid items.


## display
display: grid 
dipslay: inline-grid - For old browsers
XXX: difference 



## Properties of grid container
* column-gap
* row-gap
* gap



# Grid items properties
* Change column span 
```css
.item1 {
  grid-column-start: 1;
  grid-column-end: 3;
}
```

* Change row span
```css
.item1 {
  grid-row-start: 1;
  grid-row-end: 3;
}
```



# All properties
* Property	Description
* column-gap	Specifies the gap between the columns
* gap	A shorthand property for the row-gap and the column-gap properties
* grid	A shorthand property for the grid-template-rows, grid-template-columns, grid-template-areas, grid-auto-rows, grid-auto-columns, and the grid-auto-flow properties
* grid-area	Either specifies a name for the grid item, or this property is a shorthand property for the grid-row-start, grid-column-start, grid-row-end, and grid-column-end properties
* grid-auto-columns	Specifies a default column size
* grid-auto-flow	Specifies how auto-placed items are inserted in the grid
* grid-auto-rows	Specifies a default row size
* grid-column	A shorthand property for the grid-column-start and the grid-column-end properties
* grid-column-end	Specifies where to end the grid item
* grid-column-gap	Specifies the size of the gap between columns
* grid-column-start	Specifies where to start the grid item
* grid-gap	A shorthand property for the grid-row-gap and grid-column-gap properties
* grid-row	A shorthand property for the grid-row-start and the grid-row-end properties
* grid-row-end	Specifies where to end the grid item
* grid-row-gap	Specifies the size of the gap between rows
* grid-row-start	Specifies where to start the grid item
* grid-template	A shorthand property for the grid-template-rows, grid-template-columns and grid-areas properties
* grid-template-areas	Specifies how to display columns and rows, using named grid items
* grid-template-columns	Specifies the size of the columns, and how many columns in a grid layout
* grid-template-rows	Specifies the size of the rows in a grid layout
* row-gap	Specifies the gap between the grid rows



# Defining grid size


* four columns with same width (auto)
`grid-template-columns: auto auto auto auto;` 

* Custom size of first two columns. Rest is auto - fill container with same size
`grid-template-columns: 10px 50px auto auto;` 


* Define with fraction. In this case 1/4 of the screen per grid item. 
`grid-template-columns: 1fr 1fr 1fr 1fr;` 

* five grid items with 1/5 of the grid container
`grid-template-columns: repeat(5, 1fr)` 


# Defining min an max size
XXX: Nice 
* min 50px og maks 1fr (1/4 av skjermen)
```css
grid-template-rows: repeat(4, minmax(50px, 1fr))
```

# Align grid items
## justify-content and align-content

**Values**: 
* space-around
* space-evenly
* space-between
* center
* start
* end
 
 


# Grid items
**Defining item positions:**

## Grid column
* Make "item1" start on column 1 and end before column 5:
```css
.item1 {
  grid-column: 1 / 5;
}
```

* Make "item1" start on column 2 and span 3 columns:
```css
.item1 {
  grid-column: 2 / span 3;
}
```

## Grid row  
* `grid-row` 

## Grid area
* item property
* Kan brukes til å bytte plass på items




* Make "item8" start on row-line 1 and column-line 2, and end on row-line 5 and column line 6:
```css
.item8 {
  grid-area: 1 / 2 / 5 / 6;
}
```

* Make "item8" start on row-line 2 and column-line 1, and span 2 rows and 3 columns:
```css
.item8 {
  grid-area: 2 / 1 / span 2 / span 3;
}
```

## Grid template area - Define grid names
* Make "item1" span two columns and two rows (period signs represent items with no name):
```css
.item1 {
  grid-area: myArea;
}
.grid-container {
  grid-template-areas: 'myArea myArea . . .' 'myArea myArea . . .';
}
```


* Seksjoner i grid template area må være rektangulere. 
* Dtte fungerer ikke:
```css
grid-template-areas: 
"nav nav"
"main main"
"footer footer"
```


**More examples**

* by name
```css
.item1 { grid-area: header; }
.item2 { grid-area: menu; }
.item3 { grid-area: main; }
.item4 { grid-area: right; }
.item5 { grid-area: footer; }

.grid-container {
  grid-template-areas:
    'header header header header header header'
    'menu main main main right right'
    'menu footer footer footer footer footer';
}

```

* by col and row number
```css
.item1 { grid-area: 1 / 3 / 2 / 4; }
.item2 { grid-area: 2 / 3 / 3 / 4; }
.item3 { grid-area: 1 / 1 / 2 / 2; }
.item4 { grid-area: 1 / 2 / 2 / 3; }
.item5 { grid-area: 2 / 1 / 3 / 2; }
.item6 { grid-area: 2 / 2 / 3 / 3; }
```





