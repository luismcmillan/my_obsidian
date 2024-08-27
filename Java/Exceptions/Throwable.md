- A Trowable in [[Java]] is an event that disrupts the normal flow of a programm.
	- When a problem occurs within a method, the method creates an object and hands it off to the runtime System
	- This is calles Throwable object
	- Its a class defined in java.lang
	- contains a **snapshot of the execution stack at the time it was created**
	- contains String that provides more information
	- In the case where on problem caused another which caused another and so on, **Throwable may contain another Throwable**

There are two general categories or , more precisely, two subclasses of Throwable objects:
- Error: Represents serious problems that an application should not try to recover from.
- **Exception are problems that an application might want to capture**
	- Runtime
	- Non-Runtime exception
		- can be handled via the standard try-catch block [[Catching Exceptions]]
		- OR ![[throws]]
- [[Creating Exception]]