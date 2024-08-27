[[SQL]]
```Shell
sudo apt update
sudo apt install postgresql postgresql-contrib
sudo systemctl start postgresql
sudo systemctl enable postgresql
sudo systemctl status postgresql //überprüfen ob postgresql läuft
sudo -i -u postgres //anmelden als standard-postgres user
SELECT CURRENT_USER; // anzeigen welcher User aktiv ist
psql //Postgres Shell starten
psql -U obsidian_uploader -d datenbankname
\c obsidian_data //verbinden mit Datenbank
CREATE USER neuer_benutzername WITH PASSWORD 'sicheres_passwort'; //Neuen Benutzer anlegen
GRANT SELECT, INSERT, UPDATE, DELETE ON ALL TABLES IN SCHEMA public TO obsidian_uploader;
\l //um alle Datenbanken auf dem PostgreSQL-Server
\dt mein_schema.* //List all tables
\dn //List all schemas
psql --version //welche Version
psql -d meine_datenbank //Verbinden mit 'meine_datenbank'
\q //PostgreSQL-Shell verlassen
exit //Verlassen Sie den `postgres`-Benutzer und kehren Sie zu Ihrem regulären Benutzer
```