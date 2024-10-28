title:: JavaScript Questions/2022-05

- [[2022-05-01 Sunday]] #Unpack #Array
  collapsed:: true
	- ```javascript
	  const numbers = [1, 2, 3, 4, 5];
	  const [y] = numbers;
	  
	  console.log(y);
	  ```
	- this program will print `1`
	- to correctly unpack the values in an array, we should do `[a, b, c, d, e] = [1, 2, 3, 4, 5]`
	- `[y] = [1 ,2, 3, 4, 5]` will only make `y` equal to `1`
- [[2022-05-02 Monday]] #Object #[[Spread Operator]]
  collapsed:: true
	- ```javascript
	  const user = { name: 'Lydia', age: 21 };
	  const admin = { admin: true, ...user };
	  
	  console.log(admin);
	  ```
	- this program will print `{admin: true, name: "Lydia", age: 21}`
	- `...` is a spread operator, it creates a copy of the key-value pairs of an object
		- it doesn't copy the object, it copies the key-value pairs
- [[2022-05-03 Tuesday]] #Object #Enumerable
  collapsed:: true
	- ```javascript
	  const person = { name: 'Lydia' };
	  
	  Object.defineProperty(person, 'age', { value: 21 });
	  
	  console.log(person);
	  console.log(Object.keys(person));
	  ```
	- this program will print `{ name: "Lydia", age: 21}`, `["name"]`
	- we can add new properties to an object using `defineProperty` method, but those properties are not enumerable in default
		- `Object.keys()` method can only return enumerable properties name
		- we can change the behavior of `Object.defineProperty()` by adding additional properties in the descriptor
