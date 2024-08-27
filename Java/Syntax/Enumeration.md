[[Java Syntax]]
```Java
public enum Days {
	SUNDAY, MONDAY, TUESDAY, WEDNESDAY, THURSDAY, FRIDAY, SATURDAY
}

public class CourseExample{
	public static void main(String[] args){
		Days today = Days.FRIDAY;

		switch(today){
		case MONDAY:
			response = "Get to work!";
			break;
		case FRIDAY:
			response = "Time to relax";
			break;
		default:
			response = "Practice Java"; 
		}
		System.out.println(response);
	}

}


public enum MusicType {
	CLASSICAL(1), JAZZ(4), ROCK(6), METAL(11);
	private int earDamageFactor;

	private MusicType(int earDamageFactor){
		this.earDamageFactor = earDamageFactor;
	}

	public String toString(){// Ordinal CLASSICAL=0, JAZZ=1, ROCK=2
		return this.name() + "-"+ this.ordinal()+ "-"+ this.earDamageFactor;
	}
}


```