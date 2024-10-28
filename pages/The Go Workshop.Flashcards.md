- What is the entry point of a go package? #card
  card-last-interval:: -1
  card-repeats:: 0
  card-ease-factor:: 2.5
  card-last-reviewed:: nil
  card-next-schedule:: nil
  card-last-score:: nil
  id:: 6207ba59-17e5-4796-8001-e038a4a2b093
	- Main function
- True of false? Every source code under same directory belongs to same package? #card
  card-last-interval:: -1
  card-repeats:: 0
  card-ease-factor:: 2.5
  card-last-reviewed:: nil
  card-next-schedule:: nil
  card-last-score:: nil
  id:: 6207ba59-d843-4e05-a7e6-395b90d45b56
	- True, and they should have same package name
- What is longest format to declare variable using `var`? #card
  id:: 6207ba59-a6f9-45fe-b2f7-2227426648cf
	- `var <name> <type> = <value>`
- How to declare multiple variable using `var` in one line? #card
  id:: 6207ba59-3142-4d07-950c-ead097160cde
	- `var <name_1>, <name_2>, <name_3> <type>`
	- `var <name_1>, <name_2>, <name_3> = <value_1>, <value_2>, <value_3>`
- What happen if you don't assign initial value when declaring a variable? (assuming the declaration is valid) #card
  id:: 6207ba59-6f7c-412a-96af-2336ba1114fe
	- Zero value depending on the type of variable will be assigned
- Where does go store variable in memory? What about pointer? #card
  id:: 6207ba59-24ac-44d0-8968-bd3cb1d8e1f8
	- Variable in go resides in stack, and pointer resides in heap
- Which service of go is responsible of detecting and recycling memory? #card
  id:: 6207ba59-4a9c-47af-bfa7-2149bdea6d4e
	- Garbage collection
- Name three ways to declare pointer in go #card
  id:: 6207ba59-f6a8-49a5-8bd7-ece82b7ab72a
	- `var <name> *<type>`
	- `var <name> = new(<type>)`
		- pointer declared by this method will point to zero value of that type
	- `<name_1> := &<name_2>`
- What are the constraints of constant in go? #card
  id:: 6207ba59-4cb9-4498-a36a-8af61e17bf17
	- Initial value must be provided when it's declared
	- the value of constant cannot be changed once declared
- When go compiler is searching a variable, what happen when it find a variable with same name but different type? #card
  id:: 6207ba59-8fbc-4e9f-9296-00f9c9cae9e4
	- Throw an error
- How can we use `if` statement in go to create a local variable for its condition? #card
  id:: 6207ba59-bb23-4a33-ba7e-ef0c7abe24ae
	- ```golang
	  if <init statement>; <boolean expression> {
	  	<code>
	  }
	  ```
- What is the syntax of `switch` in go? #card
  id:: 6207ba59-1183-4a53-ac28-f344476c9325
	- ```golang
	  switch <init statement>; <expression> {
	  case <expression>:
	  	<code>
	  case <expression>, <expression>:
	  	<code>
	      fallthrough
	  default:
	  	<code>
	  }
	  ```
- What is the purpose of `fallthrough` in go? #card
  id:: 6207ba59-fdb5-4b0c-a5ce-767695b2a7e3
	- It's used in 'switch' statement
	- It cannot be used in the final `case` of `default`
- What happen if we add `fallthrough` at the end of of `case` block? #card
  id:: 6207ba59-bf7b-442f-9b24-35bff427419b
	- It will transfer control of program to the first statement in the next `case`, skipping the expression
- What is the output of the following program? #card
  id:: 6207ba59-51bd-4bae-aee7-6f17b76d69a1
  ```golang
  package main
  
  import (
  	"fmt"
  )
  
  func main() {
  	switch 1 {
  	default:
  		fmt.Println("default")
  		fallthrough
  	case 1:
  		fmt.Println("I will print")
  		fallthrough
  
  	case 0:
  		fmt.Println("I will also print")
  	}
  }
  
  ```
	- ```bash
	  I will print
	  I will also print
	  ```
- How to replicate `while` in other language in go? #card
  id:: 6207ba59-74fc-4d96-9902-1740792be186
	- ```golang
	  for {
	  	<code>
	  }
	  ```
- How to iterate through container without calculating its length in go? #card
  id:: 6207ba59-28ac-476b-8ce4-248c50ab7212
	- ```golang
	  for <key>, <value> := range <set> {
	  	<code>
	  }
	  ```
