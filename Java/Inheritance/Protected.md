- [[Inheritance]]
- [[Access Modifier]]
- Protected access means that the state or behavior is available to code in the same class, same package and to subtypes in any other package

```Java
package example.here;
public class Person {
	protected void doSomething(){
		System.out.println("Doing something"); 
	}
}
```

```Java
package example.here;
puvlic class PersonTester {
	public static void main(String[] args){
		Person p = new Person();
		p.doSomething(); //LEGAL because it is being invoked from a class in the same package
	}
}
```

```Java
package example.else;
puvlic class Employee extends Person {
	public void testingProtectedMethod(){
		doSomething(); // LEGAL because Employee extends Person
	}
}
```

```Java
package example.else;
puvlic class EmployeeTester {
	public static void main(String[] args){
		Employee e = new Employee();
		e.doSomething() //ILLEGAL because different package and not a subtype of Person
	}
}
```

```Java
package example.else;
import example.here.Person;
import example.here.Musician;
puvlic class Employee extends Person {

	public void testingProtectedMethod(){
		doSomething(); //LEGAL
	}
	
	public static void main(String[] args){
		Employee e = new Employee();
		e.doSomething() //LEGAL
		Person p = new Person();
		p.doStomething(); //ILLEGAL
		Musician m = new Musician();
		m.doSomething(); //ILLEGAL
	}
}
```