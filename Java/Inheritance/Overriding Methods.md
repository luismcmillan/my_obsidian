- [[Inheritance]]
- An overriding method cannot be less accessible than the inherited method
- return type must be the same or a subtype of the overridden return type ([[Covariant Returns]])
- Overriding methods cannot declare additional Exceptions than those declared in the overridden method, **unless** the new Exceptions are either a subtype of one of the overridden exceptions, or a "runtime" exception.
- The **super** keyword can also be used to call on the super class's methods
```Java
public class Father {
	public void drive() {
		setVelocity(45);
		setPath(LESS_TRAVELED);
		go();
	}
}

public class Son extends Father {
	public void drive() {
		setVelocity(75);
		setPath(SHORTEST);
		go();
	}
	
	public void driveLikeDad() {
		super.drive(); //Calls on the Father drive method
		super.super.drive(); //ILLEGAL
	}
}
```