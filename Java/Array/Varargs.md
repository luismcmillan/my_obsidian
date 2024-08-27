[[Java Array]]
- There may be times when you need to pass a variable number of arguments to a method.
	- One option is to create a method that accepts an array:
```Java
public void myMethodtakesLotsofInts(int[] manyInts){
	...
}
//OR
public void myMethodtakesLotsofInts(int... manyInts){ // myMethodtakesLotsofInts(2,3,4,6);
	...
}
```
- Under the covers, Java treats the variable length argument as an array whose elements are all of same type
- The use of varargs and the ellipsis can occur only once in a parameter list.
	- **must always be placed at the end of the parameter list**
```Java
public void myMethodtakesLotsofInts(String aString, double someDouble,int... manyInts){ 
	...
}
```

- Also, main may be legally written using varargs instead of a String
```Java
public static void main(String... args){

}
```