
# DOM events
[HTML DOM Event Object](https://www.w3schools.com/jsref/dom_obj_event.asp)



# Events Listener

* Best practice - Define in js file, not in html file.


## Events
* click - works only on desktop XXX: ???
* pointer, butvent (same as click), but works on mobile and desktop
* pointerdown 
* pointerup 

## .onclick VS .addEventListener

### .oneclick
* kan bruke onclick attribute
* bruker referanse til funksjonen


```javascript
element.onclick = handleClick


function handleClick() {
    console.log("clicked")
}
```

### .addEventListener
* bruker callback funksjon

```javascript
element.addEventListener("click", handleClick)
```


### onclick HTML
* do not use onclick in html



# Keyboard events - Best practice 
**Key events**: 
* Bruk code eller key 
* ikke bruk charCode, which, keyCode

## Code
* code is dependent on Number Lock, Caps Lock, and Shift key

## Key
* key is constant. 


