- [[Java.nio]]
```java
import java.nio.file.*;

Path directory = Paths.get("/Users/luismcmillan/Documents/My_obsidian");
if (Files.exists(directory) && Files.isDirectory(directory)) {
	
	try (DirectoryStream<Path> stream = Files.newDirectoryStream(directory)) {
		for(Path file: stream){
			System.out.println(file.getFileName());
		}
	} catch (IOException e) {
		e.printStackTrace();
	}
}
```