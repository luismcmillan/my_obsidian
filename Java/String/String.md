[[Java]]
- Java String objects are a sequence of chars
```Java
String s = new String("Hello World");
```
![[Pasted image 20240609124429.png]]
```Java
String mystring1 = new String("Mulligan");
String mystring2 = new String("Mulligan");
```
- When creating a String object using "new" keyword and the String constructor, a new String object is always created!
- **This is true even when the sequence of chars is the same**
![[Pasted image 20240609125024.png]]
```Java
String mystring3 = "Seamus";
String mystring4 = "Seamus";
```
- But when using String literals, only one object is created on the heap that many references point to
![[Pasted image 20240609125250.png]]
[[Immutable Strings]]