- To get [[Collection]] or Arrays to sort your types (MyDate, Person), the types must implement the Comparable interface.
```Java
public class MyDate implements Comparable{
	private int day, month, year;
	public MyDate(int month, int day, int year){
		this.day = day;
		this.year = year;
		this.month = month;
	}
	public int compareTo(Object o){
		MyDate d = (MyDate) o;
		if(year != d.year){
			return year - d.year;
		}
		if(month != d.month){
			return month - d.month;
		}
		if(month != d.month){
			return day - d.day;
		}
		return 0;
	}
}
```