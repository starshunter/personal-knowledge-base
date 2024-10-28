title:: JavaScript Questions/2022-08

- [[2022-08-01 Monday]] #Promise
  collapsed:: true
	- ```javascript
	  const promise1 = Promise.resolve('First')
	  const promise2 = Promise.resolve('Second')
	  const promise3 = Promise.reject('Third')
	  const promise4 = Promise.resolve('Fourth')
	  
	  const runPromises = async () => {
	  	const res1 = await Promise.all([promise1, promise2])
	  	const res2  = await Promise.all([promise3, promise4])
	  	return [res1, res2]
	  }
	  
	  runPromises()
	  	.then(res => console.log(res))
	  	.catch(err => console.log(err))
	  ```
	- this program will print `Third`
	- `Promise.all()` will reject if one of the promises fails, and the value will be the failed promise's value
	- the `catch()` method will catch the rejected value
- [[2022-08-02 Tuesday]] #Object
  collapsed:: true
	- ```javascript
	  const keys = ["name", "age"]
	  const values = ["Lydia", 22]
	  
	  const method = /* ?? */
	  Object[method](keys.map((_, i) => {
	  	return [keys[i], values[i]]
	  })) // { name: "Lydia", age: 22 }
	  ```
	- `method` should be `fromEntries`
	- `fromEntries()` turns a two dimensional array into an object
		- the first element of a subarray will be the key, and the second element will be the value
	- reference
		- [Object.fromEntries()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/fromEntries)
		  type:: document
		  tags:: JavaScript, Object, Array
		  title:: Object.fromEntries()
- [[2022-08-03 Wednesday]] #Object
  collapsed:: true
	- ```javascript
	  const createMember = ({ email, address = {}}) => {
	  	const validEmail = /.+\@.+\..+/.test(email)
	  	if (!validEmail) throw new Error("Valid email pls")
	  
	  	return {
	  		email,
	  		address: address ? address : null
	  	}
	  }
	  
	  const member = createMember({ email: "my@email.com" })
	  console.log(member)
	  ```
	- this program will print `{email: "my@email.com", address: {}}`
	- the default value of `address` is `{}`
	- an empty object is a truthy value
- [[2022-08-04 Thursday]]
  collapsed:: true
	- ```javascript
	  let randomValue = { name: "Lydia" }
	  randomValue = 23
	  
	  if (!typeof randomValue === "string") {
	  	console.log("It's not a string!")
	  } else {
	  	console.log("Yay it's a string!")
	  }
	  ```
	- this program will print `Yay it's a string!`
	- `typeof randomValue` returns `"number"`
	- `!typeof randomValue` returns `false`