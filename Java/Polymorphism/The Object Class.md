- Two commonly overridden methods can further demonstrate polymorphism,
	- toString()
	- [[equals()]]
- Both methods are originally defined in the class java.lang.Object

- **Everything in Java (except primitives) "is a" Object - LITERALLY**

```Java
public class Person{}
public class Person extends Object{}
```

- String class uses toString() method to allow any object to be added (concatenated) to a String.
![[equals() vs ==]]

```Java
MyDate javaRelease = new MyDate(3,18,2014);
String s = "Java SE 8 was released on " + javaRelease +".";
System.out.println(s); // Java SE 8 was released on 3/18/2014

```