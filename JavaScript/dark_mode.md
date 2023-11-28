
# Dark mode logic

```html
<button id="dark-mode" onclick="darkModeToggle()"></button>
```

```css
.dark-mode {
  background-color: black;
  color: white;
}
```

```javascript
function darkModeToggle() {
  let body = document.body;
  body.classList.toggle("dark-mode");
}
```


