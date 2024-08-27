[[Date & Time]]

```Java
Period period = Period.of(3, 5, 12);
now = now.minus(period);
System.out.println(now); //2012-12-09T10:43:38.004  old_now =2016-05-21T10:36:37:371

now = now.plus(period);
System.out.println(now); //2012-12-09T10:43:38.004  old_now =2016-05-21T10:36:37:371

LocalDate now = LocalDate.now(); //now = 2016-05-21T10:43:38.004
LocalDate hireDate = LocalDate.of(2008, Month.APRIL, 21); //hireDate = 2008-04-21T13:00

Period period = Period.between(hireDate, now); 
System.out.println(period); // P8Y1M
```