title:: JavaScript Questions/2022-04

- [[2022-04-01 Friday]] #Object
  collapsed:: true
	- ```javascript
	  const a = {};
	  const b = { key: 'b' };
	  const c = { key: 'c' };
	  
	  a[b] = 123;
	  a[c] = 456;
	  
	  console.log(a[b]);
	  ```
	- this program will print `456`
	- the object will be converted to `"[object Object]"` if we use it as key
	- so the assignments will assign different values to the same key
- [[2022-04-02 Saturday]] #[[Event Loop]] #[[Callback Function]]
  collapsed:: true
	- ```javascript
	  const foo = () => console.log('First');
	  const bar = () => setTimeout(() => console.log('Second'));
	  const baz = () => console.log('Third');
	  
	  bar();
	  foo();
	  baz();
	  ```
	- this program will print `First` `Third` `Second`
	- the callback function will be pushed to the WebAPI queue
	- when the timer expires, the callback function is pushed to a queue
	- and event loop will take the function out of the queue if there is no instruction to execute in the stack
- [[2022-04-03 Sunday]] #Event
  collapsed:: true
	- ```javascript
	  <div onclick="console.log('first div')">
	    <div onclick="console.log('second div')">
	      <button onclick="console.log('button')">
	        Click!
	      </button>
	    </div>
	  </div>
	  ```
	- `<button>` will be the event target if we click the button
	- the deepest nested element that causes the event is the target of the event
	- {{embed ((624219a2-5583-4ae6-b2b1-56e2451e7068))}}
- [[2022-04-04 Monday]] #Event
  collapsed:: true
	- ```javascript
	  <div onclick="console.log('div')">
	    <p onclick="console.log('p')">
	      Click here!
	    </p>
	  </div>
	  ```
	- the console will display `p` `div` if we click it
	- by default, event handlers are executed in the bubbling phase
- [[2022-04-05]] #this
  collapsed:: true
	- ```javascript
	  const person = { name: 'Lydia' };
	  
	  function sayHi(age) {
	    return `${this.name} is ${age}`;
	  }
	  
	  console.log(sayHi.call(person, 21));
	  console.log(sayHi.bind(person, 21));
	  ```
	- this program will print `Lydia is 21` `funciton`
	- both `call()` and `bind()` can pass the object, and use `this` to access object member
	- `call()` will execute the function, but `bind()` won't
- [[2022-04-06 Wednesday]] #Function #[[Immediately Invoked Function]]
  collapsed:: true
	- ```javascript
	  function sayHi() {
	    return (() => 0)();
	  }
	  
	  console.log(typeof sayHi());
	  ```
	- this program will print `"number"`
	- the `sayHi()` return an immediately invoked function expression, which return `0`
- [[2022-04-07 Thursday]] #False #True
  collapsed:: true
	- ```javascript
	  0;
	  new Number(0);
	  ('');
	  (' ');
	  new Boolean(false);
	  undefined;
	  ```
	- `0` `''` `undefined` are falsy values
	- there are 8 falsy values in javascript
	  collapsed:: true
		- `undefined`
		- `null`
		- `NaN`
		- `false`
		- `''`
		- `0`
		- `-0`
		- `0n`
	- function constructors are truthy
- [[2022-04-08 Friday]] #Typeof
  collapsed:: true
	- ```javascript
	  console.log(typeof typeof 1);
	  ```
	- this program will print `"string"`
	- `typeof 1` return `"number"`, and `typeof "number"` return `"string"`
- [[2022-04-09 Saturday]] #Array
  collapsed:: true
	- ```javascript
	  const numbers = [1, 2, 3];
	  numbers[10] = 11;
	  console.log(numbers);
	  ```
	- this program will print `[1, 2, 3, empty x 7, 11]`
	- when you set a value in a position that exceeds an array's length, javascript will assign `undefined` in other empty spots, but in browser, those slots will be represented by `empty`
- [[2022-04-10 Sunday]] #Scope #Variable
  collapsed:: true
	- ```javascript
	  (() => {
	    let x, y;
	    try {
	      throw new Error();
	    } catch (x) {
	      (x = 1), (y = 2);
	      console.log(x);
	    }
	    console.log(x);
	    console.log(y);
	  })();
	  ```
	- this program will print `1` `undefined` `2`
	- the `x` that the catch block receives is not the `x` declared on line 2
		- this `x` is block-scoped
	- in the catch block, we assign the new `x` to 1, and `y` to 2
		- this `y` refers to the `y` declared on line 2
	- so outside the catch block, `x` hasn't been assigned a value, but `y` does
- [[2022-04-11 Monday]] #Type #Object
  collapsed:: true
	- A: primitive or object
	  B: function or object
	  C: trick question! only objects
	  D: number or object
	- the answer is A
	- primitive types are
	  collapsed:: true
		- `boolean`
		- `null`
		- `undefined`
		- `bigint`
		- `number`
		- `string`
		- `symbol`
	- primitives don't have properties or methods, but if you access a method or a property on a primitive, javascript will wrap that primitive into an object
	  collapsed:: true
		- this behavior exists for all primitives, except for `null` and `undefined`
