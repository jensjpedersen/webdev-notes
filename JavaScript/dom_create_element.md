
# Create html element

## Alternative 1:
**Preferred**
1. Create element with tag name: 
```javascript
const element = document.createElement("tagname"); 
```

2. Create text content: 
```javascript
element.textContent = "Hello World";
```

3. Append text to element. 
```javascript
element.append(element); 
```

## Alternative 2: 

1. Create element with tag name: 
```javascript
const tag = document.createElement("tagname"); 
```

2. Create text content: 
```javascript
const textNode = document.createTextNode("Hello World"); 
```

3. Append text to element. 
```javascript
tag.append(textNode); 
```


# Adding elemnts to html

## AppendChild vs Append
[append VS appendChild - DEV Community](https://dev.to/ibn_abubakre/append-vs-appendchild-a4m)

**Append**
* Append is newer and can take multiple arguments.
```javascript
document.body.append(tag, tag2, tag3); 
```

**AppendChild**
* AppendChild is older and only takes one argument.
```javascript
document.body.appendChild(tag); 
```











