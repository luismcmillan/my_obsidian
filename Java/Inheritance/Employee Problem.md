```Java
public class Employee extends Person{
	private MyDate hireDate;
	private int salary;
	public void promote(){
		salary *= 1 + (percent/100);
	}
	public Employee(String fName, String lName, Address add, MyDate date, MyDate hDate, in sal){
		firstName = fName; //Problem cause private
		lastName = lName; //Problem cause private
		homeAddress = add; //Problem cause private
		dob = date; //Problem cause private
		hireDate = hDate;
		salary = sal;
	}
}
```
Solution:
![[Employee Setters & getters]]