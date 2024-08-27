- Note that execution does not return to finish the rest of the main() method
- it is common to see the last catch block look for the most generic Exception type.
- The Compiler helps insure that the more specific exceptions are caught before the more generic
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
	}
}
```
![[Finally]]
- try will have zero or more catch blocks and zero or one finally blocks
	- try-catch-[[Finally]]
	- try-catch
	- try-[[Finally]]