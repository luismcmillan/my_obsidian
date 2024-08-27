- [[Protected]]
- [[Overloading Methods]]
- [[Overriding Methods]]
- [[Final]]
- When you extend another class, you inherit all the attributes and behaviors of the super class.
- **each class can only extend one class**
	- but the class you extend might have already extended another class.
![[Person]]

[[Employee]]
```Java
Employee e = new Employee();
e.promote(); //promote is defined in Employee
String name = e.getFullName(); //getFullname is available via Person
```

![[super constructor]]

![[Chaining Constructors]]

![[Employee Problem]]