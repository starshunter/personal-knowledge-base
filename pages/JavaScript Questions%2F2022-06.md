title:: JavaScript Questions/2022-06

- [[2022-06-01 Wednesday]] #Array
  collapsed:: true
	- ```javascript
	  let newList = [1, 2, 3].push(4);
	  
	  console.log(newList.push(5));
	  ```
	- this program will print `Error`
	- `push()` method returns the new length of the array
	- `newList` is a number, so we can't call `push()`
- [[2022-06-02 Thursday]] #Function #[[Arrow Function]] #Prototype
  collapsed:: true
	- ```javascript
	  function giveLydiaPizza() {
	    return 'Here is pizza!';
	  }
	  
	  const giveLydiaChocolate = () =>
	    "Here's chocolate... now go hit the gym already.";
	  
	  console.log(giveLydiaPizza.prototype);
	  console.log(giveLydiaChocolate.prototype);
	  ```
	- this program will print `{constructor: ...}` `undefined`
	- regular functions have a `prototype` property, which is an object that has a `constructor` property
	- arrow functions don't have `prototype` property
- [[2022-06-03 Friday]] #[[Destructuring Assignment]] #Loop #Object
  collapsed:: true
	- ```javascript
	  const person = {
	    name: 'Lydia',
	    age: 21,
	  };
	  
	  for (const [x, y] of Object.entries(person)) {
	    console.log(x, y);
	  }
	  ```
	- this program will print `name` `Lydia` and `age` `21`
	- `Object.entries()` returns an array of nested arrays, containing the keys and objects
	- use `for-of` loop we can iterate over each element in the array
	- we use `const [x, y]` to destruct the subarray
- [[2022-06-04 Saturday]] #[[Rest Parameter]]
  collapsed:: true
	- ```javascript
	  function getItems(fruitList, ...args, favoriteFruit) {
	    return [...fruitList, ...args, favoriteFruit]
	  }
	  
	  getItems(["banana", "apple"], "pear", "orange")
	  ```
	- this program will print `SyntaxError`
	- the rest parameter can only be the last parameter
- [[2022-06-05 Sunday]] #[[JavaScript Engine]] #Function
  collapsed:: true
	- ```javascript
	  function nums(a, b) {
	    if (a > b) console.log('a is bigger');
	    else console.log('b is bigger');
	    return
	    a + b;
	  }
	  
	  console.log(nums(4, 2));
	  console.log(nums(1, 2));
	  ```
	- this program will print `a is bigger` `undefined` and `b is bigger` `undefined`
	- JavaScript engine will automatically insert semicolons to lines that do not end with semicolons
	- since `a + b` is on a new line, it is never reached because a semicolon will be inserted after `return`
	- the function return `undefined` if it doesn't return anything
- [[2022-06-06 Monday]] #Class
  collapsed:: true
	- ```javascript
	  class Person {
	    constructor() {
	      this.name = 'Lydia';
	    }
	  }
	  
	  Person = class AnotherPerson {
	    constructor() {
	      this.name = 'Sarah';
	    }
	  };
	  
	  const member = new Person();
	  console.log(member.name);
	  ```
	- this program will print `Sarah`
	- we can set classes equal to other classes or function constructors
- [[2022-06-07 Tuesday]] #Symbol #Object #Enumerable
  collapsed:: true
	- ```javascript
	  const info = {
	    [Symbol('a')]: 'b',
	  };
	  
	  console.log(info);
	  console.log(Object.keys(info));
	  ```
	- this program will print `{Symbol('a'): 'b'}` and `[]`
	- a symbol is not enumerable
	- `Object.keys()` will return all enumerable key properties
	- when logging an object, all properties will be visible
- [[2022-06-08 Wednesday]] #[[Destructuring Assignment]] #[[Arrow Function]]
  collapsed:: true
	- ```javascript
	  const getList = ([x, ...y]) => [x, y]
	  const getUser = user => { name: user.name, age: user.age }
	  
	  const list = [1, 2, 3, 4]
	  const user = { name: "Lydia", age: 21 }
	  
	  console.log(getList(list))
	  console.log(getUser(user))
	  ```
	- this program will print `[1, [2, 3, 4]]` and `SyntaxError`
	- for an arrow function, every thing between the two braces will be interpreted as a block statement
		- so `getUser` has to add parentheses to immediately return the object
- [[2022-06-09 Thursday]] #Type
  collapsed:: true
	- ```javascript
	  const name = 'Lydia';
	  
	  console.log(name());
	  ```
	- this program will print `TypeError`
	- `TypeError` get thrown when a value is not of the expected type
	- `SyntaxError` get thrown when something isn't valid JavaScript
	- `ReferenceError` get thrown when JavaScript can't find a reference to a value that you're trying to access
