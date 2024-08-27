[[Interfaces]]
- They list **"static"** modifier
- Concrete classes do not inherit static methods like they do [[Default Methods]]. All static method calls must be done through the Interface itself.
	- invoked by the reference Type not be the real runtime object

```java
public interface Drawable{
	public static void draw(){
		//Drawing code here..
	}
}
public class Rectangle implements Drawable {
	public void testBehavior() {
		draw(); //illegal
		Rectangle.draw(); //illegal
		Drawable.draw(); // LEGAL
	}
}
```

![[Static Imports]]