[[Date & Time]]

```Java
LocalDateTime now = LocalDateTime.now();
System.out.println(now); //2016-05-21T10:36:37:371

LocalDateTime timeHired = LocalDateTime.of(2008, Month.APRIL, 21, 13, 0, 0);
System.out.println(timeHired); //2008-04-21T13:00

System.out.println(now.isBefore(timeHired)); //false
```