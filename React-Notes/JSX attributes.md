--> jsx attributes are the parameters/attributes which we give in html elements 

For example : 
```html
<img src="#">
```

--> here src is an attribute 

==> Example 2 : 
```js
<h1 contentEditable="true">This is heading</h1>
```

--> and we can edit the heading text with the help of this attribute 

-----
--> in react the tags which don't have any children (i.e tags which don't have closing tag ) are written as follows : 

```js
<img /> // This called self closing tag
```

--> Code : 

```js
reactDOM.render(
 <>
 	<h1 contentEditable="true">This is an image</h1>
 	<img src="https://picsum.photos/200/300" alt="Image not found"/>
 </>,
 document.getElementById('root')
);
```