- [[2022-05-04 Wednesday]] #Object
  collapsed:: true
	- ```javascript
	  const settings = {
	    username: 'lydiahallie',
	    level: 19,
	    health: 90,
	  };
	  
	  const data = JSON.stringify(settings, ['level', 'health']);
	  console.log(data);
	  ```
	- this program will print `"{ "level": 19, "health": 90 }"`
	- the second argument of `JSON.stringify()` method is a replacer, it lets you control what and how the values should be stringified
	- if the replacer is an array, only the property names included in the array will be added to the JSON string
	- if the replacer is a function, this function gets called on every property in the object you're stringfying
		- if the value of a property is `undefined`, then that property is excluded
	- reference
		- [JSON.stringify()](https://developer.mozilla.org/zh-TW/docs/Web/JavaScript/Reference/Global_Objects/JSON/stringify) 
		  type:: document
		  tags:: JavaScript, Object, String
		  title:: JSON.stringify()
- [[2022-05-05 Thursday]] #[[Postfix Operator]]
  collapsed:: true
	- ```javascript
	  let num = 10;
	  
	  const increaseNumber = () => num++;
	  const increasePassedNumber = number => number++;
	  
	  const num1 = increaseNumber();
	  const num2 = increasePassedNumber(num1);
	  
	  console.log(num1);
	  console.log(num2);
	  ```
	- this program will print `10` `10`
	- the postfix operator will return the value first, then increment the value
	- in both cases, the functions both return `10`
- [[2022-05-06 Friday]] #Object #[[Default Value of Parameters]] #[[Spread Operator]]
  collapsed:: true
	- ```javascript
	  const value = { number: 10 };
	  
	  const multiply = (x = { ...value }) => {
	    console.log((x.number *= 2));
	  };
	  
	  multiply();
	  multiply();
	  multiply(value);
	  multiply(value);
	  ```
	- this program will print `20` `20` `20` `40`
	- we can provide default value to the parameters of a function
		- parameter will be set to default value if no argument is passed to the function, or the parameter gets `undefined`
	- we use a spread operator to copy the object, and use it as the default value
		- the change we make won't affect the original object
	- if we pass the object into the function, we then make the change directly onto the object
- [[2022-05-07 Saturday]] #Reduce #Array
  collapsed:: true
	- ```javascript
	  [1, 2, 3, 4].reduce((x, y) => console.log(x, y));
	  ```
	- this program will print `1` `2` `undefined` `3` `undefined` `4`
	- the first argument of `reduce()` is the accumulator
		- its value is equal to the previously returned value of the callback function
		- if we don't pass the initial value argument to `reduce`, it will default to the first element in the array
	- the second argument is the current value
	- we don't have a return statement, so it returns `undefined`
	- reference
		- {{embed ((6273c8aa-7895-406a-8f80-fbecdf2fb633))}}
- [[2022-05-08 Sunday]] #Class
  collapsed:: true
	- ```javascript
	  class Dog {
	    constructor(name) {
	      this.name = name;
	    }
	  };
	  
	  class Labrador extends Dog {
	    // 1
	    constructor(name, size) {
	      this.size = size;
	    }
	    // 2
	    constructor(name, size) {
	      super(name);
	      this.size = size;
	    }
	    // 3
	    constructor(size) {
	      super(name);
	      this.size = size;
	    }
	    // 4
	    constructor(name, size) {
	      this.name = name;
	      this.size = size;
	    }
	  
	  };
	  ```
	- the second constructor can successfully extend the `Dog` class
	- we cannot access `this` before calling `super()` in the derived class
	- we need to pass arguments the parent's constructor needs to `super()`
- [[2022-05-09 Monday]] #Import
  collapsed:: true
	- ```javascript
	  // index.js
	  console.log('running index.js');
	  import { sum } from './sum.js';
	  console.log(sum(1, 2));
	  
	  // sum.js
	  console.log('running sum.js');
	  export const sum = (a, b) => a + b;
	  ```
	- this program will print `running sum.js` `running index.js` `3`
	- all imported modules are pre-parsed, so they get run first
	- `require()` will load dependencies on demand
- [[2022-05-10 Tuesday]] #Object #Symbol
  collapsed:: true
	- ```javascript
	  console.log(Number(2) === Number(2));
	  console.log(Boolean(false) === Boolean(false));
	  console.log(Symbol('foo') === Symbol('foo'));
	  ```
	- this program will print `true` `true` `false`
	- the argument passed to `Symbol()` is the description of the symbol
	- every symbol is unique
	- `Symbol()` does not require `new` operator to create new object
	- reference
	  collapsed:: true
		- [Symbol](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Symbol) 
		  type:: document
		  tags:: Symbol, JavaScript, Object
		  title:: Symbol
- [[2022-05-11 Wednesday]] #String
  collapsed:: true
	- ```javascript
	  const name = 'Lydia Hallie';
	  console.log(name.padStart(13));
	  console.log(name.padStart(2));
	  ```
	- this program will print `" Lydia Hallie"` `"Lydia Hallie"`
	- we can add padding to the beginning of a string using `padStart()`
	- the argument passed to `padStart()` is the total length of the string
	- there will be no padding added if the argument is smaller than the string length
- [[2022-05-12 Thursday]] #[[Generator Function]]
  collapsed:: true
	- ```javascript
	  function* startGame() {
	    const answer = yield 'Do you love JavaScript?';
	    if (answer !== 'Yes') {
	      return "Oh wow... Guess we're gone here";
	    }
	    return 'JavaScript loves you back ❤️';
	  }
	  
	  const game = startGame();
	  console.log(/* 1 */); // Do you love JavaScript?
	  console.log(/* 2 */); // JavaScript loves you back ❤️
	  ```
	- we have to log `game.next().value` and `game.next("Yes").value` to get the desired output
	- a generator function pauses its execution when it sees the `yield` keyword
	- the execution will pause before assignment on the first line happens
	- when the function executes again, the previous `yield` is replaced with the value passed to `next()`
- [[2022-05-13 Friday]] #String
  collapsed:: true
	- ```javascript
	  console.log(String.raw`Hello\nworld`);
	  ```
	- this program will print `Hello\nworld`
	- `String.raw` returns a string where escape characters are ignored
	- it allows us to use backslashes in the string
	- reference
		- [String.raw()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/raw) 
		  type:: document
		  tags:: JavaScript, String, [[Escape Character]]
		  title:: String.raw()
- [[2022-05-14 Saturday]] #Promise #Asynchronous
  collapsed:: true
	- ```javascript
	  async function getData() {
	    return await Promise.resolve('I made it!');
	  }
	  
	  const data = getData();
	  console.log(data);
	  ```
	- this program will print `Promise {<pending>}`
	- we didn't add `await` in front of `getData()`, so the assignment won't wait for the promise to resolve
- [[2022-05-15 Sunday]] #Array
  collapsed:: true
	- ```javascript
	  function addToList(item, list) {
	    return list.push(item);
	  }
	  
	  const result = addToList('apple', ['banana']);
	  console.log(result);
	  ```
	- this program will print `2`
	- `push()` method returns the length of the new array
- [[2022-05-16 Monday]] #Object
  collapsed:: true
	- ```javascript
	  const box = { x: 10, y: 20 };
	  
	  Object.freeze(box);
	  
	  const shape = box;
	  shape.x = 100;
	  
	  console.log(shape);
	  ```
	- this program will print `{x: 10, y: 20}`
	- `Object.freeze()` makes it impossible to add, remove or modify properties of the object
		- if the property is another object, then it can be modified
	- `shape` references to the same frozen object, so we are unable to change its property
	- reference
		- [Object.freeze()](https://developer.mozilla.org/zh-TW/docs/Web/JavaScript/Reference/Global_Objects/Object/freeze) 
		  type:: document
		  tags:: JavaScript, Object
		  title:: Object.freeze()
- [[2022-05-17 Tuesday]] #Object #Unpack
  collapsed:: true
	- ```javascript
	  const { name: myName } = { name: 'Lydia' };
	  
	  console.log(name);
	  ```
	- this program will print `undefined`
	- we unpack the `name` property from the object, and its value is stored in `myName`
	- `name` is never declared, so the program will print `undefined`
- [[2022-05-18 Wednesday]] #[[Pure Function]]
  collapsed:: true
	- ```javascript
	  function sum(a, b) {
	    return a + b;
	  }
	  ```
	- this is a pure function
	- a pure function is a function that always returns the same result if the same arguments are passed
- [[2022-05-19 Thursday]] #Closure #[[Variable Capture]]
  collapsed:: true
	- ```javascript
	  const add = () => {
	    const cache = {};
	    return num => {
	      if (num in cache) {
	        return `From cache! ${cache[num]}`;
	      } else {
	        const result = num + 10;
	        cache[num] = result;
	        return `Calculated! ${result}`;
	      }
	    };
	  };
	  
	  const addFunction = add();
	  console.log(addFunction(10));
	  console.log(addFunction(10));
	  console.log(addFunction(5 * 2));
	  ```
	- this program will print `Calculated! 20` `From cache! 20` `From cache! 20`
	- `cache` was captured by the function returned by `add()`
		- the function can access the same `cache`
	- reference
	  collapsed:: true
		- [閉包](https://developer.mozilla.org/zh-TW/docs/Web/JavaScript/Closures) 
		  type:: document
		  tags:: JavaScript, Closure, [[Variable Capture]] 
		  title:: 閉包
- [[2022-05-20 Friday]] #Object #Array #Loop
  collapsed:: true
	- ```javascript
	  const myLifeSummedUp = ['☕', '💻', '🍷', '🍫'];
	  
	  for (let item in myLifeSummedUp) {
	    console.log(item);
	  }
	  
	  for (let item of myLifeSummedUp) {
	    console.log(item);
	  }
	  ```
	- this program will print `0` `1` `2` `3` `☕` `💻` `🍷` `🍫`
	- in a for-in loop, we can iterate over enumerable properties
		- for an array, it's its keys
	- in a for-of loop, we can iterate over iterables
		- an array is an iterable
- [[2022-05-21 Saturday]] #Array
  collapsed:: true
	- ```javascript
	  const list = [1 + 2, 1 * 2, 1 / 2];
	  console.log(list);
	  ```
	- this program will print `[3, 2, 0.5]`
- [[2022-05-22 Sunday]] #[[Default Value of Parameters]]
  collapsed:: true
	- ```javascript
	  function sayHi(name) {
	    return `Hi there, ${name}`;
	  }
	  
	  console.log(sayHi());
	  ```
	- this program will print `Hi there, undefined`
	- arguments have default value of `undefined`
- [[2022-05-23 Monday]] #this #Object
  collapsed:: true
	- ```javascript
	  var status = '😎';
	  
	  setTimeout(() => {
	    const status = '😍';
	  
	    const data = {
	      status: '🥑',
	      getStatus() {
	        return this.status;
	      },
	    };
	  
	    console.log(data.getStatus());
	    console.log(data.getStatus.call(this));
	  }, 0);
	  ```
	- this program will print `🥑` and `😎`
	- `this` refers to the object that the method belongs to
	- we can assign `this` by using `call()`
	- `setTimeout` is declared under global object, so its `this` refers to global object
- [[2022-05-24 Tuesday]] #Object
  collapsed:: true
	- ```javascript
	  const person = {
	    name: 'Lydia',
	    age: 21,
	  };
	  
	  let city = person.city;
	  city = 'Amsterdam';
	  
	  console.log(person);
	  ```
	- this program will print `{name: "Lydia", age: 21}`
	- we initially assign `undefined` to `city`
	- when we set `city` to `Amsterdam`, we didn't change `person`
- [[2022-05-25 Wednesday]] #Variable #Scope
  collapsed:: true
	- ```javascript
	  function checkAge(age) {
	    if (age < 18) {
	      const message = "Sorry, you're too young.";
	    } else {
	      const message = "Yay! You're old enough!";
	    }
	  
	    return message;
	  }
	  
	  console.log(checkAge(21));
	  ```
	- this program will print `ReferenceError`
	- `const` variables are block-scoped
	- we cannot reference a block-scoped varilabe outside of its block
- [[2022-05-26 Thursday]] #Promise #[[Callback Function]]
  collapsed:: true
	- ```javascript
	  fetch('https://www.website.com/api/user/1')
	    .then(res => res.json())
	    .then(res => console.log(res));
	  ```
	- this program will print the result of the callback in the previous `.then()`
- [[2022-05-27 Friday]]
  collapsed:: true
	- ```javascript
	  function getName(name) {
	    const hasName = //
	  }
	  ```
	- we can set `hasName` to `true` by assigning it `!!name`
	- `!false` returns `true`
- [[2022-05-28 Saturday]]
  collapsed:: true
	- ```javascript
	  console.log('I want pizza'[0]);
	  ```
	- this program will print `"I"`
- [[2022-05-29 Sunday]] #[[Default Value of Parameters]]
  collapsed:: true
	- ```javascript
	  function sum(num1, num2 = num1) {
	    console.log(num1 + num2);
	  }
	  
	  sum(10);
	  ```
	- this program will print `20`
	- the value of a parameter can be another parameter, so long as it is defined before the default parameter
- [[2022-05-30 Monday]] #Module
  collapsed:: true
	- ```javascript
	  // module.js
	  export default () => 'Hello world';
	  export const name = 'Lydia';
	  
	  // index.js
	  import * as data from './module';
	  
	  console.log(data);
	  ```
	- this program will print `{default: function default(), name: "Lydia"}`
	- we import all exports from `module.js` as an object `data`
	- the object has a `default` property for default export
- [[2022-05-31 Tuesday]] #Object #[[Function Constructor]]
  collapsed:: true
	- ```javascript
	  class Person {
	    constructor(name) {
	      this.name = name;
	    }
	  }
	  
	  const member = new Person('John');
	  console.log(typeof member);
	  ```
	- this program will print `object`
	- `class` is syntactical sugar for function constructors