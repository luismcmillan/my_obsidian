[[Node.js]]
```Javascript
import { exec } from 'child_process';
// Pfad zu Ihrer C++-executable Datei
const executablePath = './test'; // oder './myprogram.exe' unter Windows
exec(executablePath, (error, stdout, stderr) => {
	if (error) {
		console.error(`Fehler beim Ausführen des Programms: ${error.message}`);
		return;
	}
	if (stderr) {
		console.error(`Fehlerausgabe: ${stderr}`);
		return;
	}
	// Ausgabe des Programms
	console.log(`Ausgabe: ${stdout}`);
});
```