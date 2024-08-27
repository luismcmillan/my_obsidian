- A [[Throwable]] object is given as an argument to each [[Catching Exceptions]] block.
	- The object may contain useful information to both the application and the developer.
	- Each Throwable has a set of methods that allow you to access that information within the catch block.
		- getCause()
		- getMessage()
		- getStackTrace
		- printStackTrace()
```Java
public static void main(String[] args) {
	try{
		String str = "A char string";
		System.out.println("Before problem");
		char ch = str.charAt(20);
		System.out.println("After problem");
	} catch (StringIndexOutOfBoundsException e){
		System.out.println("Problem: "+ e.getMessage());
		e.printStackTrace()
	}
}
```
