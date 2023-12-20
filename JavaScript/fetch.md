

# Fetch 
* built in fuction to make api requests
* The fetch() method starts the process of fetching a resource from a server.


* Can not console log data outside of fetch. Need to do it inside fetch
* [ ] Else will get promise pending - console log does not know when data is
  available (syncronious code).

**Returns:**
* **A `Promise`  that resolves to `Response` object.** - 
* Or rejects with a `TypeError`

    A fetch() promise only rejects when a network error is encountered (which is
    usually when there's a permissions issue or similar). A fetch() promise does
    not reject on HTTP errors (404, etc.). Instead, a then() handler must check the
    Response.ok and/or Response.status properties.



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


## .then() and .catch()
That function contains the code for handling the data received from
the API.

* if the promise is resolved, the function within the `then()` method is executed.
* if the promise is rejected, the function within the `catch()` method is executed.



## Manipulate data
```javascript
.then(res => res.json())
.then(data => {
  // Do something with the data
})
```

* Response.json() - Returns a new Response object for returning the provided
  JSON encoded data.

# Promise
* The Promise object represents the eventual completion (or failure) of an
  asynchronous operation and its resulting value.




