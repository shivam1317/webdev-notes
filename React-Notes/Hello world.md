# Hello world in react
-----

--> react is a javascript library which is used for making frontend of web applications 

--> react distributes the DOM (document object model) into smaller components

--> to create react app do : 

```c
npx create-react-app <appname>
```

--> after successful creation go to the app folder and run : 
```c
npm start
```

--> it will start the react web server on port 3000 

------

## Hello world code in react 

```js
var react = require('react');
var reactDOM = require('react-dom');

reactDOM.render(
 <h1>Hello world!</h1>,
 document.getElementById('root')
);
```
--> here the h1 tags is not known as html but it's JSX 

--> here we need to import 2 things react and react-dom.

--> render() function renderes the html code into the DOM 

==> syntax for render() is 
```js
render(what to show,where to show, callback func);
```

--> callback function is optional 

-------

--> react by default installs the babel and webpack 

--> babel is a compiler for modern js which converts the modern js code into the browser understandable code 

--> so you can write import statements like this 

```js
import react from 'react';
import reactDOM from 'react-dom';
```

------
