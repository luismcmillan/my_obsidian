[[Throwable]]
- Your Exception class must indectly extend java.lang.Throwable

```Java
public class OverdraftException extends Exception {
	public OverdraftException(String message) {
		super(message);
	}
}

public void withdraw(double amount) throws OverdraftException {
	if(balance - amount < 0){
		throw new OverdraftException("insufficient funds");
	}
}

```
