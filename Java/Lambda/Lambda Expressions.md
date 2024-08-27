- A Lambda expression (or simply, "lambda"), is a syntax used to pass a block of code into a method that accepts a functional interface parameter.
	- **RATHER than creating an entire class that implements the functional interface, the developer is able to simply pass in an implementation of the interface's sole method

**Traditional interface/implementation example**
- The functional interface, Payable, defines a method to give an employee a raise:
```java
public interface Payable {
	public abstract double raiseSalary(double percentage);
}
```
- A cutCheck method accepts a Payable as a parameter:
```java
public void cutCheck(Payable p){
	double updatedSalary = p.raiseSalary( .04 ); //cut check with new updatedSalary
}
```
- A Consultant class implements the interface:
```java
public class Consultant implements Payable{
	private double saraly = 80_000.0;
	public double raisSaraly(double percentage){
		return saraly + (salary * percentage);
	}
}
```
- ... and cutCheck is passed a Consultant instance as a Payable argument
```java
Consultant uxEngineer = new Consultant();
cutCheck(uxEngineer);
```
This code works as expected, however anytime we want to make a new raiseSalary implementation, we'll need to create a new class (or [[Anonymous Class]])
- **Lambda expressions allow us to pass in the functional interface method implementation, without having to create an entire class for it.**
```java
double salary = 75_000;
cutCheck(
( double percentage ) -> {return salary + (percentage*salary);}
);
```
-![[Lambda syntax]]
![[Predicate]]