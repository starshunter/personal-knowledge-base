title:: JavaScript Questions/2022-07

- [[2022-07-01 Friday]] #Setter
  collapsed:: true
	- ```javascript
	  const config = {
	    languages: [],
	    set language(lang) {
	      return this.languages.push(lang);
	    },
	  };
	  
	  console.log(config.language);
	  ```
	- this program will print `undefined`
	- `language` is a setter method, it will only return `undefined`
	- reference
		- [setter](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/set)
		  type:: document
		  tags:: Setter, JavaScript
		  title:: setter
- [[2022-07-02 Saturday]]
  collapsed:: true
	- ```javascript
	  const name = 'Lydia Hallie';
	  
	  console.log(!typeof name === 'object');
	  console.log(!typeof name === 'string');
	  ```
	- this program will print `false` `false`
	- `typeof name` returns `string`, and `!typeof name` returns `false`
- [[2022-07-03 Sunday]] #[[Arrow Function]]
  collapsed:: true
	- ```javascript
	  const add = x => y => z => {
	    console.log(x, y, z);
	    return x + y + z;
	  };
	  
	  add(4)(5)(6);
	  ```
	- this program will print `4` `5` `6`
	- `add()` is an arrow function which invokes another arrow function, which invokes another arrow function
- [[2022-07-04 Monday]] #Promise #[[Generator Function]]
  collapsed:: true
	- ```javascript
	  async function* range(start, end) {
	    for (let i = start; i <= end; i++) {
	      yield Promise.resolve(i);
	    }
	  }
	  
	  (async () => {
	    const gen = range(1, 3);
	    for await (const item of gen) {
	      console.log(item);
	    }
	  })();
	  ```
	- this program will print `1` `2` `3`
	- we are awaiting on the promise `range` returns
- [[2022-07-05 Tuesday]] #Object
  collapsed:: true
	- ```javascript
	  const myFunc = ({ x, y, z }) => {
	    console.log(x, y, z);
	  };
	  
	  myFunc(1, 2, 3);
	  ```
	- this program will print `undefined` `undefined` `undefined`
	- `myFunc` expects an object with three properties, but it only gets three numbers
- [[2022-07-06 Wednesday]]
  collapsed:: true
	- ```javascript
	  function getFine(speed, amount) {
	    const formattedSpeed = new Intl.NumberFormat('en-US', {
	      style: 'unit',
	      unit: 'mile-per-hour'
	    }).format(speed);
	  
	    const formattedAmount = new Intl.NumberFormat('en-US', {
	      style: 'currency',
	      currency: 'USD'
	    }).format(amount);
	  
	    return `The driver drove ${formattedSpeed} and has to pay ${formattedAmount}`;
	  }
	  
	  console.log(getFine(130, 300))
	  ```
	- this program will print `The driver drove 130 mph and has to pay $300.00`
- [[2022-07-07 Thursday]] #[[Destructuring Assignment]] #Object
  collapsed:: true
	- ```javascript
	  const spookyItems = ['👻', '🎃', '🕸'];
	  ({ item: spookyItems[3] } = { item: '💀' });
	  
	  console.log(spookyItems);
	  ```
	- this program will print `["👻", "🎃", "🕸", "💀"]`
	- we assign the value `💀` to `spookyItems[3]` using object destructuring
- [[2022-07-08 Friday]]
  collapsed:: true
	- ```javascript
	  const name = 'Lydia Hallie';
	  const age = 21;
	  
	  console.log(Number.isNaN(name));
	  console.log(Number.isNaN(age));
	  
	  console.log(isNaN(name));
	  console.log(isNaN(age));
	  ```
	- this program will print `false` `false` `true` `false`
	- `Number.isNaN()` can check if the value passed is a numeric value and equal to `NaN`
	- `isNaN()` can check if the value passed is not a anumber
- [[2022-07-09 Saturday]] #[[Temporal Dead Zone]]
  collapsed:: true
	- ```javascript
	  const randomValue = 21;
	  
	  function getInfo() {
	    console.log(typeof randomValue);
	    const randomValue = 'Lydia Hallie';
	  }
	  
	  getInfo();
	  ```
	- this program will print `ReferenceError`
	- variables declared with `const` and `let` are not referenceable before their initialization
