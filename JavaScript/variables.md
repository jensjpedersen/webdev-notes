

# Varibles


## Declare empty variable 

`let var1` 
* automatically assigned value undefined



## Variables
* Mutable variable
`let var` 

* Konstant variabel 
`const var` 

Hvis du prøver å redefinerer `const` -> gir TypeError

**Ikke bruk var**
* ble brukt i gammel javascript, pre 2015

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

