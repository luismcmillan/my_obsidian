[[Date & Time]]
```Java
LocalTime now = LocalTime.now();
System.out.println(now); //10:32:20.533

LocalTime timeHired = LocalTime.of(13, 0, 0);
System.out.println(timeHired); //13:00

LocalTime anHourFromNow = now.plusHours(1);
System.out.println(anHourFromNow); //11:34:56  (now =10:34)

LocalTime anHourEarlier = now.minusHours(1);
System.out.println(anHourEarlier); //09:34:56  (now =10:34)

System.out.println(timeHired.isAfter(now)); //true
```