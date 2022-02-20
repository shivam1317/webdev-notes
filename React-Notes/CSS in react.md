--> to add the css into our index.js file we have one css file called index.css so first we have to add that file into index.js

```js
import './index.css'
```

--> you just need to do same as we do in simple html and css . just add 
`className` attribute and add css into it in `index.css` file 

==> Code : 

```js
reactDOM.render(

 <>
 <h1 className="heading">This is an image</h1>
 <div className="img_div">
 	<img src="https://picsum.photos/200/300" alt="Image not found"/>
 	<img src="https://picsum.photos/210/300" alt="Image not found"/>
 	<img src="https://picsum.photos/220/300" alt="Image not found"/>
 </div>
 </>,
 document.getElementById('root')
);
```

--> this is the output :

![[Pasted image 20210813141937.png]]

------
## Inline CSS

--> to add inline css we have to make an object of css properties in `index.js` file and then we can pass that object in `style` attribute 

==> example : 

```js
const head = {
	color : 'red'
}

reactDOM.render(
	<h1 style = {head}> This is heading </h1>,
	document.getElementById('root')
)
```

--> you **can't** add inline css like `<h1 style="color:blue;">test</h1>`

