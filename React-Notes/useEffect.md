--> useEffect is a one type of hook which will be triggered after render 

==> For example : 

This code will change the count once user clicks on button then counter will increase 

![[Pasted image 20210917130057.png]]

-----
#### But what if we want an alert everytime when user clicks on button and count also must be changed ?

then we will use `useEffect()` hook which will trigger after render that means every time it will trigger after render function called

if we add more than one button in our DOM then whenever we click on any button then we will get alert regardless the states for buttons are same or not 

-----

#### But what if we want alert only once when someone refreshes the page?

then we just need to modify the `useEffect` code a little bit 

```js
useEffect(() => {

 alert("Why are you clicking me mf?");

 }, []);
 ```
 
 just add `[]` at the end of `useEffect()` and it will be called only after refresh !
 
 ----
 
 #### But what if we want to trigger useEffect only when someone click on perticular button only?
 
 then just make some changes in above code :
 
 ```js
useEffect(() => {

 alert("Why are you clicking me mf?");

 }, [<hookname>]);
 ```
 
 for example : 
 
 ![[Pasted image 20210917132535.png]]