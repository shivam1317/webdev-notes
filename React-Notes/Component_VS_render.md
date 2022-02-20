--> we know that with component method we can directly pass the component which we want to get displayed at perticular path using `Route` and `Switch`

### But what if we want to pass the props in our components ?

i have written this in `Main.jsx` file

![[Pasted image 20210922151154.png]]

--> because we can't directly pass the props in `component` method so we have to make a callback function

and then write like this in all components 

```js
import React from "react";

function Home(props) {
 return (
 <div>
 <h1>This is a {props.name} page</h1>
 </div>
 );
}
export default Home;
```

-----
--> if we write `render` in the place of component then we will get the same results 

![[Pasted image 20210922152456.png]]

-----

## So what is the difference between component and render method ?

==> whenever we call the component then it will create a new element everytime and then display us . For example using `CreateElement`

==> whenever we call render method then it will display only changes and if there are not any changes then it will display the same element 

-----

## when to use component and render?

--> if you don't have any props in your components then use `component` method and if you have to pass any props in component then use `render` method 

==> There is a no difference between component and render in performance.	