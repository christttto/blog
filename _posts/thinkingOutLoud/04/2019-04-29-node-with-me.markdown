---
layout: post
---
  

Why use node?  
Highly scalabe because event driven, non-blocking i/o model  
Same language on the front and back end(JS)  
  

Works on a single thread using non-blocking i/o calls  
	php would be synchronous where a thread will have to wait till request finishes.  
	Can max out on the machine memory.  
The single thread can handle more.  
Would not want to use with cpu heavy calculation.  
  

Fires an event, let it add to eventloop and moves on.  
  
Rest API & Microservices  
Real Time Services (Chat, Live Updates)  
CRUD Apps - Blogs, shopping carts, social networks  
	Short updates, displays, fetches from db  
Tools & utilities  
  
NPM - Node package managers  
  

The reason why in node, we do require and not import like how we do in react, is because it is not yet implemented.  
For this, babel, compiler for es6 is required.  
  

This is called common js, where we import a file using require.  
The import way is ES6 way.  
  

Path module.  
Used to work with fire directories.  
Path.join is useful because regardless of being mac or windows, uses back or foward slash accordingly.  
  

So fs writeFile overwrites  
  
  
So on os if you do platform(), you will get darwin for os.  
  
  
  
added Nodemon to the json package to package script with dev, to let me restart server everytime change has been made  
  


