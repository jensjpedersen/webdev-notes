



# arr.sort() 
* sorts by alphabetical order by default
* To sort the elements in an array without mutating the original array, use toSorted().


**Parameters**
* compareFunction (optional) - defines the sort order 

| compareFn(a, b) return value | sort order                     |
|------------------------------|--------------------------------|
| > 0                          | sort a after b, e.g. [b, a]    |
| < 0                          | sort a before b, e.g. [a, b]   |
| === 0                        | keep original order of a and b |



## Example sort in ascending order
```javascript
arr.sort((a, b) => a <= b ? -1 : 1);
```

* or better: 

```javascript
arr.sort((a,b) => a - b  );
```
* if  a > b, then change the order => return `postive number` 
* if a < b, then correct order => return `negative number`


## Sorting alphabetically
**Methods:** 
```javascript
console.log(arr.sort());
console.log(arr.sort((a,b) => a <= b ? -1 : 1));
console.log(arr.sort((a, b) => d3.ascending(a, b)));
console.log(arr.sort((a, b) => a.localeCompare(b)));
```

* Obs: Possible to compare alphabetical order by <, >, <=, >=


## Example - sort array with objects
```javascript

const arr = [
    { kommune: "Sande", kommunenummerVerdi: "1514" },
    { kommune: "Sandnes", kommunenummerVerdi: "1108" },
    { kommune: "Sauda", kommunenummerVerdi: "1135" },
    { kommune: "Sokndal", kommunenummerVerdi: "1111" },
    { kommune: "Sola", kommunenummerVerdi: "1124" },
    { kommune: "Stavanger", kommunenummerVerdi: "1103" },
    { kommune: "Strand", kommunenummerVerdi: "1130" },
    { kommune: "Stranda", kommunenummerVerdi: "1525" },
    { kommune: "Suldal", kommunenummerVerdi: "1134" },
    { kommune: "Sykkylven", kommunenummerVerdi: "1528" }
]
arr.sort((a, b) => a.kommune.localeCompare(b.kommune));
console.log(arr);

```


**LocaleCompare**
* sorts by aplhabetical order by default
* The localeCompare() method returns sort order -1, 1, or 0 (for before, after, or equal).

