- Abstract methods have no **{}, no body, no implementation**
- if a class has even one abstract method, the hole class must be abstract!
- **NO *new* keyword**, Abstract classes can't be instantiated
- Descendant classes of an abstract class **must implement** the inherited abstract methods or become **abstract themselves**
- Abstract classes provide generalizations, or relationships, between classes. This relationship can be exploited using polymorphism.

**NOT ALLOWED FOR METHODS**
- private
- static
- final
because all methods **must** be overridden, which is not allowed with private, static and findal

## abstract Shape
```Java


public abstract class Shape{
	public abstract double area();
}
public class Circle extends Shape {
	public double r; //radius
	public double area(){
		return Math.PI * r * r;
	}
}
public class Rectangle extends Shape {
	public double h, w; //height and width
	public double area() {
		return h * w;
	}
}
```


When we say that a concrete subtype must make sure all abstract methods are overridden, it doesn't necessarily mean that all of the abstract methods are implemented **in** the subtype.  Basically, the rule is that for a class to be concrete, it must make sure that any method call has some concrete definition that can be invoked.  And that concrete definition could be defined in a supertype (even in an abstract class!)

```java
public abstract class Person {
    protected String firstName;
    public abstract String getName();
}

public abstract class Employee extends Person {
   protected String title;
   public abstract double pay();
   public String getName()  {
		return title + ": " + firstName;
	}
}

  

public class Consultant extends Employee {
    public double pay() {
        return 80_000.0;
    }
}
```
Notice that Person defines an abstract method (getName()), and it is not implemented in the Consultant class. This is perfectly OK because Employee defines getName(). When we instantiate a Consultant and call getName(), the concrete implementation defined in Employee is available... and that satisfies the main rule: a class may become concrete (non-abstract), as long as all abstract methods in its hierarchy have a corresponding concrete implementation.

