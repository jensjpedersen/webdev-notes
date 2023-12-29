

# Date ouput
*Output in milliseconds*

convert to days: 
* 1000*60*60*24
* 86400000


# Get current date
```javascript
const date = new Date().toLocaleDateString();
```



# Calculate the interval between two dates
```javascript
const dayDiff = (d1, d2) => Math.ceil(Math.abs(d1.getTime() - d2.getTime()) / 86400000)

dayDiff(new Date("2023-06-23"), new Date("1997-05-31")) // 9519
```
