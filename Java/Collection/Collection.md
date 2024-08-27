[[Java]]
- The collection framework is a set of prebuilt data structure components
- There are two basic types in the collection framework, all of which are found in the **java.util** package
	- [[Lists]]
		- [[ArrayList]]
		![[ArrayList Pro and Cons]]
		- LinkedList
		![[LinkedList Pro and Cons]]
	- [[Sets]]
		- [[HashSet]]
		- [[TreeSet]]
	- [[Queues]]
	- [[Deque]]
	- [[Maps]]
[[Iterator]]

Limitations:
- Collections can't store primitive data types [[Java Wrapper]] 
```Java
List list = new ArrayList();
int j = 7;
list.add(j); //adding int to a collection - requires Java SE5 or greater
```
- Everything in a collection is treated or stored as an Object reference
	- Collections can be heterogeneous data structures. **This makes collections powerful data structures capable of grouping all sorts of objects/data
	- However, each collection generalizes the objects that are added to it.
	- When you retrieve an object from any collection (List, Set, Map, and so on), it returns an Object reference ![[Collections stores Objects]]
- [[Generics and Autoboxing]]
- [[Collection Sorting & Searching]]