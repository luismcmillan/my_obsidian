- [[Interfaces]]
- An Interface that has one, and only one **abstract** method is known as a "Functional" Interface.
	- if abstract, static or default mentioned, **then assumed to be abstract**
```java
public interface Payable{
	double raiseSalary(double percentage);
}
```
- Even if an interface contains multiple default and/or static methods, it is still considered "functional" if it is limited to **one abstract method**
	- The single exception the this "onlx one abstract method" rule is if the additional abstract methods are overriding ones declared in java.lang.Object