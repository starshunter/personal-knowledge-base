- there are many ways to save the state of Java program
	- use serialization
	  collapsed:: true
		- the data will be used only by Java program that generates it
		- make a file and output stream, then write the desired objects into the file through stream
		- ((6256dd45-739d-45cb-b25f-5006b6c06dd5))
		- ((6256dd70-163b-444f-8007-d4c603aab6fb))
		  collapsed:: true
			- the object's instance variables are saved into the file, along with some additional information, sot that JVM can reconstruct the exact object from the file
		- similar procedures for deserialization
			- ((6256e269-9efe-44a0-8f48-de5075581eae))
		- when an object is serialized, all the objects it refers to from instance variables are also serialized
		  collapsed:: true
			- serialization saves the entire object graph
		- if we want our class to be serializable, we need to implement `Serializable` interface
			- the interface has no method, it just serves as a marker
			- if the superclass is serializable, then its every subclass is serializable
		- either the entire object graph is serialized correctly or serialization fails
		- mark the instance variable as transient if it can't be saved
		- in deserialization, if there's a non-serializable class in the inheritance tree, the constructor for that non-serializable class will run, as well as any constructors above that class
	- write a plain text file
	  collapsed:: true
		- the data will be used by other programs
		- create a file write and write string to that file directly
		- a file object represents the name and path of a file or directly on the disk
		- use buffer to avoid accessing the disk every time we write a string
			- the buffer will wait until it's full, then it will write its contents into the file
		- the same procedures can apply to reading strings from a file
- a serialized object is stamped with a version ID number for the object's class
  collapsed:: true
	- the class could have a different version ID if the class is changed
	- we can manually set the version ID in the class, so that even we change the class, JVM will still allow us to deserialize the object
		- we have to take the responsibility to ensure the serialized object can be correctly deserialized into the new class