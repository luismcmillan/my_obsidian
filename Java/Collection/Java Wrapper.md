[[Collection]]
- Wrappers allow you to add primitives to collections
- Wrappers attach functionality to primitive data types
- To create a wrapper instance, pass the associated primitive into the constructor for the wrapper
```Java
List list = new ArrayList();
int j = 7;
list.add(Integer.valueOf(j));
```
- To get the primitive back out of the wrapper object, call the *type*Value()method.
```Java
Integer wrapInt = Integer.valueOf(7);
int j = wrapInt.intValue();
```
	- byte: Byte
	- short: Short
	- int: Integer
	- long: Long
	- float: Float
	- double: Double
	- char: Character
	- boolean: Boolean