[[Sets]]
```Java
Treeset tree = new TreeSet();
tree.add("88");
tree.add("53");
tree.add("12"); 
tree.add("120"); 
Iterator iter = tree.iterator();
while(iter.hasNext()){
	System.out.println(iter.next() + " ") //12 53 88 120
}
```
- Treesets rely on the use of compareTo() to sort stored components automatically
- Otherweise, the TreeSet uses Comparator that is passed to the constructor during instantiation 
- Internally, TreeSets use a tree organization to organize the set, but you have no control over links between oarents
- Even though TreeSets are ordered, items in the set are no indexed. Therefore you cannot insert or fetch values from index