- What is the zero values of various types of numbers in go? #card
  id:: 6207ba59-ca4f-42e0-bde3-0ac685feae2a
	- 0
- What is the size of `int` in go? #card
  id:: 6207ba59-a2f3-42a9-9e40-e107e0504803
	- Depending on what kind of machine, may be 4 bytes or 8 bytes, as well as `uint`
- True or false? We can assign a value of a `int64` variable to a `int` variable on a 64 bits machine? #card
  id:: 6207ba59-8a55-4041-8b02-1b912ca0cbd0
	- False, to protect inconsistent across different machine, compiler doesn't allow you to do that without conversion
- True or false? A variable of `int8` type can assign its value to another variable of type `int`? #card
  id:: 6207ba59-982e-4a54-a530-a5e57d158cea
	- False, you cannot do it directly without conversion, ie `int()`
- How many types are there in go to store floating-point number? #card
  id:: 6207ba59-5b8f-40cd-8946-667f584e9ea2
	- 2, `float32` and `float64`
- What does overflow in go mean? #card
  id:: 6207ba59-d463-44f0-8e10-2e8792ec413f
	- When a variable of numbers got assign to a value that exceeds its type's limit
- What does wraparound in go mean? #card
  id:: 6207ba59-5e7a-4131-ae0a-bc939dcc512c
	- When a variable of numbers exceed its type's limit, the value will reset to the type's maximum or minimum
- If we want to use big numbers in go, which package should we import? #card
  id:: 6207ba59-51f1-41f4-b58f-bd446eef5fa1
	- `math/big`
- What is the difference between raw and interpreted string literal? #card
  id:: 6207ba59-5308-490b-a984-46b246b0674d
	- Raw string literal will preserve the format of the string literal, whereas interpreted string literal will not. Also, interpreted string literal will transform special characters like `\n`, `\t` into newline and tab, but raw string literal won't
- What is type `rune` in go? #card
  id:: 6207ba59-5c03-4e72-ba1f-5bdac68526a6
	- It's a type that can store a UTF-8 character, regardless how many bytes that character may be
- What is the output of the following program? #card
  id:: 6207ba59-d582-452a-8b10-d140bcc08eae
  ```golang
  // You can edit this code!
  // Click here and start typing.
  package main
  
  import "fmt"
  
  func main() {
  	s := "你好嗎"
  	runes := []rune(s)
  	fmt.Println(len(s))
  	fmt.Println(len(runes))
  }
  
  ```
	- ```bash
	  9
	  3
	  ```
- What is the output of the following program? #card
  card-last-interval:: -1
  card-repeats:: 0
  card-ease-factor:: 2.5
  card-last-reviewed:: nil
  card-next-schedule:: nil
  card-last-score:: nil
  id:: 6207ba59-15b6-4573-b82d-c78404fa616b
  ```golang
  // You can edit this code!
  // Click here and start typing.
  package main
  
  import "fmt"
  
  func main() {
  	s := "你好嗎"
  	runes := []rune(s)
  	for i := 0; i < len(s); i++ {
  		fmt.Println(i, " ", string(s[i]))
  	}
  	for i := 0; i < len(runes); i++ {
  		fmt.Println(i, " ", string(runes[i]))
  	}
  	for i, v := range s {
  		fmt.Println(i, " ", string(v))
  	}
  	for i, v := range runes {
  		fmt.Println(i, " ", string(v))
  	}
  }
  
  ```
	- ```bash
	  0   ä
	  1   ½
	  2    
	  3   å
	  4   ¥
	  5   ½
	  6   å
	  7   
	  8   
	  0   你
	  1   好
	  2   嗎
	  0   你
	  3   好
	  6   嗎
	  0   你
	  1   好
	  2   嗎
	  ```
- Is the following line of code valid? #card
  id:: 6207ba59-5be3-48b1-ae34-8d7341ad008d
  `a := nil`
	- No, `nil` in go has no type, if we use short variable declaration to declare `a`, compiler won't be able to know what type is `a`
- How to initiate an array with initial value? #card
  id:: 6207ba59-0f22-4238-a8f7-32bfd24c08d7
	- `[...]<type>{<value_1>, <value_2>, ..., <value_n>}`
