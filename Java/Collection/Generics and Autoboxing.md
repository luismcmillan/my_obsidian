[[Collection]]
- Generics allow you to specify the intended data type to be stored in a reference.
```Java
List<Integer> primes = new ArrayList<Integer>();
primes.add(Integer.valueOf(1));
primes.add(Integer.valueOf(2));
primes.add(Integer.valueOf(3));
primes.add(Integer.valueOf(4));
primes.add(Integer.valueOf(5));
int x = primes.get(1).intValue();
```
- **Autoboxing** is the automatic conversion the compiler makes between Java primitives and their corresponding object wrapper classes.
```Java
Integer y = 5;
System.out.println(y);
```
- Unboxing allows primitive type references to be assigned wrapper objects.
```Java
int z = y;
System.out.println(z);
```
- real coding time-saver:
```Java
List<Integer> primes = new ArrayList<Integer>();
primes.add(1);
primes.add(2);
primes.add(3);
primes.add(4);
primes.add(5);
int x = primes.get(1);
```