[[Interfaces]]
While an IDE or a compiler will complain if you make this mistake, you won't have these tools when taking the exam.  So remember: all interface methods are public, even if they don't use the public keyword.

Therefore given the following legal interface:
```Java
public interface Payable {
	double pay();
}
```


Unlike interface methods, concrete implementations MUST include the public modifier.  Therefore, the following code will **not** compile because pay() is missing the "public" modifier. 

<font color="red"> WRONG:</font>
```java
public class Consultant implements Payable {
    double pay() {
        return 80_000.0;
    }
}
```



The <font color="green"> CORRECT:</font> code is:
```java
public class Consultant implements Payable {
    public double pay() {
        return 80_000.0;
    }
}
```

