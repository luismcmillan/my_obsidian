[[JavaScript]]
- Das `async`-Schlüsselwort wird verwendet, um eine Funktion zu deklarieren, die einen Promise zurückgibt. Eine Funktion, die als `async` deklariert ist, kann `await` verwenden, um auf die Erfüllung eines Promises zu warten.
```Typescript
async function fetchData() {
  return "Hello, World!";
}
```

- Das `await`-Schlüsselwort kann nur innerhalb von `async`-Funktionen verwendet werden und pausiert die Ausführung der Funktion, bis der Promise erfüllt (oder abgelehnt) ist. Es ermöglicht das Schreiben von asynchronem Code, der wie synchroner Code aussieht.
```TypeScript
async function fetchData() {
  const data = await fetch('https://api.example.com/data');
  return data.json();
}

```