- What is the result of the line `a := [...]int{3: 3}` ? #card
  id:: 6207ba59-3e66-4c1e-aaa0-dc7f8656bf82
	- Create an array of length 4 with the forth element is 3 and assign it to `a`
- Under what circumstance can two arrays be compared in go? #card
  id:: 6207ba59-4d2f-4da0-859f-3390befc1b64
	- They have same length and same data type
- How to declare a new slice from an old slice in go? #card
  id:: 6207ba59-8d8c-42d1-a7da-cc2b6db52a3f
	- `<new slice> = <old slice>[:]`
	- `<new slice> = append(<empty slice>, <old slice>...)`
	- `copy(<new slice>, <old slice>)`
- What happen to a slice when appending a value that cause it to exceed its capacity? #card
  id:: 6207ba59-d588-4f79-9892-2de670286808
	- Go will allocate a new array, than copy old values into new array
- How to append multiple values into a slice in go? #card
  id:: 6207ba59-6e09-4581-b2c1-95839d772221
	- `append(<slice>, <value 1>, <value 2>, ..., <value n>)`
	- `append(<slice>, <another slice>...)`
- What is the output of the following program? #card
  id:: 6207ba59-ccce-40d8-8b21-41a453a30d3a
  ```golang
  // You can edit this code!
  // Click here and start typing.
  package main
  
  import "fmt"
  
  func main() {
  	a := [5]int{1, 2, 3, 4, 5}
  	b := a[1:3]
  	c := a[1:3]
  	b = append(b, 6)
  	fmt.Println(cap(b), a, b, c)
  }
  
  ```
	- ```bash
	  4 [1 2 3 6 5] [2 3 6] [2 3]
	  ```
- How to declare a map with initial values in go? #card
  id:: 6207ba59-dd78-4561-b915-dd86cd3695eb
	- `map[<key type>]<value type>{<key 1>: <value 1>, <key 2>: <value 2>, ..., <key n>: <value n>}`
- What is the output of the following program? #card
  id:: 6207ba59-2d3c-44ff-82de-201dad1219ac
  ```golang
  // You can edit this code!
  // Click here and start typing.
  package main
  
  import "fmt"
  
  func main() {
  	var a map[int]int
  	b := make(map[int]int, 10)
  	fmt.Println(a == nil, b == nil)
  }
  
  ```
	- ```bash
	  true false
	  ```
- How to delete a key from map in go? #card
  id:: 6207ba59-1db0-4e3a-be04-bc0488f6e15d
	- `delete(<name>, <key)`
- How to check if a key exist in map? #card
  id:: 6207ba59-5794-4671-8b23-56bb20f6b37e
	- `<value>, <exist> := <name>[key]`
- What is the output of the following program? #card
  id:: 6207ba59-c635-4da2-9f1c-15b203237e17
  ```golang
  // You can edit this code!
  // Click here and start typing.
  package main
  
  import "fmt"
  
  func main() {
  	a := map[int]int{1: 10, 2: 20}
  	b := a
  	b[1] = 3
  	fmt.Println(a)
  }
  
  ```
	- ```bash
	  map[1:3 2:20]
	  ```
- How to create custom type in go? #card
  id:: 6207ba59-1806-4f6b-8e1d-c137f19abce8
	- `type <custom name> <core types>`
- What is the output of the following program? #card
  id:: 6207ba59-cbc5-429e-84ed-3105e5111a55
  ```golang
  // You can edit this code!
  // Click here and start typing.
  package main
  
  import "fmt"
  
  type t int
  
  func main() {
  	var a t = 1
  	var b int = 1
  	fmt.Println(a, b, a == b)
  }
  
  ```
	- compilation error
- How to use anonymous struct in go? #card
  id:: 6207ba59-1f42-4b5f-8bec-e555febf9a5a
	- ```golang
	  <variable> := struct {
	  	<field 1> <type>
	      <field 2> <type>
	      ...
	      <field n> <type>
	  } {
	  	<value 1>,
	      <value 2>,
	      ...
	      <value n>
	  }
	  ```
- If there is a struct type `Person` in your program, how do you declare a variable of that type? #card
  id:: 6207ba59-fc3d-40be-8049-c4bbbe681221
	- ```golang
	  a := Person{
	  	<field 1>: <value 1>,
	      <field 2>: <value 2>,
	      ...
	      <field n>: <value n>
	  }
	  ```