- [[2022-07-10 Sunday]] #Asynchronous #Promise
  collapsed:: true
	- ```javascript
	  const myPromise = Promise.resolve('Woah some cool data');
	  
	  (async () => {
	    try {
	      console.log(await myPromise);
	    } catch {
	      throw new Error(`Oops didn't work`);
	    } finally {
	      console.log('Oh finally!');
	    }
	  })();
	  ```
	- this program will print `Woah some cool data` `Oh finally!`
- [[2022-07-11 Monday]] #Array #Flat
  collapsed:: true
	- ```javascript
	  const emojis = ['🥑', ['✨', '✨', ['🍕', '🍕']]];
	  
	  console.log(emojis.flat(1));
	  ```
	- this program will print `['🥑', '✨', '✨', ['🍕', '🍕']]`
	- we can create a new flattened array using `flat()`
	- we can pass the value about the depth of the flattened array
	- reference
		- Array.prototype.flat()
		  type:: document
		  tags:: JavaScript, Array
		  title:: Array.prototype.flat()
- [[2022-07-12 Tuesday]] #Object #[[Call By Sharing]]
  collapsed:: true
	- ```javascript
	  class Counter {
	    constructor() {
	      this.count = 0;
	    }
	  
	    increment() {
	      this.count++;
	    }
	  }
	  
	  const counterOne = new Counter();
	  counterOne.increment();
	  counterOne.increment();
	  
	  const counterTwo = counterOne;
	  counterTwo.increment();
	  
	  console.log(counterOne.count);
	  ```
	- this program will print `3`
	- objects in JavaScript are call by sharing, so `counterTwo` references to `counterOne`
- [[2022-07-13 Wednesday]] #Promise #[[Call Stack]]
  collapsed:: true
	- ```javascript
	  const myPromise = Promise.resolve(Promise.resolve('Promise'));
	  
	  function funcOne() {
	    setTimeout(() => console.log('Timeout 1!'), 0);
	    myPromise.then(res => res).then(res => console.log(`${res} 1!`));
	    console.log('Last line 1!');
	  }
	  
	  async function funcTwo() {
	    const res = await myPromise;
	    console.log(`${res} 2!`)
	    setTimeout(() => console.log('Timeout 2!'), 0);
	    console.log('Last line 2!');
	  }
	  
	  funcOne();
	  funcTwo();
	  ```
	- this program will print `Last line 1! Promise 2! Last line 2! Promise 1! Timeout 1! Timeout 2!`
	- the callback function of `setTimeout()` and the promise cannot be added to the callstack if it's not empty
	- promises are micro-tasks, so they are resolved first once the callstack is empty
- [[2022-07-14 Thursday]] #Import
  collapsed:: true
	- ```javascript
	  // sum.js
	  export default function sum(x) {
	    return x + x;
	  }
	  
	  // index.js
	  import * as sum from './sum';
	  ```
	- we can invoke `sum()` in `index.js` using `sum.default(4)`
	- using `*` imports all exported values from the file
- [[2022-07-15 Friday]] #Proxy #Object
  collapsed:: true
	- ```javascript
	  const handler = {
	    set: () => console.log('Added a new property!'),
	    get: () => console.log('Accessed a property!'),
	  };
	  
	  const person = new Proxy({}, handler);
	  
	  person.name = 'Lydia';
	  person.name;
	  ```
	- this program will print `Added a new property!` `Access a property!`
	- we can add custom behavior to an object using proxy object
		- we pass a `handler` object with `set` and `get` method
	- the two methods will be invoke when we try to set or get a property
	- reference
		- [Proxy](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Proxy)
		  type:: document
		  tags:: JavaScript, Proxy, Object
		  title:: Proxy
- [[2022-07-16 Saturday]] #Object #Seal
  collapsed:: true
	- ```javascript
	  const person = { name: 'Lydia Hallie' };
	  
	  Object.seal(person);
	  ```
	- `persion.name = "Evan Bacon` can modify the object
	- `Object.seal()` can prevent new properties being added or existing properties being removed for an object
	- reference
		- [Object.seal()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/seal)
		  type:: document
		  tags:: JavaScript, Object, Seal
		  title:: Object.seal()
