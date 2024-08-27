- [[Lambda Expressions]]
- Java includes a [[Functional Interface]] called "Predicate" to handle a very common scenario: a "test" method is onvoked with a parameter, resulting in a **boolean outcome**
- The type is 

```java
Predicate<T>
```

where "T" can be any type needed in the test.

- It's single abstract method is: **boolean test(T t)**, which uses the same parameter type declared in the Predicate reference
- The syntax that supports "T" as a variable of any type is called "Generics" [[Generics and Autoboxing]].

```java
public class PromotionsService {
	private Customer customer = new Customer();
	public void sendPromotion(Predicate<Customer> p){
		if(p.test(customer)){
			//Send promotional mailing
		}
	}
}
```
- **NOW any code that calls sendPromotion can pass in a lambda expression that executes the test, based on any criteria desired:

```java
PromotionService ps = new PromotionsService();
ps.sendPromotion( customer -> customer.getAge() >= 18);
```