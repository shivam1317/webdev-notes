--> in Synchonous programming, all the request will perform simultaneously that's why it takes time.

==> for Example if you want these 3 requests

```c
www.codewithharry.com -> takes 10sec
www.contact.html -> takes 12sec
www.aboutus.html -> takes 5sec
```

--> so it will first do the first request after that it will do second so it will take a lot time if the server have many request and clients have to wait for the long time which is not good .

------
--> that's why we use Asynchronous programming to do this work.

--> An asunchronous model allows multiple things to happen at the same time.

==> there is a one disadvantage of this model :

--> when you call a function that permforms some action and returns something so in this model the function will stop the asynchromous model to do things and it will execute the funtion first and when it returns the value then the other request will proceed.

-----
### Few ways to write asynchronous code in js
```js
Async/wait
Callbacks
Promises
```

-----
### Example Code for Asynchronous Programming

```js
setTimeout(() => {
 for(let i=0;i<100;i++){
 	const ele = i;
 	console.log("your number is ",ele);
 }
}, 100);
console.log("Done!");
```

--> here the for loop will execute after Printing "Done" in console. because we have set the timeout for the forloop of 100ms.