- [[2022-07-17 Sunday]] #Object #Freeze
  collapsed:: true
	- ```javascript
	  const person = {
	    name: 'Lydia Hallie',
	    address: {
	      street: '100 Main St',
	    },
	  };
	  
	  Object.freeze(person);
	  ```
	- `persion.address.street = "101 Main St` can modify the object
	- `Object.freeze()` can freeze the object, no properties can be added, modified or removed
		- it only shallowly freezes the object
	- reference
		- [Object.freeze()](https://developer.mozilla.org/zh-TW/docs/Web/JavaScript/Reference/Global_Objects/Object/freeze)
		  type:: document
		  tags:: JavaScript, Object, Freeze
		  title:: Object.freeze()
- [[2022-07-18 Monday]] #[[Default Value of Parameters]]
  collapsed:: true
	- ```javascript
	  const add = x => x + x;
	  
	  function myFunc(num = 2, value = add(num)) {
	    console.log(num, value);
	  }
	  
	  myFunc();
	  myFunc(3);
	  ```
	- this program will print `2` `4` and `3` `6`
- [[2022-07-19 Tuesday]] #Class #[[Private Variable]]
  collapsed:: true
	- ```javascript
	  class Counter {
	    #number = 10
	  
	    increment() {
	      this.#number++
	    }
	  
	    getNum() {
	      return this.#number
	    }
	  }
	  
	  const counter = new Counter()
	  counter.increment()
	  
	  console.log(counter.#number)
	  ```
	- this program will print `SyntaxError`
	- we can add private variables in classes using `#`
	- we cannot access private variables outside of the class
- [[2022-07-20 Wednesday]] #[[Generator Function]]
  collapsed:: true
	- ```javascript
	  const teams = [
	    { name: 'Team 1', members: ['Paul', 'Lisa'] },
	    { name: 'Team 2', members: ['Laura', 'Tim'] },
	  ];
	  
	  function* getMembers(members) {
	    for (let i = 0; i < members.length; i++) {
	      yield members[i];
	    }
	  }
	  
	  function* getTeams(teams) {
	    for (let i = 0; i < teams.length; i++) {
	      // ✨ SOMETHING IS MISSING HERE ✨
	    }
	  }
	  
	  const obj = getTeams(teams);
	  obj.next(); // { value: "Paul", done: false }
	  obj.next(); // { value: "Lisa", done: false }
	  ```
	- we should add `yield* getMembers(teams[i].members)`
- [[2022-07-21 Thursday]] #Object #Array #[[Call By Sharing]]
  collapsed:: true
	- ```javascript
	  const person = {
	    name: 'Lydia Hallie',
	    hobbies: ['coding'],
	  };
	  
	  function addHobby(hobby, hobbies = person.hobbies) {
	    hobbies.push(hobby);
	    return hobbies;
	  }
	  
	  addHobby('running', []);
	  addHobby('dancing');
	  addHobby('baking', person.hobbies);
	  
	  console.log(person.hobbies);
	  ```
	- this program will print `["coding", "dancing", baking"]`
	- array in JavaScript is basically an object, so it's call by sharing
- [[2022-07-22 Friday]] #Class #Constructor
  collapsed:: true
	- ```javascript
	  class Bird {
	    constructor() {
	      console.log("I'm a bird. 🦢");
	    }
	  }
	  
	  class Flamingo extends Bird {
	    constructor() {
	      console.log("I'm pink. 🌸");
	      super();
	    }
	  }
	  
	  const pet = new Flamingo();
	  ```
	- this program will print `I'm pink. 🌸` `I'm a bird. 🦢`
	- `super()` calls the constructor of the parent class
- [[2022-07-23 Saturday]] #Object #Array #Const
  collapsed:: true
	- ```javascript
	  const emojis = ['🎄', '🎅🏼', '🎁', '⭐'];
	  
	  /* 1 */ emojis.push('🦌');
	  /* 2 */ emojis.splice(0, 2);
	  /* 3 */ emojis = [...emojis, '🥂'];
	  /* 4 */ emojis.length = 0;
	  ```
	- `emojis = [..emojis, '🥂']` will result in an error
	- we cannot reassign value to variable declared with `const` keyword
	- changing the length of an array will also change the content of the array
- [[2022-07-24 Sunday]] #Iterable #Object #[[Generator Function]]
  collapsed:: true
	- ```javascript
	  const person = {
	    name: "Lydia Hallie",
	    age: 21
	  }
	  
	  [...person] // ["Lydia Hallie", 21]
	  ```
	- we need to add `*[Symbol.iterator]() { yield* Object.values(this) }` to the `person` object
	- objects are not iterable by default
	- we can add `[Symbol.iterator]` to the object
	- reference
		- [Symbol.iterator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Symbol/iterator)
		  type:: document
		  tags:: JavasScript, Iterable, Object, [[Generator Function]] 
		  title:: Symbol.iterator
- [[2022-07-25 Monday]] #False
  collapsed:: true
	- ```javascript
	  let count = 0;
	  const nums = [0, 1, 2, 3];
	  
	  nums.forEach(num => {
	  	if (num) count += 1
	  })
	  
	  console.log(count)
	  ```
	- this program will print `3`
	- `0` is a falsy value
- [[2022-07-26 Tuesday]]
  collapsed:: true
	- ```javascript
	  function getFruit(fruits) {
	  	console.log(fruits?.[1]?.[1])
	  }
	  
	  getFruit([['🍊', '🍌'], ['🍍']])
	  getFruit()
	  getFruit([['🍍'], ['🍊', '🍌']])
	  ```
	- this program will print `undefined` `undefined` ` 🍌`
	- `?` allows us to optionally access deeper nested properties within objects
- [[2022-07-27 Wednesday]] #Object #Class #Constructor
  collapsed:: true
	- ```javascript
	  class Calc {
	  	constructor() {
	  		this.count = 0 
	  	}
	  
	  	increase() {
	  		this.count ++
	  	}
	  }
	  
	  const calc = new Calc()
	  new Calc().increase()
	  
	  console.log(calc.count)
	  ```
	- this program will print `0`
	- the `count` property is not shared on the prototype of `Calc`
- [[2022-07-28 Thursday]] #Object #[[Call By Sharing]]
  collapsed:: true
	- ```javascript
	  const user = {
	  	email: "e@mail.com",
	  	password: "12345"
	  }
	  
	  const updateUser = ({ email, password }) => {
	  	if (email) {
	  		Object.assign(user, { email })
	  	}
	  
	  	if (password) {
	  		user.password = password
	  	}
	  
	  	return user
	  }
	  
	  const updatedUser = updateUser({ email: "new@email.com" })
	  
	  console.log(updatedUser === user)
	  ```
	- this program will print `true`
	- the return value of `updateUser` references to `user`
- [[2022-07-29 Friday]] #Array
  collapsed:: true
	- ```javascript
	  const fruit = ['🍌', '🍊', '🍎']
	  
	  fruit.slice(0, 1)
	  fruit.splice(0, 1)
	  fruit.unshift('🍇')
	  
	  console.log(fruit)
	  ```
	- this program will print `['🍇', '🍊', '🍎']`
	- `slice()` doesn't modify the original array
	- `splice` modify the original array
	- `unshift()` modify the original array and add the content as the first element of the array
- [[2022-07-30 Saturday]] #Object
  collapsed:: true
	- ```javascript
	  const animals = {};
	  let dog = { emoji: '🐶' }
	  let cat = { emoji: '🐈' }
	  
	  animals[dog] = { ...dog, name: "Mara" }
	  animals[cat] = { ...cat, name: "Sara" }
	  
	  console.log(animals[dog])
	  ```
	- this program will print `{ emoji: "🐈", name: "Sara" }`
	- using object as key is using `"object Object"` as key
- [[2022-07-31 Sunday]] #Object #[[Arrow Function]]
  collapsed:: true
	- ```javascript
	  const user = {
	  	email: "my@email.com",
	  	updateEmail: email => {
	  		this.email = email
	  	}
	  }
	  
	  user.updateEmail("new@email.com")
	  console.log(user.email)
	  ```
	- this program will print `my@email.com`
	- `updateEmail` is an arrow function, so it's not bind to `user`