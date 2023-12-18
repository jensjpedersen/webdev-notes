
# Response
* The Response interface of the Fetch API represents the response to a request.
* You can create a new Response object using the Response() constructor
* documentation: [Response - Web APIs | MDN](https://developer.mozilla.org/en-US/docs/Web/API/Response)



## Response: json() method
It returns a promise which resolves with the result of
parsing the body text as JSON.

Note that despite the method being named json(), the result is not JSON but is
instead the result of taking JSON as input and parsing it to produce a
JavaScript object.

**Returns**
A Promise that resolves to a JavaScript object. This object could be anything
that can be represented by JSON — an object, an array, a string, a number…

