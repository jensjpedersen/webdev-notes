
# Regex
* not a string
* `/regex/` - Regex is placed between two forward slashes


# Replace with Regular Expression
```javascript
var str = "abc123def456ghi";
var result = str.replace(/\D/g, "");
console.log(result); // 123456
```