- Under what circumstance can a struct type be comparable? #card
  id:: 6207ba59-650d-4845-9584-c9b2bf3e6cda
	- Every field's type has to be comparable and their name have to be the same
- What is the difference between having a struct field with type of another struct, and embedding another struct into current struct? #card
  id:: 6207ba59-d92d-4e44-8275-f938927dbd10
	- The embedded struct's fields will be promoted, we can access them by `<embedding struct>.<promoted field>`
- How to embed a struct in go? #card
  id:: 6207ba59-0846-4081-8975-20ddffd3a312
	- ```golang
	  type <name> struct {
	  	<field> <type>
	      <struct type>
	  }
	  ```
- How to initiate a struct with an embedding struct? #card
  id:: 6207ba59-ea6f-47fa-b508-2033359d93bf
	- ```golang
	  <variable> := <embedding struct> {
	  	<embedded struct>: <embedded struct> {
	      	<field>: <value>
	      }
	  }
	  ```
	- `<embedding struct>.<embedded struct>.<embedded field>`
- Suppose there is a custom type struct `Person` in your program, how do you add a method `getName` to this type? #card
  id:: 6207ba59-fa0d-4953-8056-5c6ac2fdcc52
	- ```golang
	  func (p Person) getName() {
	  	<code>
	  }
	  ```
- What will happen in the following program? #card
  id:: 6207ba59-cead-4907-a945-44df98ac5652
  ```golang
  // You can edit this code!
  // Click here and start typing.
  package main
  
  import "fmt"
  
  type T struct {
  	x int
  }
  
  func (t *T) setX(x int) {
  	t.x = x
  }
  
  func (t T) getX() int {
  	return t.x
  }
  
  func main() {
  	var t T
  	t.setX(5)
  	fmt.Println(t.getX())
  }
  ```
	- ```bash
	  5
	  ```
- Does go have implicit type conversion? #card
  id:: 6207ba59-27e8-4216-bc92-c84dba0c89db
	- No
- Why do we need type assertion? #card
  id:: 6207ba59-be9c-4a40-8337-fdef45ac71e2
	- We can use type assertion to check if a value is `nil`, if it can convert to the type we require and to convert it to the type we require if possible. Generally occurs at situation where we use interface to store values of different types
- What is the syntax of type assertion in go? #card
  id:: 6207ba59-ff8c-49bf-9200-973b4bdbf0e7
	- `<value>, <ok> := <variable>.(<type>)`
- How to use type switch in go? #card
  id:: 6207ba59-debe-476c-9f9b-5672673ae88e
	- ```golang
	  switch <value> := <variable>.(type) {
	  case <type>:
	  	<code>
	  case <type>, <type>:
	  	<code>
	  default:
	  	<code>
	  }
	  ```
	- `fallthrough` is not available in type switch
- What is the syntax of declaring a function in go? #card
  id:: 6207ba59-0f28-4520-8b4a-29dff916d0e2
	- ```golang
	  func f(<param 1> <type 1>, <param 2> <type 2>, ...) <return type> {
	  
	  }
	  ```
- What does naked return in go mean? #card
  id:: 6207ba59-c9bc-4dcc-bcfd-32ee058ce343
	- Naked return means there's nothing being return after the `return` keyword, and this is possible only when return values' name are specific
- What is the syntax of variadic function in go? #card
  id:: 6207ba59-70b1-4802-8242-96f776ca5c5a
	- `func <name>(<param> ...<type>)`
- How can we access the values we pass into variadic function? #card
  id:: 6207ba59-2a77-4b75-8b4a-aee93f1a7f20
	- Those values will be put into a slice, so we can access them using slice syntax
- How can we pass a slice into variadic function? #card
  id:: 6207ba59-1d3d-47b1-8517-d0c47e935d98
	- Use unpack operator `...` after the variable
- What is the syntax of anonymous function? #card
  id:: 6207ba59-b6e6-460d-9f8a-31f83db890b6
	- ```golang
	  func(<param> <type>) {
	  	
	  }(<arg>)
	  ```
- Explain what is closure? #card
  id:: 6207ba59-3b10-4d27-a5fc-5e6a8617467e
	- A closure is a function value that references variables from outside its body. The function may access and assign to the referenced variables, and it is the variable itself that being captured, not its value
- What is the required conditions to pass function as argument into another function? #card
  id:: 6207ba59-f656-45df-b077-b972929b40c2
	- The signature of the function being passed need to match the function signature specify in the function
