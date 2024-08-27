- [[Inheritance]]
- [[String]] class is final
- The modifier final means "unable to change".
- Final can be used for three different things
	- **final** before a variable makes the variable constant.
		- Final variables must be set before they are used.
		- Trying to set a final outside of explicit initialization or in a constructor results in a compiler error
```Java
public class FinalTest {
	public static final int LESS_TRAVELED = 0; //explicit initialization
	public final int SHORTEST;
	public FinalTest() {
		SHORTEST = 1; //constructor initialization
	}
}

public class FinalTest {
	public static final int LESS_TRAVELED = 0; //explicit initialization
	public final int SHORTEST;
	public foo() {
		SHORTEST = 1; //compiler error
	}
}
```



- **final** before a method makes the  it so method cannot be overridden.
```Java
public class Father {
	public final void drive() {
		setVelocity(45);
		setPath(LESS_TRAVELED);
		go();
	}
}

public class Son extends Father {
	public void drive() { //Illegal! Results in a compile error
		setVelocity(75);
		setPath(SHORTEST);
		go();
	}
}
```

- **final** before a class makes that class unextendable.
```Java
public final class Father {
	public final void drive() {
		setVelocity(45);
		setPath(LESS_TRAVELED);
		go();
	}
}

public class Son extends Father { //Illegal! Results in a compile error.
	
}
```