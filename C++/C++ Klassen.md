[[C++]]
```C++
#include <iostream>

class Car {
public:
    std::string brand;
    void honk() {
        std::cout << "Beep beep!" << std::endl;
    }
};

int main() {
    Car myCar;
    myCar.brand = "Toyota";
    myCar.honk();
    std::cout << "Brand: " << myCar.brand << std::endl;
    return 0;
}

```