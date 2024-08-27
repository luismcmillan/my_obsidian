[[Java.io]]
```Java
try {
	// Erstellen eines BufferedWriter-Objekts für effizienteres Schreiben
	BufferedWriter bufferedWriter = new BufferedWriter(new FileWriter(location));
	// Schreiben des Inhalts in die Datei
	bufferedWriter.write(content);
	// Schließen des BufferedWriter-Objekts
	bufferedWriter.close();
} catch (IOException e) {
	System.out.println("Ein Fehler ist aufgetreten."); e.printStackTrace();
}
```
