# Fetch API
----

--> we can use syntax of fetch api instead of making xhr request and fetch api is latest concept to make requests 

--> syntax is :

```js
function getData(){
	fetch(url).then((response)=>{
		return response.txt();//if your data is json then use response.json()
	}).then((data)=>{
		console.log(data);
	})
}
```

--> you can use arrow functions also 

------

### Example 1 (GET request on github)

```js
function getData(){

 let url = "https://api.github.com/users"
 fetch(url).then(response=>response.json())
 .then(data=>console.log(data))
})
```

--> response :

![[Pasted image 20210716172903.png]]

----
### Example 2 (POST request on dummyAPI)

--> code :

```js
function postData(){
 let url = "http://dummy.restapiexample.com/api/v1/create";
 let data = {"name":"sfataetf","salary":"123","age":"23"};
 let params = {
 	method: 'POST',
 	Headers: {
 		'Content-Type':'application/json'
 	},
	body: data
 }
fetch(url,params).then(response=>response.json())
.then(data=>console.log(data))
}
postData();
```

-->response :

![[Pasted image 20210716174143.png]]

----