- [[2022-04-12 Tuesday]]
  collapsed:: true
	- ```javascript
	  [[0, 1], [2, 3]].reduce(
	    (acc, cur) => {
	      return acc.concat(cur);
	    },
	    [1, 2],
	  );
	  ```
	- this program will print `[1, 2, 0, 1, ,2, 3]`
	- `[1, 2]` is the initial value, and also is the initial `acc`
	- `reduce` will loop through the array and concatenate each element after the initial value
	- reference
	  id:: 6273c8aa-0824-4d5b-9f2b-a81b45b41f9d
		- [Array.prototype.reduce()](https://developer.mozilla.org/zh-TW/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce)
		  type:: document
		  tags:: JavaScript, Reduce, Array
		  title:: Array.prototype.reduce()
		  id:: 6273c8aa-7895-406a-8f80-fbecdf2fb633
- [[2022-04-13 Wednesday]] #False
  collapsed:: true
	- ```javascript
	  !!null;
	  !!'';
	  !!1;
	  ```
	- this program will print `false` `false` `true`
	- `null` is falsy
	- `''` is falsy
	- `1` is falsy
- [[2022-04-14 Thursday]] #setInterval
  collapsed:: true
	- ```javascript
	  setInterval(() => console.log('Hi'), 1000);
	  ```
	- this program will a unique id, which can be used to clear this interval with `clearInterval()` function
- [[2022-04-15 Friday]]
	- ```javascript
	  [...'Lydia'];
	  ```
	- this program will print `["L", "y", "d", "i", "a"]`
	- the spread operator maps every character of an iterable to one element
	- reference
	  collapsed:: true
		- [Spread syntax (...)](https://developer.mozilla.org/zh-TW/docs/Web/JavaScript/Reference/Operators/Spread_syntax) 
		  type:: document
		  tags:: JavaScript, [[Spread Operator]], Array, Object
		  title:: Spread syntax (...)
- [[2022-04-16 Saturday]] #[[Generator Function]]
  collapsed:: true
	- ```javascript
	  function* generator(i) {
	    yield i;
	    yield i * 2;
	  }
	  
	  const gen = generator(10);
	  
	  console.log(gen.next().value);
	  console.log(gen.next().value);
	  ```
	- this program will print `10` `20`
	- a generator function can be stopped mid-way, and using `yield`, the generator function yields the value behind it without returning a value
	- we can invoke the generator function by calling `next()` method
	- the first time we encounter `yield`, the function yields `10`
	- then we call `next()` again, the function encounters another `yield`, which yields `20`
	- reference
	  collapsed:: true
		- [function*](https://developer.mozilla.org/zh-TW/docs/Web/JavaScript/Reference/Statements/function*)
		  type:: document
		  tags:: JavaScript, [[Generator Function]] 
		  title:: function*
- [[2022-04-17 Sunday]] #Promise #setTimeout
  collapsed:: true
	- ```javascript
	  const firstPromise = new Promise((res, rej) => {
	    setTimeout(res, 500, 'one');
	  });
	  
	  const secondPromise = new Promise((res, rej) => {
	    setTimeout(res, 100, 'two');
	  });
	  
	  Promise.race([firstPromise, secondPromise]).then(res => console.log(res));
	  ```
	- this program will print `"two"`
	- `Promise.race()` will resolve or reject the first promise that resolve or reject
	- once the `setTimeout()` method expires, the `res` variable will hold the value that is also in the method argument
- [[2022-04-18 Monday]] #Object #Reference
  collapsed:: true
	- ```javascript
	  let person = { name: 'Lydia' };
	  const members = [person];
	  person = null;
	  
	  console.log(members);
	  ```
	- this program will print `[{name: 'Lydia'}]`
	- when we set `members` to an array with the first element as `person`, we essentially copy the reference to the object into the array
	- when we do `person = null`, we wipe out the reference, but the object is still there
	- so `console.log(members)` will still print the array with the object
	- reference
		- [JS基本觀念：call by value 還是reference 又或是 sharing?](https://medium.com/@mengchiang000/js%E5%9F%BA%E6%9C%AC%E8%A7%80%E5%BF%B5-call-by-value-%E9%82%84%E6%98%AFreference-%E5%8F%88%E6%88%96%E6%98%AF-sharing-22a87ca478fc) 
		  type:: article
		  tags:: JavaScript, Object, Reference
		  title:: JS基本觀念：call by value 還是reference 又或是 sharing?
		  id:: ffc2399d-644b-4999-aae4-8a6f494a5cbe
- [[2022-04-19 Tuesday]] #Object #Key
  collapsed:: true
	- ```javascript
	  const person = {
	    name: 'Lydia',
	    age: 21,
	  };
	  
	  for (const item in person) {
	    console.log(item);
	  }
	  ```
	- this program will print `"name", "age"`
	- the `for` loop will iterate through the object keys
	- object keys are strings
- [[2022-04-20 Wednesday]] #Type #[[Implicit Coercion]]
  collapsed:: true
	- ```javascript
	  console.log(3 + 4 + '5');
	  ```
	- this program will print `"75"`
	- the associativity of this expression is left-to-right
	- `7 + "5"` is evaluated to `"75"`, because `7` is converted into string, and `+` will concatenate two strings
		- [number plus string will result in a string](((62545721-fa64-48ae-a82f-2e836d740ebd)))
- [[2022-04-21 Thursday]] #Number #String
  collapsed:: true
	- ```javascript
	  const num = parseInt('7*6', 10);
	  ```
	- this program will produce `7`
	- `parseInt()` check if the string can be converted to a number, once it encounters an invalid character, it will stop parsing and ignore the rest of the string
	- the second argument `10` indicate that the base of the number should be 10
- [[2022-04-22 Friday]] #Map #Array #Type
  collapsed:: true
	- ```javascript
	  [1, 2, 3].map(num => {
	    if (typeof num === 'number') return;
	    return num * 2;
	  });
	  ```
	- this program will output `[undefined, undefined, undefined]`
	- in mapping method, `num` equals to the element in the array, so the `typeof num == 'number'` condition holds
	- mapping method will create a new array
	- when we don't return value from a function, the function returns `undefined`
- [[2022-04-23 Saturday]] #Object #[[Call By Sharing]]
  collapsed:: true
	- ```javascript
	  function getInfo(member, year) {
	    member.name = 'Lydia';
	    year = '1998';
	  }
	  
	  const person = { name: 'Sarah' };
	  const birthYear = '1997';
	  
	  getInfo(person, birthYear);
	  
	  console.log(person, birthYear);
	  ```
	- this program will print `{name: "Lydia"}, "1997"`
	- argument is called by value unless it is an object
	- objects are called by sharing
		- when we modify `member.name` in the function, the change will reflect to the object pointed by `person`
	- reference
		- {{embed ((ffc2399d-644b-4999-aae4-8a6f494a5cbe))}}
- [[2022-04-24 Sunday]] #Error
  collapsed:: true
	- function greeting() {
	    throw 'Hello world!';
	  }
	  
	  function sayHi() {
	    try {
	      const data = greeting();
	      console.log('It worked!', data);
	    } catch (e) {
	      console.log('Oh no an error:', e);
	    }
	  }
	  
	  sayHi();
	- this program will print `Oh no an error: Hello world!`
	- the `catch` statement can catch the exception thrown from the `try` block
	- `greeting()` will throw an error
- [[2022-04-25 Monday]] #Object #Constructor
  collapsed:: true
	- ```javascript
	  function Car() {
	    this.make = 'Lamborghini';
	    return { make: 'Maserati' };
	  }
	  
	  const myCar = new Car();
	  console.log(myCar.make);
	  ```
	- this program will print `"Maserati"`
	- if the constructor returns a value, then the value we get is the returned value
- [[2022-04-26 Tuesday]] #Object #Scope #Variable
  collapsed:: true
	- ```javascript
	  (() => {
	    let x = (y = 10);
	  })();
	  
	  console.log(typeof x);
	  console.log(typeof y);
	  ```
	- this program will print `"undefined", "number"`
	- `let x = (y = 10);` is actually `y = 10; let x = y;`
	- `y` is a property of the global object
	- variables declared with `let` are block scoped
		- `typeof x` will return `"undefined"` because `x` is not defined in the scope
	- `y` is accessible since it's a property of the global object
- [[2022-04-27 Wednesday]] #Object #Prototype
  collapsed:: true
	- ```javascript
	  class Dog {
	    constructor(name) {
	      this.name = name;
	    }
	  }
	  
	  Dog.prototype.bark = function() {
	    console.log(`Woof I am ${this.name}`);
	  };
	  
	  const pet = new Dog('Mara');
	  
	  pet.bark();
	  
	  delete Dog.prototype.bark;
	  
	  pet.bark();
	  ```
	- this program will print `"Woof I am Mara"`, `TypeError`
	- we can delete object's properties using the `delete` keyword
	- we will get `TypeError` if we try to invoke something that is not a function
- [[2022-04-28 Thursday]] #Set
  collapsed:: true
	- ```javascript
	  const set = new Set([1, 1, 2, 3, 4]);
	  
	  console.log(set);
	  ```
	- this program will print `{1, 2, 3, 4}`
- [[2022-04-29 Friday]] #Module
  collapsed:: true
	- ```javascript
	  // counter.js
	  let counter = 10;
	  export default counter;
	  ```
	- ```javascript
	  // index.js
	  import myCounter from './counter';
	  
	  myCounter += 1;
	  
	  console.log(myCounter);
	  ```
	- these program will print `Error`
	- imported modules are read-only
- [[2022-04-30 Saturday]] #Variable #[[Global Variable]]
  collapsed:: true
	- ```javascript
	  const name = 'Lydia';
	  age = 21;
	  
	  console.log(delete name);
	  console.log(delete age);
	  ```
	- this program will print `false`, `true`
	- the `delete` operation will return `true` if the deletion is successful, otherwise, it will return `false`
	- variable declared with `var`, `const` and `let` cannot be deleted using `delete`
		- variables declared by `var` are also added to the global object, but they cannot be deleted using `delete`
	- variables without declaration are added to the global object directly
-
-