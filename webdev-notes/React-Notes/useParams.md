--> if you want to add the parameter in `path` attribute of `Route` component then you have to do like this :

```js
<Route path="/users/:name" component={User} />
```

here if you want to add a parameter then you have to add `:` before the parameter name 

--> in `Users.jsx` file :
```js
import React from "react";

function User({ match }) {
 return (
 <div>
 <h1>This is a Users page!</h1>
 <h3>Welcome {match.params.name}</h3>
 </div>
 );
}
export default User;
```

------

--> using `useParams()` we can do this more easily 

you just need to make one variable using `useParams()` and then write it at the place of `match.params.name`

Example : 
```js
const {name} = useParams();
return <h1>Welcome {name}</h1>
```

-----

--> if you want to pass multiple parameters then write like this : 

```js
<Route path="/users/:fname/:lname" component={User} />
```

NOTE : parameter name and variable name must be same !