- [[2022-06-10 Friday]] #True #False #String
  collapsed:: true
	- ```javascript
	  // 🎉✨ This is my 100th question! ✨🎉
	  
	  const output = `${[] && 'Im'}possible!
	  You should${'' && `n't`} see a therapist after so much JavaScript lol`;
	  ```
	- this program will print `Impossible! You should see a therapist after so much JavaScript lol`
	- with `&&` operator, the right-hand value will be returned if the left-hand value is a truthy value
	- `[]` is a truthy value, and `""` is a falsy value
- [[2022-06-11 Saturday]] #True #False #[[OR Operator]]
  collapsed:: true
	- ```javascript
	  const one = false || {} || null;
	  const two = null || false || '';
	  const three = [] || 0 || true;
	  
	  console.log(one, two, three);
	  ```
	- this program will print `{}` `""` `[]`
	- with `||`, it will return the first truthy operand, if there isn't any, then it will return the last operand
- [[2022-06-12 Sunday]] #Promise #Asynchronous
  collapsed:: true
	- ```javascript
	  const myPromise = () => Promise.resolve('I have resolved!');
	  
	  function firstFunction() {
	    myPromise().then(res => console.log(res));
	    console.log('second');
	  }
	  
	  async function secondFunction() {
	    console.log(await myPromise());
	    console.log('second');
	  }
	  
	  firstFunction();
	  secondFunction();
	  ```
	- this program will print `second` `I have resolved!` and `I have resolved` `second`
- [[2022-06-13 Monday]] #Object #String #[[Implicit Coercion]]
  collapsed:: true
	- ```javascript
	  const set = new Set();
	  
	  set.add(1);
	  set.add('Lydia');
	  set.add({ name: 'Lydia' });
	  
	  for (let item of set) {
	    console.log(item + 2);
	  }
	  ```
	- this program will print `3` `Lydia2` `[object Object]2`
	- `+` can be used to concatenate strings, whenever JavaScript engine sees one or more operands are not numbers, it coerces the number into a string
	- when we stringify an object, it becomes `[object Object]`
- [[2022-06-14 Tuesday]] #Promise #Resolve
  collapsed:: true
	- ```javascript
	  Promise.resolve(5);
	  ```
	- this program will print `Promise {<fulfilled>: 5}`
	- we can pass any type of value we want to `Promise.resolve()`
	- if you pass a regular function, it will be a resolved promise with a regular value
	- if you pass a promise, it will be a resolved promise with the resolved value of that promise
- [[2022-06-15 Wednesday]] #Object #[[Call By Sharing]]
  collapsed:: true
	- ```javascript
	  function compareMembers(person1, person2 = person) {
	    if (person1 !== person2) {
	      console.log('Not the same!');
	    } else {
	      console.log('They are the same!');
	    }
	  }
	  
	  const person = { name: 'Lydia' };
	  
	  compareMembers(person);
	  ```
	- this program will print `They are the same!`
	- JavaScript is call by sharing
	- we compare their references when we use `===` on two objects
- [[2022-06-16 Thursday]] #Object
  collapsed:: true
	- ```javascript
	  const colorConfig = {
	    red: true,
	    blue: false,
	    green: true,
	    black: true,
	    yellow: false,
	  };
	  
	  const colors = ['pink', 'red', 'blue'];
	  
	  console.log(colorConfig.colors[1]);
	  ```
	- this program will print `TypeError`
	- we try to access the second element of `colorConfig.colors`, which is `undefined`
- [[2022-06-17 Friday]] #String
  collapsed:: true
	- ```javascript
	  console.log('❤️' === '❤️');
	  ```
	- this program will print `true`
	- emojis are unicodes under the hood
- [[2022-06-18 Saturday]] #Map #Reduce #Filter #Splice
  collapsed:: true
	- ```javascript
	  const emojis = ['✨', '🥑', '😍'];
	  
	  emojis.map(x => x + '✨');
	  emojis.filter(x => x !== '🥑');
	  emojis.find(x => x !== '🥑');
	  emojis.reduce((acc, cur) => acc + '✨');
	  emojis.slice(1, 2, '✨');
	  emojis.splice(1, 2, '✨');
	  ```
	- only `splice` will modify the original array
- [[2022-06-19 Sunday]] #String #Type #[[Primitive Data Type]] #[[Call By Sharing]]
  collapsed:: true
	- ```javascript
	  const food = ['🍕', '🍫', '🥑', '🍔'];
	  const info = { favoriteFood: food[0] };
	  
	  info.favoriteFood = '🍝';
	  
	  console.log(food);
	  ```
	- this program will print `['🍕', '🍫', '🥑', '🍔']`
	- a string in javascript is a primitive data type
	- the value of `favoriateFood` property of `info` is just a copy of `food[0]`, so changing it won't change `food`
- [[2022-06-20 Monday]] #JSON
  collapsed:: true
	- ```javascript
	  JSON.parse();
	  ```
	- this method parses JSON to a javascript value
