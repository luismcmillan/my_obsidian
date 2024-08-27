[[Inheritance]]
- The call of the super constructor is always the first call (either explicitly or implicitly) in an extending class's constructor
```Java
//Constructors
public Employee(String fName, String lName, Address add, MyDate date, MyDate hireDate, int salary){
		super(fname, lName, add, date)
		this.hireDate = hireDate;
		this.salary = salary;
		...
	}
```