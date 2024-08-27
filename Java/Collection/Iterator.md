[[Collection]]
```Java
Iterator iter = list.iterator();
while(iter.hasNext()){
	System.out.println(iter.next());
}
```
- Iterator Interface only defines three methods
	- public boolean hasNext()
	- public Object next()
	- public void remove()
- ListIterator has more functions