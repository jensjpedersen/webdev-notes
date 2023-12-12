

# Fetch 
* built in fuction to make api requests
* The fetch() method starts the process of fetching a resource from a server.


**Returns:**
* promise


* Resolve - If the Promise returned is resolve, the function within the `then()` 
  method is executed. 

```javascript
fetch(url)
  .then((response) => {
    return response.json();
  })
  .then((data) => {
    // Do something with the data
    });
  })
```

## Post
* 1st argument is the url
* 2nd argument is an options object with the method, body, and headers


```javascript
fetch(url, {
  method: 'POST',
  body: JSON.stringify(data),
  headers: {
    'Content-Type': 'application/json'
  }
})

```


## .then()
That function contains the code for handling the data received from
the API.


## Manipulate data
```javascript
.then(res => res.json())
.then(data => {
  // Do something with the data
})
```


# Promise
* The Promise object represents the eventual completion (or failure) of an
  asynchronous operation and its resulting value.




