

# React Components
* Should be written in PascalCase - **upper case** first letter.   
* Component and file name should be the same
* jsx is used to write html in js 
* jsx expression must have one parent element - usually [fragment_tag](fragment_tag.md) or div 


**Component**
* resable code that returns a react element
* two types: class and function components







# Simple React Function Component

* Function component: 
    * function 
    * returns react element
    * props as parameter

```js
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}
```


# Use component
* Use component as html tag


# Props
Props are like function arguments, and you send them into the component as attributes.
```javascript
function Car(props) {
  return <h2>I am a {props.color} Car!</h2>;
}

const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(<Car color="red"/>);
```


