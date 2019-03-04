---
layout: post
---
  

notes for common JS problems.

  

# What is prototypical inheritance?
	(prototype base inheritance)  
	Every object has a property called prototype.  
	can add methods and properties to it.  

	if to an object, prototype can be added, than it can be used in others.  

# Function Delaration vs. Function Expression  
  
	Declaration: where I am making a function in normal way  
	Expression: let a variable save anon function  

	if function executed before than declaration, it will be available.  
	But for expression, it will not be available like how let would be.  
  
  	function expression can pass the function expression to another variable. 
  
# What is promise, why do we use it?  
  
  When you wanna make async call, which has to wait for something to happen and than once it comes back you exit with a callback funciton.  
  Within that callback's function, you might do another ajax call which can wait for another result (waiting on waiting on waiting).  
  it gets ugly, hard to debug, so we use promise calls.  
  It can become a variable, to make it read better.  

# setTimeout() quiz  
	===code===  
	setTimeout(function(){  
		console.log('a')  
	}, 0)  
	console.log('b')  
	console.log('c')  
	===code===  
  
	the result will be in order of b,c,a.  
	when it becomes asynchronous, it has to wait for all the stack to finish.  
	Than, all the asynchronous will start.  

# What is closure  
  
	When function returns another function, it will hold its environment with it.  

	===code===
	let obj = function(){
		let i = 0
		return {
			setI(k){
				i = k
			},
			getI(){
				return i
			}
		}
	}

	let x = obj()
	x.setI(2)
	console.log(x.getI()) //returns 2














