```Java
public class Person{
	private String firstName;
	private String lastName;
	private Address homeAddress;
	private MyDate dob;
	public String getFullName() {
		return firstName + " "+ lastName;
	}

	public Person(String firstName, String lastName, Address homeAddress, MyDate dob){
		this.firstName = firstName;
		this.lastName = lastName;
		this.homeAddress = homeAddress;
		this.dob = dob;
	}
}
```