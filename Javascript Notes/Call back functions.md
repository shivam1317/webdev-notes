## Definition
--> call back functions are nothing but the functions which can be given as argument .

for example if we want a function to run a another function inside it then we call it a call back function.

-----
## Example 
```js
function addstudent(student,callbackFun){

 setTimeout(() => {
	 students.push(student);
	 console.log("Student added!");
	 callbackFun();
 }, 5000);
}

let str = "";
let slist = document.getElementById('slist');

function getStudents(){
 setTimeout(() => {
	 console.log("Student data fetched!");
	 students.forEach(function (element){
	 str+=`<li>Name: ${element.name} and Marks: ${element.marks}<li>`
 })
 slist.innerHTML = str;
 }, 1000);
}

let a = {name:"test",marks:25}
addstudent(a,getStudents);
```

--> in the above code , addStudent() will call the getStudents() function so first the addStudent function will run after 5s because we have set timout of 5s and after that getStudents function will run after 1s 

-->and this is called call back functions.