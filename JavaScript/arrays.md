

# Empty array 

* Index starts at 0

let array = []

let array = ["banan", "eple", "pære"]




# Array methods
* Get index of the item in the array - Returns `-1` if not found. 
`array.indexOf('item') ` 

* Join array elements in a string separated by space
`arr.join(" ")` 

* Check if array includes element: 
`arr.includes('element')` 

* sort array 
`arr.sort()` 

* reverse array
`arr.reverse()` 

# Array methods - Concat 
* Add array to array
`arr.concat(arr2)` 

* Can add multiple arrays: 
`arr.concat(arr2, ["eple"])` 



# Array methods - Add and remove elements
## Splice 
* At position 2, add 2 elements - Changes original array:
`fruits.splice(2, 0, "Lemon", "Kiwi");` 

* At position 2, remove 2 items - Changes original array:
`fruits.splice(2, 2);` 

## Slice 
* `array.slice(start, end)` 

**Parameters:**
* start	 - Optional. Start position. Default is 0.
    Negative numbers select from the end of the array.
* end -	Optional. End position. Default is last element.
    Negative numbers select from the end of the array.

## Other
* Add element at index - Changes origianl array: 
`arr[index] = "element"` 

* Remove last element from array - Returns last item in array - Changes original array
`arr.pop()` 

* Add element to end of array - Returns length of array - Changes original array
`arr.push("element")` 

* Add element to beginning of array - Changes orignal array
`arr.unshift("element")` 


# Array attributes
* length - number of items in array





# Splice

## Syntax
array.splice(index, howmany, item1, ....., itemX)

### Add elements

* At position 2, add 2 elements:

```javascript
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.splice(2, 0, "Lemon", "Kiwi");
```



### Remove elements

* At position 2, remove 2 items:

```javascript

const fruits = ["Banana", "Orange", "Apple", "Mango", "Kiwi"];
fruits.splice(2, 2);
```


