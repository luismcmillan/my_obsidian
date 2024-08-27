[[Java]]
**Strings objects are immutable**
	- Once created and initialized, a String cannot be changed on the same reference
```Java
String a = "It is ";
String b = "a dog ";
String c = "day afternoon.";
```
![[Pasted image 20240609125934.png]]
```Java
a = a + b + c;
c = "Wow";
```
![[Pasted image 20240609130133.png]]
