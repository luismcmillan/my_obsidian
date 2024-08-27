[[Date & Time]]
```Java
LocalDate now = LocalDate.now();
System.out.println(now); // 2016-05-21

LocalDate hireDate = LocalDate.of(2008, Month.APRIL, 21);
System.out.println(hireDate); // 2008-04-21
System.out.println(hireDate.isBefore(now)); // true

LocalDate aWeekFromNow = now.plusWeeks(1);
System.out.println(aWeekFromNow); // 2016-05-28

LocalDate aWeekAgo = now.minusWeeks(1);
System.out.println(aWeekAgo); // 2016-05-14
```
