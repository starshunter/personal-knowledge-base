- ((62517345-5339-4789-8ef6-d4b577b82528))
  collapsed:: true
	- instance variables are declared inside a class but not inside a method
	- local variables are declared inside a method, including method parameters
	- local variables live on stack, instance variables live inside class instance, which lives in the heap
		- an object only allocate the size of the reference variable for its instance variable, not the whole object
	- if a local variable of a method is an object reference, then that variable is on the stack, but the object it refers is in the heap
	- when we call a method, the stack frame of that method is pushed onto the stack
	- a method stays on the stack until it finishes execution
- a constructor has the code that runs when you instantiate an object
  collapsed:: true
	- every class has a constructor, even if we don't write it
		- the compiler will create a default constructor only if we don't write any constructor
	- can be used to initialize the state of the object
	- to have multiple constructor, they must have different argument lists
		- ((6251787a-c9ff-4070-9936-4bac7a49eead))
- ((62518009-5be0-4976-bc46-ccfce55389b4))
  collapsed:: true
	- all the constructors in an object's inheritance tree must run when you make a new object
	- abstract classes also have constructors
	- to call a superclass's constructor in its subclass, we can use `super()`
		- the compiler calls `super()` if we don't
	- the superclass constructor must finish before its subclass constructor
	- use `this()` to call a constructor from another overloaded constructor in the same class
		- `this()` must be the first statement in a constructor
		- a constructor cannot have both `super()` and `this()`
- an object's life depends entirely on the life of references referring to it
  collapsed:: true
	- a local variable lives only within the method that declared the variable
	- an instance variable lives as long as the object does
	- ((625183a6-21c0-417f-997f-d7c1c8791caa))
	- once the only reference variable disintegrated with the stack frame, the abandoned object becomes eligible for garbage collection
	- if we use the dot operator on a null reference, we'll get a `NullPointerException`