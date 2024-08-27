[[Java Array]]
- Array have a supporting class to aid sorting: java.util.Arrays
- Use the stativ Arrays.sort() method to sort an array
	- If no comparison instructions are passed in to sort ([[Comparable]]), primitives are sorted by Unicode value
```Java
char[] letters = {'d','a','c','b'};
Arrays.sort(letters);
```
- Array.binarySearch() searches an array and returns the index of the searched for element. **Arrays must be sorted for a binary search to work**.
```Java
int cLocation;
cLocation = Arrays.binarySearch(letters, 'c');
// Expected index of e: 4 // cLocation = (4+1)*-1 // cLocation = -5
```
- Arrays.fill() fills all elements of an array with one value.
```Java
Arrays.fill(letters, 'z');
```
- Arrays of chars were used in the examples above. However, all the methods above are overloaded to handle any type of array.