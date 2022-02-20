# Hooks 
---
--> Hooks in react js introduced in the `16.8` version of react and it's very useful in functional components 

==> for example if we want to make a button which will increase the value of count when we click that button 

so for that i have written this code : 
```js
import React from 'react'
import './click.css'

let count = 1;
function inc(){
 count++;
 console.log("Clicked");
}

const Click = ()=>{
 return(
 <>
 <h1>{count}</h1>
 <button onClick={inc}>Click me</button>
 </>
 )
}
export default Click;
```

--> but it's not increasing the value of the count in DOM 

![[Pasted image 20210825132228.png]]

----

--> so we will use hooks here. to use that we need to write like this :
```js
const state = useState();
```

--> but i got this error 

![[Pasted image 20210825134616.png]]

--> which means we can't define hooks outside the component function so we have to define hooks in the component function at the top 

and error gone !

--> and we can see `useState()` returns 2 values : first one is undefined and second is a function.

![[Pasted image 20210825140806.png]]

---
## Syntax for useState()
--> the syntax for useState function is 
```js
useState(initial, changed function);
```

--> for example : 
we want to change the count when someone click on the button so we will initialise the count with `1` and in `onClick` function we will set the `second parameter` 

```js
const [count,secondCount] = useState(1);
```

--> in onclick function we will call the secondCount function 

```js
secondCount(100);
```

--> so it will change the value of count to 100 

----

--> so to create the button which will increase the value of counter after every click i made this :

```js
import React, { useState } from 'react'
import './click.css'

const Click = ()=>{
 let [count,secondCount] = useState(1);
 function inc(){
 secondCount(count+1);
 }
 return(
 <>
 <h1>{count}</h1>
 <button onClick={inc}>Click me</button>
 </>
 )
}
export default Click;
```

