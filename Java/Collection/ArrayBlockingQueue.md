[[Queues]]
- An ArrayBlockingQueue implements a first-in-first-out (FIFO) Queue.
- ArrayBlockingQueues hold a fixed number of elements.
```Java
ArrayBlockingQueue queue = new ArrayBlockingQueue(3);
queue.offer("Bruce Banner"); // could also call add()
queue.offer("Bruce lala");
queue.offer("Bruce huhu"); // not added, queue at capacity
String superHero = (String) queue.poll() // could also call remove()
String nextHero = (String) queue.peek() // could also call element()
```