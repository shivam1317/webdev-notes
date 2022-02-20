## Props 
----
--> props in react js is nothing but it's a short form of properties 

--> Using props we can make our own attributes in react js like we make our own tags 

==> for example we have this component 
```
ReactDOM.render(
 <Card image="https://mir-s3-cdn-cf.behance.net/project_modules/fs/aac57a29688377.55ffa78f025a6.jpg" sname="Mr.robot" info="Hacker's web series" plink="https://www.amazon.com/Mr-Robot-Season-1/dp/B00YBX664Q"/>,
 document.getElementById('root')
);
```

--> here image,sname,plink and info are props 

----

==> JSX file 

```js
function Card(props){
 return (

 <>
 <div className="cards">
 	<div className="card">
 		<img src={props.image} alt="NoImage" className="card_img" />
 		<div className="card_info">
 			<h3>{props.sname}</h3>
 			<span>{props.info}</span>
 			<a href={props.plink} target="_blank" rel="noreferrer">
 			<button>Watch now</button>
 			</a>
		</div>
 	</div>
 </div>

 </>
 );

}
export default Card;
```

--> here all the attributes which we defined in `index.js` file are referred as an object so we can write attributes as `object.key` in our function 

----