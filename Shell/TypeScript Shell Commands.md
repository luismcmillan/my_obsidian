[[TypeScript]]
[[Shell]]
```Shell
npm install -g typescript
# Installiert TypeScript global auf dem System.

tsc --init
# Initialisiert ein neues TypeScript-Projekt und erstellt eine tsconfig.json-Datei.

tsc filename.ts
# Kompiliert eine TypeScript-Datei in JavaScript.

tsc -w
# Startet den TypeScript-Compiler im Überwachungsmodus, um Änderungen automatisch zu kompilieren.

node filename.js
# Führt die kompilierte JavaScript-Datei mit Node.js aus.

npx ts-node filename.ts
# Führt eine TypeScript-Datei direkt aus, ohne sie vorher manuell zu kompilieren.

npm install --save-dev @types/node
# Installiert Typdefinitionen für Node.js als Entwicklungsabhängigkeit.

```