- Composition
```Java
public class Employee {
	private String firstName;
	private String lastName;
	private Address homeAddress;
	private MyDate dob;
	public String getFullName() {
		return firstName + " "+ lastName;
	}

	private MyDate hireDate;
	private int salary;
	public void promote(){
		salary *= 1 + (percent/100);
	}
}
```
- [[Inheritance]]   (with [[Person]]):
```Java
public class Employee extends Person{
	private MyDate hireDate;
	private int salary;
	public void promote(){
		salary *= 1 + (percent/100);
	}
}
```
