[[Collection]]
- The ArrayList is a collection that represents a dynamically resizable array.
- Working with an ArrayList is almost as easy as working with an array.
	- using [[add()]] method to add elements to the ArrayList
	- using [[size()]] to access ArrayList's size
	- using [[remove()]] to remove an ekement
	- using [[contains()]] method to see whether an object is in ArrayList
	- using [[clear()]] to empty all elements

```Java
import java.util.*;
public class TestArrayList{
	public void main(String[] args) {
		ArrayList list = new ArrayList();
		list.add("Hello");
		list.add("world");
		System.out.println(list);
	}
}
```

- You can set the initial size of the ArrayList with its constructor
```Java
ArrayList list = new ArrayList(4);
```