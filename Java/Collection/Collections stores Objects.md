[[Collection]]
```Java
List staff = new ArrayList();
Employee e = new Employee();
e.name = "Steve";
staff.add(e);
Secretary s = new Secretary();
s.name = "William";
staff.add(s);
String x = "Mr. Johnson";
staff.add(x);
Employee bill = (Employee)staff.get(1);
```