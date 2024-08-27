[[Java Array]]
[[Polymorphism]]
```Java
Employee[] staff = new Employee[3];
staff[0] = new Employee();
staff[0].name = "James";
staff[1] = new Secretary();
staff[1].name = "Moneypenny";
staff[2] = new Manager();
staff[2].name = "Miles";
((Manager) staff[2]).department = "MI6";
```