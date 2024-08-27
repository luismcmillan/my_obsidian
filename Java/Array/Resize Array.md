[[Java Array]]
```Java
int[] array = {1,2,3};
int[] temp = array;
array = new int[4];
System.arrayCopy(temp, 0, array, 0 , temp.length);
temp = null;
```