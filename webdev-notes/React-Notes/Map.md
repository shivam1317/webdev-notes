# Maps in react js 
----

--> if you want to iterate an array or an array of objects which is coming from API then you can use maps to iterate the array. 

==> Syntax : 

```js
array.map(function(value,index,arr),thisvalue)
```

--> here 
`array` means the array which you want to traverse 
`value` means the element of an array
`index` means index of current element
`arr` means the array which you are traversing currently

--> we will se later about `thisvalue`

---
==> Example :

--> we have the array `arr = ['shivam','op',1,7]` and we have to iterate it using map 

code will be :
```js
const a = arr.map(function(value){
	return value;
});
console.log(a);
```

--> and you will get all elements from an array.

----
--> if you want to iterate an array of objects then you can do same using map

==> Example : 
```js
const arr = [
 {id:1,fname:"shivam",age:19},
 {id:2,fname:"krunal",age:21},
 {id:3,fname:"furqan",age:20},
 {id:4,fname:"parth",age:18}
];

let it2 = arr2.map((value)=>{
 return `My name is ${value.fname} and my age is ${value.age}`;
});

console.log(it2);
```

--> and you will see all the objects in output 

----

NOTE : if you are getting an `warning` like this  : 

![[Pasted image 20210823133853.png]]

then you need to make one attribute called `key` in your component 

--> Example : 

![[Pasted image 20210823133951.png]]

---
