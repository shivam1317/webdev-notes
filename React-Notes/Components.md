-->  the components in react are very useful and best part of react .

--> components means we divide the website code into the smaller part and then we combine them to make final website.

--> NOTE : the name of the `.jsx` file must be start with capital letter 

--> For example if we want to make a heading component then we will make one file called `Heading.jsx` and add this :

```js
import React from 'react';
function Heading(){
	return <h1>This is a heading</h1>
}
export default Heading;
```

--> so i made 2 components for Heading and paragraph 

```js
import React from 'react';
function Para(){
 return <p>This is a paragraph</p>
}

export default Para;
```

-----
--> now just import the components 

![[Pasted image 20210813175809.png]]

--> and use them 

![[Pasted image 20210813175837.png]]

--> and we got the output 

![[Pasted image 20210813175944.png]]

--> as they don't have child so we can write these tags as 
```html
<Heading />
<Para />
```
--> These are known as self closing tags 

-----
--> But if there was a master component and we only import that in our main `index.js` file 

--> so we made a file called `Master.jsx` which is master component 

--> i added this into `Master.jsx`
![[Pasted image 20210813180300.png]]

--> and just import it in `index.js` file 
--> we just need to write this 

```js
reactDOM.render(
 <Master></Master>,
 document.getElementById('root')
);
```