--> There are 4 ways to add multiple elements in render function

==> Method 1 :

--> you can add multiple elements in DOM by adding them between div tags

```js
reactDOM.render(
	<div>
		<h1>Hello world</h1>
		<p> React is op </p>
	</div>,
	document.getElementById('root')
);
```

==> Method 2 :

--> if your react version is greater than 16.0 then you can use arrays to add multiple elements in the DOM 

```js
reactDOM.render(
	[
		<h1>Hello world</h1>,
		<p> React is op </p>,
		<h3> This is heading </h3>
	],
	document.getElementById('root')
);
```

==> Method 3 : 

--> if you don't need extra div in the first method then put them between react fragment

```js
reactDOM.render(
	<React.fragment>
		<h1>Hello world</h1>
		<p> React is op </p>
	</React.fragment>,
	document.getElementById('root')
);
```

==> Method 4 : 

--> you also don't need to write `React.fragment` just put the elements between empty open and close tag 

```js
reactDOM.render(
	<>
		<h1>Hello world</h1>
		<p> React is op </p>
	</>,
	document.getElementById('root')
);
```


