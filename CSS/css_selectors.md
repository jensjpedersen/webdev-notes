
* In CSS, selectors are patterns used to select the element(s) you want to style.

# Css selector

## Grouping selectors
* You can group selectors to apply the same styles to several selectors.
```css
h1, h2, p {
  text-align: center;
  color: red;
}
```


# Class
* The class selector selects elements with a specific class attribute.
* To select elements with a specific class, write a period (.) character, followed by the name of the class.

## Class
```css
.intro {
  background-color: yellow;
}
```

In html the class is referenced as: 
```html
<div class="intro">Some text</div>
```


## Style tag with a class

```css
p.hometown { 
  background: yellow;
}

```

* This elemetns is styled:
<p class="hometown">I live in Ducksburg.</p> 

* This elements is not styled
<p>My name is Donald.</p>


## Comaprison of the two above
Key difference is that element.classname narrows down the selection to div elements
with the specified class, while .classname selects all elements with the
specified class, **regardless of their element type.**


# Multiple calsses
* Style with center and large class

```html
<p class="center large">This paragraph refers to two classes.</p>
```



# Id
Style the element with id="firstname":
```css
#firstname {
  background-color: yellow;
}
```


# Style all elements

* Select all elements, and set their background color to yellow:
```css
* {
    background-color: yellow;
}
```


# Style nested elements


* Styles all elements inside div to yellow
```css
div * {
    background-color: yellow;
}
```

* Style elements inside another element:  
```css
element element {
  css declarations;
}

```





# Element in another element
## Style element inside another element
```css
element, element {
  css declarations;
}
```

## Style element2 with element1 as parent

```css
div > p {
  background-color: yellow;
}
```

**Differnece between two above**
So, the key difference is that div > p selects only immediate child p elements
of a div, while div p selects all p elements that are descendants of a div,
whether they are immediate children or nested deeper within the structure.


# Continue from here on css styling
XXX: Differnece between id and class
XXX: 
[CSS element+element Selector](https://www.w3schools.com/cssref/sel_element_pluss.php)
