[[Throwable]]

```Java
import java.net.*;
public class TestConnection {
	public static void main(String[] args){
		try{
			openHttpConnection("http://www.google.com");
		} catch (MalformedURLException e){
			System.out.println("Hey - the URL isn't correct");
		}
	}
	public static void openHttpConnection(String url) throws MalformedURLException{
		URL site = new URL(url);
	}
}
```

- even main() method could also be written to throw exception
	- **BUT NOT GOOD, programm will crash**
```Java
public static void main (String[] args) throws MalformedURLException {
	openHttpConnection();
}
```