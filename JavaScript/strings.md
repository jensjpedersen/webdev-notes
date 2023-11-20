


# Basics
* You can use single or double quotes
* You can use quotes inside a string, as long as they don't match the quotes surrounding the string:

# Common string methods


* `string.toUpperCase()` 

* `string.toLowerCase()` 

* `string[index]` 


* get from index 4 to 10-1
`string.substring(4, 10)` 


* replace first instance of a string with another string 
`string.replace("replace this", "with this")` 


* Strip whitespace from beginning and end of a string
`string.trim()` 


* Split and create an array from a string
`string.split("") // split on every character` 

## Slice 
* `array.slice(start, end)` 

**Parameters:**
* start	 - Optional. Start position. Default is 0.
    Negative numbers select from the end of the array.
* end -	Optional. End position. Default is last element.
    Negative numbers select from the end of the array.


# Escape characters
`let text = "We are the so-called \"Vikings\" from the north.";` 

# Attributes

* length 


# Breaking string

Works: 
```javascript
document.getElementById("demo").innerHTML = "Hello \
Dolly!";
```

better (safer): 
```javascript
document.getElementById("demo").innerHTML = "Hello " +
"Dolly!";
```



# String concatenation
* `string1 + string2 + not_string` 
`not_string` will be converted to string


**Template string**
* use backticks
```javascript
console.log(`nummeret er: ${total}` )
```








