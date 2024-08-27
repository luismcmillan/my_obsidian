- [[Lambda Expressions]]
![[Pasted image 20240626145032.png]]
- If there are multiple parameters passed into the interface method, they need to be comma separated:
```java
(String a, String b, String c) -> ( return a + b + c;)
```
- If there are no parameters, use an empty set of parentheses
 ```java
() -> ( return "Hello!";)
```


**The lambda syntax may be simplified if certain conditions are met.**
```java
(double percentage) -> {return salary + (percentage * salary);}
```
- The parameter type is optional
```java
(percentage) -> {return salary + (percentage * salary);}
```
- If there is only one parameter, and the parameter type has been omitted, the parentheses that surround the parameter are optional
```java
percentage -> {return salary + (percentage * salary);}
```
- If there is only one statement in the body, the curly braces, "return" keyword, and semicolon are optional. However they all exist together as a group; either they all appear together or they are omitted together
```java
percentage -> salary + (percentage * salary)
```

**Now the cutCheck method invocation looks like this**
```java
double salary = 75_000;
cutCheck( percentage -> salary + (percentage * salary));
```
