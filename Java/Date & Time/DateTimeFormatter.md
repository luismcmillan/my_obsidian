[[Date & Time]]

```Java
LocalDate now = LocalDate.now();
System.out.println(now); // 2016-05-21

DateTimeFormatter dtf = DateTimeFormatter.ofLocalizedDate(FormatStyle.FULL);
System.out.println(now.format(dtf)); //Saturday, May 21, 2016 

DateTimeFormatter dtf = DateTimeFormatter.ofLocalizedDate(FormatStyle.LONG);
System.out.println(now.format(dtf)); //May 21, 2016 

DateTimeFormatter patternFormatter = DateTimeFormatter.ofPattern("yyyy/dd/M");
System.out.println(now.format(patternFormatter)); // 2016/21/5

DateTimeFormatter patternFormatter = DateTimeFormatter.ofPattern("yyyy/dd/MM");
System.out.println(now.format(patternFormatter)); // 2016/21/05

DateTimeFormatter patternFormatter = DateTimeFormatter.ofPattern("dd 'in the year of' yyyy");
System.out.println(now.format(patternFormatter)); //21 in the year of 2016 
```