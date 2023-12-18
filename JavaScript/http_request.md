


# HTTP requests

* In browser - go to network tab to see all requests
* staus 404 - is not an error. It is a valid response.


## Headers
* metadata about the request

## Response
* status code


## HTTP request methods
**Most common**
* GET request - get data from server
* POST request - send data to server
* PUT request - update data on server
* DELETE request - delete data on server


# Array methods
**Important**: with array methods, e.g. forEach. Data may be fetched in
different order. E.g. not sorted wit correct numbering
* this is still true if using async await.

**Use ordinary for loop if correct order is cirtcal**

# How to make a request
* use `fetch(url)` to create http request
* fetch returns a promise. Need to resolve it with `.then()`

```javascript
async function getUsers() {
    const response = await fetch('https://jsonplaceholder.typicode.com/users')
}
```



# Response
**Response object**
* type - type of request:
    basic
    cors - tpyical for fetch
    error
* url - url of request
* redirected - if request was redirected to another url
* status - status code
* ok - true if status code is 200. If false, then status code is 400 or 500
* statusText - status code text
* headers - Extra data about request
* body - ReadableStream - data from server. Need to convert it to json

## Status code


**Status codes**
* 100-199 - information responses
* 200-299 - success responses. This is what we want
* 300-399 - redirect - If page is moved to another url
* 400-499 - client error - If error on client side 
* 500-599 - server error - If error on server side


* Invalid url wil give status code 404 (page not found)


## Error handling

### OK status code
* The ok read-only property of the Response interface contains a Boolean
  stating whether the response was successful (status in the range 200-299) or
  not.

```javascript
if (response.ok) {
    // do something
}
```

### Error status code
```javascript
if (!response.ok) {
    throw new Error(response.status)
}
```

## Get data from response 

* Remember to use await to get data from response - else will return pending promise. 

```javascript
const data = await repsonse.text()
```

or

```javascript
const data = await repsonse.json()
```
