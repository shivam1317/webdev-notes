--> import means taking anything from someone and export means giving our product to others 

--> in js/react we can import variables,functions,objects etc from other files using `import` keyword 

--> for example if we have one file called `Test.jsx` and it contains this code : 

```js
const fname = "shivam";
export default fname;
```

--> here we are exportin gthe variable `fname` so that we can use it in other files . and we are using `default` here That means we can give any name to this variable in other file

--> NOTE : we can export only 1 default variable in a file 

--> if you want to export any variable then you have to write the same name in other file 

==> for example : 
```js
const lname = "boi";
export {lname};
```

--> you have to write the variable name in `{}` 

-----
--> if you want to export any functions then you can do the same as variables . just write them in same `{}` sepereted by comma

```js
let fname = "shivam";
function getName(){
	return fname;
}
export {fname,getName};
```

--> you can import them by sepereting them by comma 
```js
import {name,getName} from './Test'
```

--> if you want to import all the exported variables at one time then you can use  wildcard `*` which will store the variables and functions in the form of object

==> for example : 

--> Test.jsx file:
```js
let name = "shivam";
let lname = "op";
funtion getName(){
	return "shivam007"
}
export default name;
export {lname,getName};
```

--> index.js file :
```js
import * as test from './Test'

reactDOM.render(
	<>
		<p>{test.default}</p>
		<p>{test.lname}</p>
		<p>{test.getName()}</p>
	</>
);
```

--> name is exported as `default` so we can write it as `test.default`

--> and output will be same !

--> the wildcard method is not recommended because it exports all the variables and functions from the file so try to use previous method in which we import specific things.

----