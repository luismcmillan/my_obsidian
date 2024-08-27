[[Deque]]
- As is generally the case with Deques, ArrayDeque as no size limit, They grow as necessary to support the elements added to them
- Also as is generally the case with Deques, null elements are not allowed in an ArrayDeque
- ArrayDeque objects are not thread-safe
```Java
ArrayDeque deque = new ArrayDeque();
deque.offerFirst("Bruce Banner"); // could also call add()
deque.offerFirst("Bruce lala");
deque.offerLast("Bruce huhu"); // 
String superHero = (String) deque.pollLast() // could also be removeFirst()
String nextHero = (String) deque.peekFirst() 
```
