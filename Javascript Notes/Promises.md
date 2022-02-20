--> in javascript , promises can have 2 conditions : resolve and reject so we use this 2 methods to check if the promise is fullfilled or not 

--> there is a promise function in javascript which have syntax like this :

```js
promise(function(resolve,reject){
})
```

--> also we have to add 2 functions resolve and reject in this syntax 

-----
## Example code 
```js
function func(){
 return new Promise(function(resolve,reject){
 const error = true;
 if(!error){
	 console.log("Function: your promise has been resolved!");
	 resolve("solved");
 }
 else{	
	console.log("Function: your promise has not been resolved!");
	reject("can's solve the issue");
 	}
 })

}
```

--> in above code if error is true then the else condition will execute and reject function will be called 

--> also when we call a func() then we have to specify 2 conditions then and catch

```js
func().then(function(message){//this function is taking a string as a parameter
	console.log(message);
}).catch(function(message){
	console.log(message);
})
```

--> so if the promise fail then reject function will be called and if promise resolved successfully then resolve function will be called 

-------
--> you can replace a call back function with promises because instead of writing call for callback function , write resolve function there and if there is a any error then write reject function for it !

