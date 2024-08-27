- Comparator is located in the java.util.package
- A class implementing the Comparator interface must implement the compare() method
- The compare() method takes two Objects as arguments
- The compare() method returns
	- positive if first argument is **larger** than second
	- zero if equal
	- negativ if second argument is **larger** than first
- The Comparator is useful when comparing elements of a heterogeneous collection and third-party classes you don't have source to.
```Java
public class MyDate implements Comparator{
	private int day, month, year;
	public MyDate(int month, int day, int year){
		this.day = day;
		this.year = year;
		this.month = month;
	}
	public int compare(Object o1, Object o2){
		MyDate d1 = (MyDate) o1;
		MyDate d2 = (MyDate) o2;
		if(d1.year != d2.year){
			return d1.year - d2.year;
		}
		if(d1.month != d2.month){
			return d1.month - d2.month;
		}
		if(d1.month != d2.month){
			return d1.day - d2.day;
		}
		return 0;
	}
}
```