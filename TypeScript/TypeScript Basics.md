[[TypeScript/TypeScript]]
```TypeScript
let age: number = 25;
let name: string = "Max";
// Statische Typisierung: Variablen haben festgelegte Typen, was Fehler frühzeitig erkennt.

interface Person {
    name: string;
    age: number;
}
const user: Person = { name: "Anna", age: 30 };
// Interfaces definieren die Struktur von Objekten und helfen bei der Typensicherheit.

class Animal {
    name: string;
    constructor(name: string) {
        this.name = name;
    }
    move(distanceInMeters: number = 0) {
        console.log(`${this.name} moved ${distanceInMeters}m.`);
    }
}
class Dog extends Animal {
    bark() {
        console.log("Woof! Woof!");
    }
}
const dog = new Dog("Rex");
dog.bark(); 
dog.move(10); 
// Klassen und Vererbung ermöglichen eine objektorientierte Programmierung mit TypeScript.

function identity<T>(arg: T): T {
    return arg;
}
let output1 = identity<string>("Hello");
let output2 = identity<number>(42);
// Generics ermöglichen es, Funktionen und Klassen für verschiedene Datentypen zu verwenden.

export function add(a: number, b: number): number {
    return a + b;
}
import { add } from "./mathUtils";
console.log(add(5, 3)); 
// Das Modul-System unterstützt die Strukturierung und Wiederverwendung von Code.

```