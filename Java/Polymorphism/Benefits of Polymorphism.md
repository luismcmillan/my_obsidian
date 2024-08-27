[[Polymorphism]]
```Java
public class Employee extends Person {
	public double pay() {
		return 0;
	}
}

public class Manager extends Employee {
	private double salary = 75000.00;
	private double bonus = 10000.00;
	public double pay(){
		return (salary/24) +(bonus/24);
	}
}

public class Instructor extends Employee {
	private double perPayClass = 1000.00;
	private int classes = 2;
	public double pay(){
		return (payPerClass * classes);
	}
}

public class Programmer extends Employee {
	private int linesOfCode = 1000;;
	private int perPerLineOfCode = 3.00;
	public double pay(){
		return (linesOfCode * payPerLineOfCode);
	}
}
```