TODO: 
wath video on partials - https://www.youtube.com/watch?v=9Ld-aOKsEDk

# Scss - Sassy CSS
* superset of css - All css is valid scss




# Variables
`$primary-color: #3498db;` 



### Scopes
* CSS: CSS variables (introduced with Custom Properties) have a global scope,
  which means they can be accessed and modified anywhere in the stylesheet.
* SCSS: SCSS variables have a more traditional scoping mechanism. They are
  scoped to the block in which they are defined, and child blocks inherit the
  variables from their parent.

### More features
* Variables - Static during compilation, but SCSS allows you to use variables
  within other variables or create more dynamic styles using control directives
  and functions.


# Nesting
* Increse readability and avoid repetition of selectors


Plane css: 
```css
nav {
  height: 10vh;
  width: 100%;
  display: flex;
}

nav ul {
  list-style: none;
  display: flex;
}

nav li {
  margin-right: 2.5rem;
}

nav li a {
  text-decoration: none;
  color: #707070;
}

nav li a:hover {
  color: #069c54;
}
```

Scss - Avoid duplication: 
```scss
nav {
  height: 10vh;
  width: 100%;
  display: flex;

  ul {
    list-style: none;
    display: flex;
  }

  li {
    margin-right: 2.5rem;

    a {
      text-decoration: none;
      color: #707070;

      &:hover {
        color: #069c54;
      }
    }
  }
}
```


# Features


## Partials
Use to organize your code into multiple files.

* To declare a partial, we will start the file name with an underscore `_` , and add
it in another Sass file using the @import directive.

### Example

Define files: `_globals.scss` , `_variables.scss` , and `_buttons.scss` 
* Import in main.scss: 
```scss
@import "globals";
@import "variables";
@import "buttons";

```
Notice: underscore and the .scss are not added. That is because Sass
automatically assumes that you are referring to the .sass or .scss file.

## Mixins
```css
@mixin flex-container {
  display: flex;
  justify-content: space-around;
  align-items: center;
  flex-direction: column;
  background: #ccc;
}

.card {
  @include flex-container;
}

.aside {
  @include flex-container;
}
```


## & - Parent selector
* & referes to the parent selector



## Loops

## Conditionals

## Math 

## Functions


# Sass vs css

# Sass
* better organization
* can use loops
* support math without using calc
* Easy to learn: If you are familiar with CSS already, then you'll be glad to know that Sass actually has a similar syntax, and so you can start using it, even after this tutorial ;)
* Compatibility: It is compatible with all versions of CSS. So, you can use any available CSS libraries.
* Saves time: It helps reduce the repetition of CSS, because of its powerful features.
* Reusable code: Sass allows for variables and chunks of code (mixins) that can be reused over and over again. This helps you save time and makes you able to code faster.
* Organized Code: Sass helps keep your code organized by using partials.
* Cross Browser Compatibility: Sass gets compiled into CSS and adds all the necessary vendor prefixes so you don't have to worry about manually writing them out.

# Css
* css nesting is possible - but not supported by all browsers
