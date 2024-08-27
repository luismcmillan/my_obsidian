- [[Java]]
- [[The Object Class]]
- Polymorphism is about substitutability.
- The flexibility provided through polymorphism allows the implementation of the pay() method to be changed **without requiring other code to be changed**
- [[Object Type Casting]]

```Java
public class PayService {
	public void cutCheck(Employee e ) {
		double gross = e.pay();
	}
}
```


![[Benefits of Polymorphism]]