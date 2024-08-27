[[Static methods]]

- Applications need constant values on occasion
	- **Along with abstract, static, and default methods, interfaces can also define constants**

```java
package com.intertech;
public interface SafeDriver {
	public static final int MAXIMUM_SPEED = 55;
	public static final int SAFE_FOLLOWING_DISTANCE = 100;
	public static final double MINIMUM_FUEL_LEVEL = 0.25;
	public static void printMaxSpeed(){
		System.out.println(MAXIMUM_SPEED);
	}
	public void drive();
	public void stop();
}
```

- Java has a feature to allow constants and static methods to be imported (from either a class or an interface) without importing the entire class.

```java
import static com.intertech.SafeDriver.printMaxSpeed;
public class Test {
	public static void main(String[] args){
		printMaxSpeed();
	}
}
```

- The code below imports all static members from the SafeDriver interface above. Note that a static import does not act as a traditional import

```java
import static com.intertech.SafeDriver.*;
public class Test {
	public static void main(String[] args){
		int speed = MAXIMUM_SPEED; // LEGAL
		double distance = SafeDriver.SAFE_FOLLOWING_DISTANCE; //ILLEGAL
		printMaxSpeed(); //LEGAL
	}
}
```

- Similar to regular imports, wildcards in static imports are not recursive


```java
public class Test {
	public static void main(String[] args){
		int rad = 5;
		double area = rad * rad * Math.PI;
	}
}
```

- **USING static imports, PI can be referenced without having to refer to it with Math.PI**

```java
import static java.lang.Math.PI;
public class Test {
	public static void main(String[] args){
		int rad = 5;
		double area = rad * rad * PI;
	}
}
```
