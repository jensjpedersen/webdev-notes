
# Modules 
[JavaScript Modules](https://www.w3schools.com/js/js_modules.asp)
* JavaScript modules allow you to break up your code into separate files.

# Importing modules 

1. add type="module" to the script tag
* set type to module in the script tag
```html
<script src="js/script.js type="module></script>
```
* Modules is automatically deferred


1. Import the module 
```javascript
import { myData } from "./data.js"
```

# Exporting 
* Need the export keyword to be able to import a module. 

./data.js
```javascript
export const myData = "my data"
```

* Can not edit imported data - it is read only, even if defined with `let` or `var`
* Need to create a `editDataFunction` in the file that exports the data, to be able to edit the data.
* Where to place export statement - Personal preferance; top of file. 


## Export example 

```javascript
// export features declared elsewhere
export { myFunction2, myVariable2 };

// export individual features (can export var, let,
// const, function, class)
export let myVariable = Math.sqrt(2);
export function myFunction() {
  // …
}
```

* After the export keyword, you can use let, const, and var declarations, as well
as function or class declarations.
* You can also use the export { name1, name2 } syntax to export a list of names
  declared elsewhere. Note that export {} does not export an empty object —
  it's a no-op declaration that exports nothing (an empty name list).


## Export before declaration
* You can declare that the module exports X before the name X itself is
  declared.

```javascript
export { x };
const x = 1;
// This works, because `export` is only a declaration, but doesn't
// utilize the value of `x`.
```

# Default export VS named export
Every module can have two different types of export, named export and default
export. You can have multiple named exports per module but only one default
export. Each type corresponds to one of the above syntax.

## Named export 
* is imported with the same name as the corresponding variable.
* Can import multiple named exports in one import statement. 

```javascript
import { myFunction, myVariable } from "./data.js"
```

## Default export
* is imported with any name you want.
* Can only import one default export in one import statement. 
* If not using {}, it is a default export.

```javascript
import myFunction from "./data.js"
```


## Combine named and default export
```javascript
import myFunction, { myVariable, myVariable2 } from "./data.js"
```


# Import all exports from a file
```javascript
import * as data from "./data.js"
```
* Create a object with all exported data from data.js
* Access data with `data.myData`
