- [[Interfaces]]
- A default method is one that includes a body
	- a normal method (with additional "default" modifier)
- **No instance members are accessible inside the default implementation, cause interfaces only have access to public static and final state**
```java
public interface Drawable {
	public default void draw(){
		//Drawing code
	}
}
```
- **"default" modifier may only appear in interfaces. Not legal in abstract or concrete classes**
- These give us the opportunity to introduce new methods, **without "breaking" classes that already implements the interface**.