- What happen when we add `defer` to the beginning of a function? #card
  id:: 6207ba59-2df4-4900-a505-dcc7b25a2024
	- We create a deferred function, that function will only be executed after current function return
- When do the parameters of a deferred function evaluate? #card
  id:: 6207ba59-bdeb-4d26-ae00-20bc63e5639d
	- They are evaluated when the function is deferred
- What is the output of the following program? #card
  id:: 6207ba59-48ae-4ff0-a64e-7eb6dd872794
  ```golang
    package main
    
    import (
    	"errors"
    	"fmt"
    )
    
    func useAClosure() error {
    	var err error
    	defer func() {
    		fmt.Printf("useAClosure: err has value %v\n", err)
    	}()
    
    	err = errors.New("Error 1")
    	fmt.Println("Finish func useAClosure")
    
    	return err
    }
    
    func deferPrintf() error {
    	var err error
        //呼叫的時候會把參數帶過去，所以err是nil
    	defer fmt.Printf("deferPrintf: err has value %v\n", err)
    
    	err = errors.New("Error 2")
    
        //注意這裡是LIFO，所以呼叫會是43210
    	for i := 0; i < 5; i++ {
    		defer fmt.Printf("%d ", i)
    	}
    	fmt.Println("Finish func deferPrintf")
    	return err
    }
    
    func main() {
    	useAClosure()
    	deferPrintf()
    }
  ```
	- ```bash
	  Finish func useAClosure
	  useAClosure: err has value Error 1
	  Finish func deferPrintf
	  4 3 2 1 0 deferPrintf: err has value 
	  ```
- What are three types of error in go? #card
  id:: 6207ba59-2ff5-4e94-b33b-07f09d5a4598
	- syntax error
	- runtime error
	- logic error
- How can we implement the error interface? #card
  id:: 6207ba59-8989-413c-9abf-2fef19bd83a0
	- Implement a method called `Error()` with return type string on a struct
- How can we define our own error value? #card
  id:: 6207ba59-5178-49a0-bcfd-1bcfbd65d2f6
	- use `errors.New()`
	- use `fmt.Errorf()` when we want to return an error value
- How can wrap an error into another error and pass it to upper function? #card
  id:: 6207ba59-02f9-4c85-8025-0ec0d2ea52a2
	- Use `fmt.Errorf("%w", <wrapped error>)` when returning an error
- What is the difference between error and panic? #card
  id:: 6207ba59-2a5f-484b-ad47-8682ae94d17c
	- Error may cause unexpected behavior but won't stop the program unless we explicitly tell the program to. Panic, on the other hand, will cause the program to crash if we don't handle it
- What should pass into `panic()`? #card
  id:: 6207ba59-58a8-458d-9d24-ce40c8f09abc
	- An error value
- What happen after a panic occur? #card
  id:: 6207ba59-a704-4d4f-b580-1d02fb92befe
	- program stop
	- if the function which panic occurs in has deferred functions, those functions will be called
	- panic pass to upper function and repeat last step until we reach `main()`
	- statements after `panic()` won't execute
	- program crash
- Why do we need `recover()`? #card
  id:: 6207ba59-49b7-435c-be1e-0e633d88ad88
	- To that program resume execution after a panic occur
- Where should we place `recover()`? #card
  id:: 6207ba59-82d6-4465-9f6a-f52aa65ae604
	- Inside a deferred function which resides in a function that a panic may occur
- How do we define a new interface in go? #card
  id:: 6207ba59-b858-4249-8cc0-ee0ede14640e
	- ```golang
	  type <name> interface {
	  	<method 1 signature>
	      <method 2 signature>
	  }
	  ```
- What does duck typing mean? #card
  id:: 6207ba59-3c2a-49c7-8be5-17be3ca35bcf
	- Implementation in go is implicit, doesn't require any keyword, just need to bind all the methods specified by interface
- What is interface in go? #card
  id:: 6207ba59-e472-4184-b0c2-5f3265029877
	- An interface is defined as a set of function signatures, if a type define this set of methods, than that type implements that interface, and can be treated like that interface as well
- Can a package contains multiple files? #card
  id:: 6207ba59-f924-4d9e-8db8-1d7243c73d2c
	- Yes, those files should reside in same directory, and their package name should also be the same
- Who can access unexported variables? #card
  id:: 6207ba59-50c7-4baf-a529-3d86c9bdcc21
	- Files belong to the same package
