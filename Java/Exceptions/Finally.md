[[Catching Exceptions]]
```Java
public static void main(String[] args) {
	try{
		String str = "A char string";
		System.out.println("Before problem");
		char ch = str.charAt(20);
		System.out.println("After problem");
	} catch (StringIndexOutOfBoundsException e){
		System.out.println("Hey - your strings not that big!");
	} catch (CoolException e | Nullpointerexception e){
		System.out.println("Hey - your strings not that big!");
	}catch (Exception e){
		System.out.println("Ooops, unexpected problem occured!");
	} finally {
		System.out.println("finally");
	}
}
```

The "try-with resources" syntax allows us to omit the finally clause, by calling "close" at the end of the method (or before an exception is thrown) on our behalf.![[try-with resources]]