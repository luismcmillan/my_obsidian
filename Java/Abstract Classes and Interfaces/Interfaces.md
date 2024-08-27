- An Interface **is a contract** that a class signs.
- **An Interface defines behavior expected of Implementers**
	- a class *implements* and **overrides** the methods defined in the Interface
[[Abstract Classes]]
```java
public class Cat extends Animal implements Drawable{
	//must provide a draw method because it implements Drawable
	public void draw(){
		//Draw Logic implementation
	}
}

public abstract class Shape implements Drawable { 
	public abstract double area(); 
} 

public class Circle extends Shape { 
	public double r; //radius 
	public double area(){ 
		return Math.PI * r * r; 
	} 
	//Must provide a draw method because Shape implements Drawable
	public void draw() {
		...
	}
} 
public class Rectangle extends Shape { 
	public double h, w; //height and width
	public double area() { 
		return h * w; 
	} 
	//Must provide a draw method because Shape implements Drawable
	public void draw() {
		...
	}
}

```




![[Pasted image 20240613202538.png]]



- Interfaces can extend other Interfaces
	- **A class can extend only one class, but can implement an unlimited number of interfaces**
	- BUT if a class implements two or more interfaces with the same default method signature, **the implementing class MUST override the method(s).**

```java
public class Foo implements Drawable, Runnable, Serializable{
	public void draw(){}
	public void run(){}
}
```

- Interfaces are defined in their own file with **.java** extention
- can only contain methods that are **public** and are (and only one) of those:
	- **abstract**
	- **default**
	- **static**
- **public is implied**, somtimes it is not present in the declaration
- Also, if neither abstract, default, or static, it is set to **abstract**
- can only contain variables that are **public, static and final**

- Interfaces are implemented by classes
	- **like an abstract class, no instances of an interface are ever created**
- [[Default Methods]]
	![[Default Methods]]
	- [[Static methods]]
	![[Static methods]]
- [[Implementing Interfaces]]
	![[Implementing Interfaces]]
- [[Marker Interface]]
	![[Marker Interface]]
- [[Functional Interface]]
	![[Functional Interface]]