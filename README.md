# random-knowledge


### What is CSRF Token?
Ans: CSRF Token is randomly generated token/key that is used to prevent an application/service from CSRF attacks. It needs to be unique per user session and must be of very large value such that cannot be guessed easily. A CSRF Token secured application assigns uique Token per user session.

### What are WSGI and ASGI in Django?
Ans: 
* ***WSGI:** Web Server Gateway Interface*
	- WSGI is a simple interface where we can define our application as a callble,
	- WSGI applications take only 1 request at a time and returns response for it. This single and synchronous callable limits WSGI for long lived connections like websockets,
	- Limitations: 
		1. It cannot deal with WebSockets
		2. Cannot work with HTTP/2
		3. It is not asynchronous(async/await cannot be used)
		
* ***ASGI:** Asynchronous Server Gateway Interface*
	- On the contrary of WSGI, ASGI is asynchronous,
	- Here we can define our application as a callble which is Async by default,
	- It allows multiple incoming & outgoing events for each application
	- It allows background coroutines so that the application is able to do other things such listening for events on an external trigger




### HTTP/1.1 Vs HTTP/2
Ans: 
