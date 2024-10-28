title:: JavaScript Questions/2022-03

- [[2022-03-05 Saturday]] #Hoist #Scope
  collapsed:: true
	- ```javascript
	  function sayHi() {
	      console.log(name);
	      console.log(age);
	      var name = 'Lydia';
	      let age = 21;
	  }
	  
	  sayHi();
	  ```
	- this would print `undefined` and `ReferenceError`
	- both variable declared with `var` and `let` will get hoisted, but only `var` will set the initialize value to `undefined`
	- the start of the scope to the line where `let` assigns value to its variable, this area is called temporal dead zone, any line tries to access this variable will get a `ReferenceError`
- [[2022-03-06 Sunday]] #Scope
  collapsed:: true
	- ```javascript
	  for (var i = 0; i < 3; i++) {
	    setTimeout(() => console.log(i), 1);
	  }
	  
	  for (let i = 0; i < 3; i++) {
	    setTimeout(() => console.log(i), 1);
	  }
	  ```
	- the program will print `3 3 3` and `0 1 2`
	- the callback function in `setTimeout` will be executed after the loop
	- variable declared by `var` is global, declared by `let` is block-scoped
- [[2022-03-07 Monday]] #this #[[Arrow Function]]
  collapsed:: true
	- ```javascript
	  const shape = {
	    radius: 10,
	    diameter() {
	      return this.radius * 2;
	    },
	    perimeter: () => 2 * Math.PI * this.radius,
	  };
	  
	  console.log(shape.diameter());
	  console.log(shape.perimeter());
	  ```
	- the program will print `20` and `NaN`
	- because in normal function, `this` will refer to the object that is calling the function
	- but for arrow function, `this` will refer to its current surrounding scope
	- references
	  collapsed:: true
		- [Arrow function 解決了什麼問題？](https://askie.today/this-arrow-function-in-javascript/)
			- type:: article
			  tags:: JavaScript, [[Arrow Function]] 
			  title:: Arrow function 解決了什麼問題？
- [[2022-03-08 Tuesday]] #[[Logical Operation]]
  collapsed:: true
	- ```javascript
	  +true;
	  !'Lydia';
	  ```
	- the program will print `1` and `false`
	- the unary plus will try to convert an operand into a number, and `true` equal to 1
	- `'Lydia'` is a truthy value, and Logical NOT means asking is the value false
- [[2022-03-09 Wednesday]]
  collapsed:: true
	- ```javascript
	  const bird = {
	    size: 'small',
	  };
	  
	  const mouse = {
	    name: 'Mickey',
	    small: true,
	  };
	  ```
	- `mouse.bird.size` is not valid
		- `mouse[bird.size]` and `mouse[bird["size"]]` are both valid
	- javascript will first interpret the statement inside `[]`
	- with dot notation, javascript interpret from the left
		- since `mouse` doesn't have property `bird`, the whole statement will return an error
- [[2022-03-10 Thursday]] #Object #Copy
  collapsed:: true
	- ```javascript
	  let c = { greeting: 'Hey!' };
	  let d;
	  
	  d = c;
	  c.greeting = 'Hello';
	  console.log(d.greeting);
	  ```
	- this program will print `Hello`
	- object is assigned by reference in javascript
	- `Object.assign({}, obj)` can achieve a fake deep copy
		- fail when the object contains another object
		- use package to achieve deep copy
- [[2022-03-11 Friday]] #Object #Equality
  collapsed:: true
	- ```javascript
	  let a = 3;
	  let b = new Number(3);
	  let c = 3;
	  
	  console.log(a == b);
	  console.log(a === b);
	  console.log(b === c);
	  ```
	- the program will print `true` `false` `false`
	- `new Number()` will create a new wrapped object
	- so `b` is a number object with value 3
	- `==` will compare two variable's value, while `===` will compare value and type
- [[2022-03-12 Saturday]] #Class #Constructor #Static
  collapsed:: true
	- ```javascript
	  - class Chameleon {
	    static colorChange(newColor) {
	    this.newColor = newColor;
	    return this.newColor;
	    }
	      
	    constructor({ newColor = 'green' } = {}) {
	    this.newColor = newColor;
	    }
	    }
	      
	    const freddie = new Chameleon({ newColor: 'purple' });
	    console.log(freddie.colorChange('orange'));
	  ```
	- this program will print `TypeError`
	- static method cannot be called with class instance
		- only can be called with class name
	- references
	  collapsed:: true
		- [static](https://developer.mozilla.org/zh-TW/docs/Web/JavaScript/Reference/Classes/static)
		- [Default value of argument in ES6](https://stackoverflow.com/questions/44491229/default-value-of-argument-in-es6)
		  collapsed:: true
			- type:: article
			  tags:: JavaScript, [[Default Value of Parameters]], [[Destructuring Assignment]]
			  title:: Default value of argument in ES6
- [[2022-03-13 Sunday]] #[[Global Variable]]
  collapsed:: true
	- ```javascript
	  let greeting;
	  greetign = {}; // Typo!
	  console.log(greetign);
	  ```
	- this program will print an empty object
	- javascript interpreter will see `greetign` as `global.greetign`
	- use `use strict` to avoid assigning a variable before declaring it
	- assign an undeclared variable will create a global variable, just like using `var`
- [[2022-03-14 Monday]] #Function
  collapsed:: true
	- ```javascript
	  function bark() {
	    console.log('Woof!');
	  }
	  
	  bark.animal = 'dog';
	  ```
	- this program will not produce any error
	- in javascript, function is a special kind of object
	- so we can add properties to an object without any problem
- [[2022-03-15 Tuesday]]
  collapsed:: true
	- ```javascript
	  function Person(firstName, lastName) {
	    this.firstName = firstName;
	    this.lastName = lastName;
	  }
	  
	  const member = new Person('Lydia', 'Hallie');
	  Person.getFullName = function() {
	    return `${this.firstName} ${this.lastName}`;
	  };
	  
	  console.log(member.getFullName());
	  ```
	- this program will produce `TypeError`
	- functions in javascript are objects, so the function was added to the constructor function object
	- we can access `getFullName` through `Person`, but not any of its instance
	- to allow its instance to access a function, we should add the function to `Person.prototype`
- [[2022-03-16 Wednesday]] #Function #Object
  collapsed:: true
	- ```javascript
	  function Person(firstName, lastName) {
	    this.firstName = firstName;
	    this.lastName = lastName;
	  }
	  
	  const lydia = new Person('Lydia', 'Hallie');
	  const sarah = Person('Sarah', 'Smith');
	  
	  console.log(lydia);
	  console.log(sarah);
	  ```
	- this program will print `Person {firstName: "Lydia", lastName: "Hallie"}` and `undefined`
	- if we don't use `new` to create an object, `this` will refer to global object
	- since we don't return any value in `Person`, `sarah` will remain undefined
- [[2022-03-17 Thursday]] #Bubbling #Capturing
  collapsed:: true
	- What are the three phases of event propagation?
		- A: Target > Capturing > Bubbling
		- B: Bubbling > Target > Capturing
		- C: Target > Bubbling > Capturing
		- D: Capturing > Target > Bubbling
	- the answer is D
	- reference
	  id:: 624219a2-5583-4ae6-b2b1-56e2451e7068
		- [DOM 的事件傳遞機制：捕獲與冒泡](https://blog.techbridge.cc/2017/07/15/javascript-event-propagation/)
			- type:: article
			  tags:: Bubbling, Capturing, Event, JavaScript
			  title:: DOM 的事件傳遞機制：捕獲與冒泡
- [[2022-03-18 Friday]] #Prototype #Object
  collapsed:: true
	- All object in javascript have prototypes
		- false
	- the base object doesn't have prototypes
- [[2022-03-19 Saturday]] #Type #[[Implicit Coercion]]
  id:: 62545721-fa64-48ae-a82f-2e836d740ebd
  collapsed:: true
	- ```javascript
	  function sum(a, b) {
	    return a + b;
	  }
	  
	  sum(1, '2');
	  ```
	- this program will print `"12"`
	- javascript is dynamically typed
	- values can be converted to another type
		- implicit coercion
	- in an addition of a number and a string, the number will be converted into a string
	- reference
		- [Implicit Coercion in JavaScript](https://medium.com/front-end-weekly/implicit-coercion-in-javascript-5077ad5510d)
		  collapsed:: true
			- type:: article
			  tags:: JavaScript, [[Implicit Coercion]] 
			  title:: Implicit Coercion in JavaScript
- [[2022-03-20 Sunday]]
  collapsed:: true
	- ```javascript
	  let number = 0;
	  console.log(number++);
	  console.log(++number);
	  console.log(number);
	  ```
	- this program will print `0 2 2`
	- postfix operation will return the old value
	- prefix operation will return incremented value
- [[2022-03-22 Tuesday]] #Object #Reference
  collapsed:: true
	- ```javascript
	  function checkAge(data) {
	    if (data === { age: 18 }) {
	      console.log('You are an adult!');
	    } else if (data == { age: 18 }) {
	      console.log('You are still an adult.');
	    } else {
	      console.log(`Hmm.. You don't have an age I guess`);
	    }
	  }
	  
	  checkAge({ age: 18 });
	  ```
	- this program will print `Hmm.. You don't have an age I guess`
	- objects are compared by their reference in javascript
- [[2022-03-23 Wednesday]] #[[Rest Parameter]]
  collapsed:: true
	- ```javascript
	  function getAge(...args) {
	    console.log(typeof args);
	  }
	  
	  getAge(21);
	  ```
	- this program will print `object`
	- `...args` will collect all remaining arguments into an array
		- [其餘參數](https://developer.mozilla.org/zh-TW/docs/Web/JavaScript/Reference/Functions/rest_parameters)
	- an array is an object
- [[2022-03-24 Thursday]] #[[Strict Mode]]
  collapsed:: true
	- ```javascript
	  function getAge() {
	    'use strict';
	    age = 21;
	    console.log(age);
	  }
	  
	  getAge();
	  ```
	- this program will print `ReferenceError`
	- in strict mode, we won't accidentally create a global variable
	- when we assign value to `age`, since we didn't declare it and we are in strict mode, it will throw a `ReferenceError`
	- if we don't use strict mode, `age` will be added to global object
- [[2022-03-25 Friday]]
  collapsed:: true
	- ```javascript
	  const sum = eval('10*10+5');
	  ```
	- the value of `sum` is `105`
	- `eval()` evaluate the string that passed to it
	- the string is evaluated
- [[2022-03-26 Saturday]] #[[Local Storage]] #[[Session Storage]]
  collapsed:: true
	- ```javascript
	  sessionStorage.setItem('cool_secret', 123);
	  ```
	- `cool_secret` will not be accessible if the user close the tab
	- in contract, item in `localStorage` will be accessible forever, unless `localStorage.clear()` is called
	- reference
	  collapsed:: true
		- [[JavaScript] Cookie、LocalStorage、SessionStorage 差異](https://medium.com/@bebebobohaha/cookie-localstorage-sessionstorage-%E5%B7%AE%E7%95%B0-9e1d5df3dd7f)
			- type:: article
			  tags:: Cookie, [[Local Storage]], [[Session Storage]] 
			  title:: [JavaScript] Cookie、LocalStorage、SessionStorage 差異
- [[2022-03-27 Sunday]]
  collapsed:: true
	- ```javascript
	  var num = 8;
	  var num = 10;
	  
	  console.log(num);
	  ```
	- this program will print `10`
	- we can declare multiple variables with same name using `var`
	- but we cannot do this with `let` and `const`
- [[2022-03-28 Monday]] #Object #Property
  collapsed:: true
	- ```javascript
	  const obj = { 1: 'a', 2: 'b', 3: 'c' };
	  const set = new Set([1, 2, 3, 4, 5]);
	  
	  obj.hasOwnProperty('1');
	  obj.hasOwnProperty(1);
	  set.has('1');
	  set.has(1);
	  ```
	- this program will print `true` `true` `false` `true`
	- all object keys are string
	- `set` doesn't have `'1'`
- [[2022-03-29 Tuesday]] #Object
  collapsed:: true
	- ```javascript
	  const obj = { a: 'one', b: 'two', a: 'three' };
	  console.log(obj);
	  ```
	- this program will print `{ a: 'three', b: 'two' }`
	- a key's value will be replaced if there is another same key
	- the order of the key will remain the same
- [[2022-03-30 Wednesday]]
  collapsed:: true
	- ```javascript
	  for (let i = 1; i < 5; i++) {
	    if (i === 3) continue;
	    console.log(i);
	  }
	  ```
	- this program will print `1 2 4`
	- normal programming concept
- [[2022-03-31 Thursday]] #Prototype #Object #String
  collapsed:: true
	- ```javascript
	  String.prototype.giveLydiaPizza = () => {
	    return 'Just give Lydia pizza already!';
	  };
	  
	  const name = 'Lydia';
	  
	  name.giveLydiaPizza();
	  ```
	- this program will print `"Just give Lydia pizza already!"`
	- `String` is a built in constructor
	- string literal is automatically converted to string object
	- so `name` can access the method we add