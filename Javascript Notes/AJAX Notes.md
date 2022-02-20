### What is AJAX?
--> AJAX stands for Asynchronous javascript and XML.

--> AJAX is not a programming language it's a new technology.

--> Modern websites use JSON instead of XML to fetch the data 

-----
### Advantage of AJAX
--> No page reload/refresh

--> Better user experience

--> Saves netowork bandwith 

-->very interactive 

------
### How it works?

![[Pasted image 20210708160905.png]]

----
### Sample code 
--> first of all you have to create a xhr object and then open it

```js
const xhr = new XMLHttpRequest();
xhr.open('GET','test.txt',true);
```

--> the syntax for open function is
```c
open(Request type , file you want to open, is Asynchronous{true or false} )
```

-->after that if you want to track the progress of the request then use onprogress() and onload() functions 

--> and at the end send the request !
```js
xhr.send();
```
----

### xhr ready states 

![[Pasted image 20210708165217.png]]

-----
--> you als can request for sample JSON request from websites who offeres free fake JSON request 

--> one website is : https://jsonplaceholder.typicode.com/

```js
xhr.open('GET','https://jsonplaceholder.typicode.com/todos/1',true);
```

--> and you can see we got the response in console 

![[Pasted image 20210708171156.png]]

----
--> you can also create POST request from xhr

--> i found another website for this : https://dummy.restapiexample.com/

![[Pasted image 20210710135628.png]]

--> to create POST request type :
```js
xhr.open('POST','http://dummy.restapiexample.com/api/v1/create',true);
xhr.getResponseHeader('Content-type','application/json');
```

--> this request is accepting JSON that's why we have set Content-type to application/json

--> set the parameters and send the request

```js
params = `{"name":"shivam","salary":"123","age":"23"}`;
xhr.send(params);
```