- How to export a function in go? #card
  id:: 6207ba59-cf19-4afe-b1c8-849d2583d88e
	- Change the first letter of the function name to uppercase
- Using `go get` to download package, where does the package reside on the computer? #card
  id:: 6207ba59-f51f-4364-a598-20e676089f6a
	- In `GOPATH/pkg/mod`
- How to assign an alias name to a imported package? #card
  id:: 6207ba59-42aa-4524-889b-99a625a69a84
	- `import <alias> <package>`
- What is the use of `init()` in go? #card
  id:: 6207ba59-b69c-457f-8306-c0944d0632c4
	- It executed before `main()`, and is used to initialize package state and global variables
- How many `init()` is allowed in one package? #card
  id:: 6207ba59-f55b-40f3-8df0-2adf2586495d
	- There can be multiple `init()` in a package
- Between outer package `init()` and package `init()`, which one get execute first? #card
  id:: 6207ba59-8ccf-4ec4-9a12-6f02de4a5743
	- Outer package's `init()` get execute first
- How to create a custom logger in go? #card
  card-last-interval:: -1
  card-repeats:: 0
  card-ease-factor:: 2.5
  card-last-reviewed:: nil
  card-next-schedule:: nil
  card-last-score:: nil
  id:: 6207ba59-fde5-4d12-9667-763e76770d69
	- `<logger> := log.New(<io.Writer interface>, <prefix>, <flags>)`
- What is the naming convention of testing file in go? #card
  id:: 6207ba59-0ab8-4b7d-a5da-01d109448bc1
	- add `_test` at the end of the file name
- How do you decode a JSON string into go's data structure? #card
  id:: 6207ba59-5651-4645-93c5-64fad7b6eced
	- Use `Unmarshal()`. First define a struct type that can take the values from JSON data, which need to have exportable fields, then pass a pointer of that datatype into `Unmarshal(data []byte, v interface{})`, also remember to convert JSON string into byte slice first
- What is the use of JSON tag? #card
  id:: 6207ba59-82a6-4e03-9fa7-c344bd8e4062
	- It help `Unmarshal()` to identify which field to decode JSON value into
- How do you encode struct into JSON? #card
  id:: 6207ba59-09ef-422b-b8b9-c351f22a0599
	- Use `Marshal()`. If there are multiple fields in the struct, than only fields with JSON tag can be encoded
- What happen to struct fields with no value while encoding it into JSON? #card
  id:: 6207ba59-8d09-46d5-a7b8-c57d4dafb95c
	- They will be filled with zero value of the fields' type
- How to ignore field when encoding a struct into JSON? #card
  id:: 6207ba59-31d3-407c-9255-1161fc7e96cb
	- Use JSON tag `json:"-"` or use `omitempty` if you want to ignore fields with no value
- What is the difference between `Unmarshal()/Marshal()` and `newDecoder()/newEncoder()`? #card
  id:: 6207ba59-41c7-4039-87f6-573057a8e5a1
	- `newDecoder()/newEncoder()` will create decoder/encoder like `Unmarshal/Marshal`, but these decoder/encoder can decode/encode from/to the source of our choice
- Why would we use `map[string]interface{}` to decode/encode JSON data? #card
  id:: 6207ba59-ae6b-424b-9a8a-ad6777e2cb7a
	- Because sometimes the values of JSON data can be unknown or change frequently, so it's unrealistic to use struct in these cases
- How to define our own flag in go? #card
  id:: 6207ba59-7faa-4efb-a3ee-ec16a476f72b
	- Use `flag` package
	  `<flag> := flag.<type>(<flag name>, <default value>, <usage string>)`
- What happen to deferred functions when the program receives a interrupt or terminate signal? #card
  id:: 6207ba59-7942-4736-8e83-93bd8f8eea5b
	- Those deferred functions will not be executed
- How to make sure our program will terminated correctly after receiving a terminate signal? #card
  id:: 6207ba59-dcb5-4bde-8bfb-d4026c045380
	- Use `signal.Notify()` to pass the signal into a channel, than retrieve that signal from the channel and determine how the program should react
- What does this `-rwxr-xr-x` file permission mean? #card
  id:: 6207ba59-e790-46b4-84ce-22c110ad3e30
	- It means owner can read, write and execute this file, while other groups and users can only read and execute this file
-