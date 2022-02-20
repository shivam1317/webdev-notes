### Difference between res.render() and res.json()

--> `res.render()` will always render the whole `html,css and js` from the server whenever someone requests the server or any data being changed. This is called server side rendering. Example : wikipedia

--> `res.json()` will render the `html,css and js` first time and then it will only respond the `json` data and DOM will be changed accordingly to the json data and this method is very useful in `API`. Example : facebook

==> `res.json()` is faster than `res.render()` because it stores some data on browser and changes it accordingly to the json response.



