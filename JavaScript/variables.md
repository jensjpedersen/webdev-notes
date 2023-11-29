

# Varibles


## Declare empty variable 

`let var1` 
* automatically assigned value undefined



## Variables
* Mutable variable
`let variabel` 

* Konstant variabel 
`const variabel` 

**Let and const are block scoped**

Hvis du prøver å redefinerer `const` -> gir TypeError

**Ikke bruk var**
* ble brukt i gammel javascript, pre 2015
* var is closure scoped, e.g. function scoped. 


## Symantic
Use camelCase for variable names
* variables: `detteErEtLangtVariabelNavn` 

* Kan bruke understrek hvis ønskelig. 



# Static variable
* Create a static variable in a function
* `foo.counter` is only initialized once 

```javascript
function foo() {
    if( typeof foo.counter == 'undefined' ) {
        foo.counter = 0;
    }
    foo.counter++;
    console.log(foo.counter);
}
```

