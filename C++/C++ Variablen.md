[[C++]]
```C++
#include <iostream>
#include <string>
#include <vector>
#include <map>
int main() {
    // Grundlegende Datentypen
    int age = 25;                // Ganze Zahl
    short int smallNumber = 10;  // Kurze ganze Zahl
    long int largeNumber = 100000L; // Lange ganze Zahl
    unsigned int positiveAge = 30; // Nicht-negative ganze Zahl

    float pi = 3.14f;            // Einzelpräzision Gleitkommazahl
    double e = 2.718281828;      // Doppelpräzision Gleitkommazahl
    long double bigNumber = 1.234567890123456789L; // Erweiterte Präzision Gleitkommazahl

    char initial = 'A';          // Einzelnes Zeichen
    unsigned char letter = 'B'; // Nicht-negative Zeichenwerte

    bool isTrue = true;          // Wahrheitswert

    // Automatische Typbestimmung
    auto num = 10;               // int
    auto decimal = 3.14;         // double

    // Typbestimmung durch Ausdruck
    decltype(num) anotherNum = 20; // int

    // Konstante Variablen
    const int daysInWeek = 7;

    // Volatile Variable (Selten verwendet)
    volatile int hardwareStatus;

    // Statische Variable
    static int count = 0;

    // Externe Variable
    extern int externalVar;

    // Mutable Variable innerhalb einer Klasse
    struct MyClass {
        mutable int x;
    };

    // Zeiger
    int value = 10;
    int* ptr = nullptr;          // Null-Zeiger
    double* dblPtr = new double(5.5); // Zeiger auf double

    // Referenzen
    int& ref = value;            // Referenz auf int
    int* p = nullptr;
    int*& refToPtr = p;          // Referenz auf einen Zeiger

    // Arrays
    int numbers[5] = {1, 2, 3, 4, 5};          // Einfaches Array
    int matrix[3][3] = {{1, 2, 3}, {4, 5, 6}, {7, 8, 9}}; // Mehrdimensionales Array

    // Strukturen
    struct Person {
        std::string name;
        int age;
    };

    Person person1 = {"Alice", 30};

    // Klassen
    class Rectangle {
    public:
        int width;
        int height;
        int area() {
            return width * height;
        }
    };
    Rectangle rect = {10, 20};
    // Standardbibliothekstypen
    std::string greeting = "Hello, World!"; // String-Klasse
    std::vector<int> vec = {1, 2, 3, 4, 5}; // Dynamisches Array

    std::map<std::string, int> ages = {{"Alice", 30}, {"Bob", 25}}; // Assoziative Container


    return 0;
}

```