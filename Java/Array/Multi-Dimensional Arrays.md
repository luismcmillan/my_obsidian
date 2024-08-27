[[Java Array]]
```Java
String[][] array = new String[5][2]; //every dimention except from the last stores an array,the last stores the values
array[0][0] = "Paul";
array[0][1] = "183479294";
array[1][0] = "Henry";
array[1][1] = "1344";
```

```Java
String[][] array = {{"1", "a"},{"2", "b"},{"3", "c"}}; 
System.out.println(array.length); //3
System.out.println(array[0].length); //2
```
- Balance the Brackets
```Java
int[][] credentials = new int[3][2];
```

- Initializing the Final Dimension
```Java
int[][][] moreStuff = new int[3][3][];
moreStuff[0][2] = new int[2];
moreStuff[0][2][0] = 0; //LEGAL
moreStuff[0][2][1] = 1; //LEGAL

moreStuff[0][1][0] = 0; //ILLEGAL! Only [0][2] has a third Dimension
```

- First dimension must be given a size during its definition
```Java
int[][][] moreStuff = new int[3][][3]; //ILLEGAL
int[][][] moreStuff2 = new int[][3][3]; //ILLEGAL
int[][][] moreStuff3 = new int[][][3]; //ILLEGAL
```
