--> async and await is the very useful feature in javascript for fetch API

--> when you define a async function it will always return promise 

```js
async function Fetchdata(){
 console.log("We are in the function");
// await will tell the function to move ahead and execute the command which are after function call
 const response = await fetch('https://api.github.com/users');
 console.log("Converting the response into json");
 const users = await response.json();
 console.log("returning the promise from function");
 return users;//this is promise
}
```

--> whole code looks like this and i have writed steps in code in terms of execution order

![[Pasted image 20210720140556.png]]

--> response 

![[Pasted image 20210720140723.png]]