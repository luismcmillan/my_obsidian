[[C++]]
```C++
#include <iostream>

class Animal {
public:
    void eat() {
        std::cout << "This animal eats food." << std::endl;
    }
};

class Dog : public Animal {
public:
    void bark() {
        std::cout << "Woof woof!" << std::endl;
    }
};

int main() {
    Dog myDog;
    myDog.eat();
    myDog.bark();
    return 0;
}

```