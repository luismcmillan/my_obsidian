
- A covariant return is where a subtype is listed in the place of a supertype.
	- [[Overriding Methods]] may use covariant return
```Java
public class GrandFatherRegistry {
	public Grandfather whosMyAncestor(String ssn){
	}
}

public class FatherRegistry extends GrandFatherRegistry{
	public Father whosMyAncestor(String ssn){
	}
}
```