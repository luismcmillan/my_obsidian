[[Java.io]]

```Java
File file = new File(file_path);
try {
	if (!file.exists()){
		BufferedWriter writer = new BufferedWriter(new FileWriter(file));
		writer.write("");
		writer.close();
	}
	BufferedReader reader = new BufferedReader(new FileReader(file));
	String line = "";
	while ((line = reader.readLine()) != null && !line.equals("") ) {
		String[] todo_array = line.split(",");
	}
	Logging.log(Level.INFO,"CSV file was read!");
	reader.close();
}catch(IOException e) {

}
```
