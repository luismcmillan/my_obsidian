- elements with a "higher" order are moved to the head of the queue
- The elements are ordered according to their natural ordering
- **PriorityQueue is unbounded with regard to capacity**
	- capacity grows automatically
```Java
PriorityQueue queue = new PriorityQueue();
queue.offer("Bruce Banner"); // could also call add()
queue.offer("Bruce lala");
queue.offer("Bruce huhu"); // 
String superHero = (String) queue.poll() // could also call remove()
String nextHero = (String) queue.peek() // could also call element()
```