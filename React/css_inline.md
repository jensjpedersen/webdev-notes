

# Inlice css
* Inline css - not recommended 

```
// JSX
<div style={{ color:'red'}}>
   Red Text
</div>
 
//DOM 
<div style="color:red;">
   Red Text
</div>
```


## Not valid
```javascript
<div style={color: 'red'}>
```

Need inner curly braces: 
* style should be an javascript object 

 
