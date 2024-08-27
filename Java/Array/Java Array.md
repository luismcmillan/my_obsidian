- An array is an object that represents a homogeneous collection of integer-indexed objects
```Java
int[] intArrayOne;
int intArrayTwo[];
```

```Java
char[] charArrayOne, charArrayTwo; //two arrays
char charArrayThree[], charOne; //charArrayThree array, and charOne char
```

- When you instantiate an array, you define how large the array will be.

```Java
int[] intArray = new int[10];
```
- When using the *new* keyword, the elements of the array are initialized to their default values (zero in the case of an in array)
```Java
int[] intArray = new int[10];
intArray[0] = 1;
intArray[1] = 2;
intArray[10] = 11; //This will fail at runtime
```

- Arrays have a special syntax built in that allow declaration, instantiation, and assignment all in one step
```Java
int[] intArray = {1,2,3,4,5,6,7,8,9,10};
```

- The special syntax is only allowed when you declare the array  initially
```Java
int[] intArray;
intArray = {1,2,3,4,5,6,7,8,9,10}; //ILLEGAL
```
- The length of an array is a read-only attribute that is set when the array is created
```Java
System.out.println(intArray.length); //displays 10
```

- Arrays can hold any Java object type.
```Java
MyDate[] dates = new MyDate[3]; //three slots with null
dates[0] = new MyDate(10,26,1999);
dates[1] = new MyDate(10,26,1999);
dates[2] = new MyDate(10,26,1999);
MyDate[] moreDates = { new MyDate(10,26,1999), new MyDate(10,26,1999) };
```

![[Resize Array]]

![[Array Polymorphism]]

![[Multi-Dimensional Arrays]]

![[Array Sorting and Searching]]

![[Varargs]]