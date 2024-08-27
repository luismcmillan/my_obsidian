[[Node.js]]
[[NPM Shell Commands]]

```Javascript
import pkg from 'pg';
const { Client } = pkg; // Konfiguration der Verbindung 
const client = new Client({ user: 'dein_db_benutzer', host: 'localhost', database: 'deine_datenbank', password: 'dein_passwort', port: 5432, }); //Verbindung herstellen 
client.connect() .then(() => console.log('Mit der Datenbank verbunden')) .catch(err => console.error('Verbindungsfehler', err.stack)); // Eine einfache Abfrage ausführen 
client.query('SELECT NOW()', (err, res) => { if (err) { console.error(err); } else { console.log('Datenbankzeit:', res.rows[0]); } // Verbindung beenden 
											client.end(); });
```