- [[2022-06-21 Tuesday]] #Variable #Hoist #Scope
  collapsed:: true
	- ```javascript
	  let name = 'Lydia';
	  
	  function getName() {
	    console.log(name);
	    let name = 'Sarah';
	  }
	  
	  getName();
	  ```
	- this program will print `ReferenceError`
	- each function first looks within its scope to see if it contains the variables we're trying to access
	- variables with `let` keyword are hoisted, but not initialized
	- we get `ReferenceError` if we try to access a variable before it's declared
- [[2022-06-22 Wednesday]] #[[Generator Function]]
  collapsed:: true
	- ```javascript
	  function* generatorOne() {
	    yield ['a', 'b', 'c'];
	  }
	  
	  function* generatorTwo() {
	    yield* ['a', 'b', 'c'];
	  }
	  
	  const one = generatorOne();
	  const two = generatorTwo();
	  
	  console.log(one.next().value);
	  console.log(two.next().value);
	  ```
	- this program will print `['a', 'b', 'c']` and `a`
	- we can yield values from another generator function or iterable object using `yield*`
- [[2022-06-23 Thursday]] [[Immediately Invoked Function]]
  collapsed:: true
	- ```javascript
	  console.log(`${(x => x)('I love')} to program`);
	  ```
	- this program will print `I love to program`
	- expressions within template literals are evaluated first
- [[2022-06-24 Friday]] #Object #[[Garbage Collection]] #[[Arrow Function]]
  collapsed:: true
	- ```javascript
	  let config = {
	    alert: setInterval(() => {
	      console.log('Alert!');
	    }, 1000),
	  };
	  
	  config = null;
	  ```
	- the `setInterval` callback will still be called every second
	- because the callback of `setInterval` is an arrow function, it still holds a reference to the `config` object
		- the object won't be garbage-collected
- [[2022-06-25 Saturday]] #Function #[[Call By Sharing]]
  collapsed:: true
	- ```javascript
	  const myMap = new Map();
	  const myFunc = () => 'greeting';
	  
	  myMap.set(myFunc, 'Hello world!');
	  
	  //1
	  myMap.get('greeting');
	  //2
	  myMap.get(myFunc);
	  //3
	  myMap.get(() => 'greeting');
	  ```
	- the second method will return `Hello world!`
	- the function `() => 'greeting` is added to the map
	- object is call by sharing
- [[2022-06-26 Sunday]] #[[Call By Sharing]] #Object #[[Default Value of Parameters]]
  collapsed:: true
	- ```javascript
	  const person = {
	    name: 'Lydia',
	    age: 21,
	  };
	  
	  const changeAge = (x = { ...person }) => (x.age += 1);
	  const changeAgeAndName = (x = { ...person }) => {
	    x.age += 1;
	    x.name = 'Sarah';
	  };
	  
	  changeAge(person);
	  changeAgeAndName();
	  
	  console.log(person);
	  ```
	- this program will print `{name: "Lydia", age: 22}`
	- `{...person}` copy all the key-value pairs in the `person` object
- [[2022-06-27 Monday]] #[[Spread Operator]]
  collapsed:: true
	- ```javascript
	  function sumValues(x, y, z) {
	    return x + y + z;
	  }
	  ```
	- `sumValues(...[1, 2, 3])` will return `6`
	- we can use spread operator to spread iterables to individual elements
- [[2022-06-28 Tuesday]]
  collapsed:: true
	- ```javascript
	  let num = 1;
	  const list = ['🥳', '🤠', '🥰', '🤪'];
	  
	  console.log(list[(num += 1)]);
	  ```
	- this program will print `🥰`
	- the `+=` operand will return the incremented value
- [[2022-06-29 Wednesday]] #[[Optional Chaining Operator]] #Object
  collapsed:: true
	- ```javascript
	  const person = {
	    firstName: 'Lydia',
	    lastName: 'Hallie',
	    pet: {
	      name: 'Mara',
	      breed: 'Dutch Tulip Hound',
	    },
	    getFullName() {
	      return `${this.firstName} ${this.lastName}`;
	    },
	  };
	  
	  console.log(person.pet?.name);
	  console.log(person.pet?.family?.name);
	  console.log(person.getFullName?.());
	  console.log(member.getLastName?.());
	  ```
	- this program will print `Mara` `undefined` `Lydia Hallie` `ReferenceError`
	- with the optional chaining operator `?.`, we don't need to check whether the deeper nested values are valid or not
		- we will get `undefined` if we try to access a property of `undefined` or `null`
	- reference
		- [Optional chaining (?.)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Optional_chaining)
		  type:: document
		  tags:: JavaScript, Object
		  title:: Optional chaining (?.)
- [[2022-06-30 Thursday]]
  collapsed:: true
	- ```javascript
	  const groceries = ['banana', 'apple', 'peanuts'];
	  
	  if (groceries.indexOf('banana')) {
	    console.log('We have to buy bananas!');
	  } else {
	    console.log(`We don't have to buy bananas!`);
	  }
	  ```
	- this program will print `We don't have to buy bananas`
	- the index of `banana` is `0`