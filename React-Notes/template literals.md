# Template literals 
----
--> we have learned template literals in javascript in which we write our code between 2 backticks (\`) and whenever we need to display any variable then we write like ${variable} 

--> we can use this same method in react also 

```js
const fname = "shivam";
const lname = "boi";
reactDOM.render(
	<>
		<h1>my name is {`${fname} ${lname}`}</h1>
		<h1>{`my name is ${fname} ${lname}`}</h1>
	</>,
	document.getElementById('root')
);
```

--> we can write both way 

