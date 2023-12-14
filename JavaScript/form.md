

# Forms - Client side javascript
## Example
* How to handle forms in client side javascript instead of backend? 


**Create a form:**
* A button defaults to submit, when inside a form.
```html
<form id="myForm">
<input type="text" id="myText">
<button type="button" id="myBtn">Click</button>
</form>
```


**Add event listener:**
```javascript
const myForm = document.getElementById('myForm');
myForm.addEventListener('submit', (e) => {
    e.preventDefault();
    console.log(myText.value);
});
```

* `e.preventDefault()`  - need to prevent default behaviour of submit button
    which is to submit the form to the backend.
* **submit only works on forms**
* Button in form is a submit button by default. 
