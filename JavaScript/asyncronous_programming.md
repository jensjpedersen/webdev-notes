

# Asyncrhonous Programming

* Allows a task to be executed in the background without blocking the main thread
* Other tasks can be executed while waiting for the background task to finish


HTTP requests are asynchronous: 
* HTTP requests require a network connection and can take a long time to complete.
* If the main thread is blocked while waiting for the request to finish, the app will become unresponsive.
