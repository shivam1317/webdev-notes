--> to print date and time into js we have 2 functions 

```js
let Currdate = new Date().toLocaleDateString();
let Currtime = new Date().toLocaleTimeString();
```

--> challenge 2 solution

```js
// challenge 2

let fname = "shivam";
let currDate = new Date().toLocaleDateString();
let currTime = new Date().toLocaleTimeString();

reactDOM.render(
 <>
 	<p>{`My name is ${fname}`}</p>
 	<p>{`Today's date is ${currDate}`}</p>
 	<p>{`Time is ${currTime}`}</p>
 </>,
 document.getElementById('test')
);
```	

