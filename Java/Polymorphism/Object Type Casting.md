- [[Polymorphism]]
- Casting in primitive data types is used to force truncation of larger types such as int into smaller types such as byte
- With Objects, casting is used to return an object to a more specific type.
```Java
Person p = new Employee();
System.out.println(p.getDescription());
Employee e = (Employee) p;
```

- The typecast in this case is used to get functionality back into the reference.
- A typecast can also be done without creating another reference
```Java
Person p = new Employee();
System.out.println(p.getDescription());
((Employee) p).title = "Instructor"
```

- Typecasting objects must be used with care, as it can be used incorrectly
```Java
Person p = new Person();
Employee e = (Employee) p; //Compiles but fails at runtime
//Casting doesn't change the object, IT ONLY changes the reference
```

- This code will generate a ClassCastException
![[Protect Casts at Runtime]]