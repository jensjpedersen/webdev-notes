
* **Best practice to use rem for font-size**

# Absolute length units

## pixel
* **Pixel is unit of length**
* In CSS, 1 pixel is formally defined as 1/96 of an inch. 
* DPI (dots per inch) 

* Screens on modern devices have much higher resolutions and DPIs, so a line that's 96 pixels long may not measure exactly 1 inch, depending on the device.


# Relative length units


## em
**Relative to parent**
When used with the font-size property, em inherits the font-size from its parent element:

### Example
```css
.container {
  font-size: 16px;
}

.container p {
  font-size: 1em;
}

.container h2 {
  font-size: 3em;
}

.container h3 {
  font-size: 2em;
}
```

In this example, the font-size of p is 16px (16 * 1). Meanwhile, the font-size
of h2 is 48px (16 * 3), and 32px for the h3 (16 * 2).


## rem  
**Realtive to root**

* If a user changes their browser's default font size, then the font-size of p will scale up or down accordingly.
### Example
```css
p {
  font-size: 1.25rem;
}
```


In most browsers, the default font size is 16, so the font-size of html
elements is 16px. So in this case, p is 20px (16 * 1.25).

## %
* **Percentages of the parent element**
* Percentages, or the percent size relative to the parent's size:

## vw
* View width. 1vw is 1% of the width of the viewport.
* Will resize of you resize the browser window

## vh
* View height. 1vh is 1% of the height of the viewport.


## vmin and vmax
* 1vmin is 1% of the viewport's smallest dimension
* 1vmax is 1% of the viewports largest dimension.

