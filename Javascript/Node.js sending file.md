[[Node.js]]
[[Express]]
```Javascript
import express from 'express';
import fs from 'fs/promises';
import path from 'path';
import cors from 'cors';
import { fileURLToPath } from 'url';
import { dirname } from 'path';
const __filename = fileURLToPath(import.meta.url);
const __dirname = dirname(__filename);
const app = express();
const port = 3000;

app.use(cors());
app.get('/', async (req, res) => {
	try {
		const dataPath = path.join(__dirname, 'obsidian.json');
		const data = await fs.readFile(dataPath, 'utf8');
		const jsonData = JSON.parse(data);
		console.log(jsonData);
		res.json(jsonData);
	} catch (error) {
	console.error('Fehler beim Lesen der Datei:', error);
	res.status(500).json({ message: 'Interner Serverfehler' });
	}
});

app.listen(port, () => {
	console.log(`Server läuft auf http://localhost:${port}`);
});
```