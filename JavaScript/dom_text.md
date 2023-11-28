
# Inspect tool 
* go to properties to show all dom properties of an element

# Text Content vs Inner Text vs Inner HTML
* textContents is all text contained by an element and all its children that are for formatting purposes only.
* innerText returns all text contained by an element and all its child elements.
* innerHtml returns all text, including html tags, that is contained by an element.




# Example 

* Consider this html code: 
```html
<div id="mylinks">
  This is my <b>link collection</b>:
  <ul>
    <li><a href="www.borland.com">Bye bye <b>Borland</b> </a></li>
    <li><a href="www.microfocus.com">Welcome to <b>Micro Focus</b></a></li>
  </ul>
</div>
```

## element.textContent 
result: 
```
This is my link collection:
```


## element.innerText
result:
```
This is my link collection:Bye bye Borland Welcome to Micro Focus
```


## element.innerHtml
result: 
```
This is my <b>link collection</b>:
<ul> 
  <li><a href="www.borland.com">Bye bye <b>Borland</b></a></li>
  <li><a href="www.microfocus.com">Welcome to <b>Micro Focus</b></a></li> 
</ul>
```

