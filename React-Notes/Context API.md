## What is context API ? 
----

--> in older react if we want to pass some data to the parent component then we used props but imaging if there are many components then it becomes hard that's why we use context API to directoly pass the data to the correct component 

==> in Context api we need 3 things :

1. useContext()
2. provider
3. consumer 

---

--> For example we have the file called `Context.jsx`

![[Pasted image 20210915160621.png]]

--> and we also have a file called `A.jsx`

![[Pasted image 20210915160644.png]]

--> we are accessing the data of `A` in `Context` 

--> Now let's make one more component and name it `B`

--> B contains this code :

![[Pasted image 20210915161459.png]]

Here `A` is importing `B` and then `Comp` is importing `A` and its making a hierarchey 

-----

### But if we want the data directly from B ?

--> then we can make `Context` a provider and we will make `B` to consumer 

for that we need to write this into `Context` file 

![[Pasted image 20210915172550.png]]

--> and we will make `B` consumer 

==Note== : consumer always requires a function inside it !

![[Pasted image 20210915172618.png]]

----

### but what if we have multiple data ? 

--> if you want to export more than one variable then do like this : 

![[Pasted image 20210915173650.png]]

--> in `Consumer` file write this : 

![[Pasted image 20210915173606.png]]

This triangle is known as `callback Hell!`

--> But this consumer code is very long so we can make this code better with `useContext()`

![[Pasted image 20210915175657.png]]

-----
