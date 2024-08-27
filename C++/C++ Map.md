[[C++]]
```C++
#include <iostream>
#include <map>

int main() {
    std::map<std::string, int> age;
    age["Alice"] = 30;
    age["Bob"] = 25;

    for (const auto& pair : age) {
        std::cout << pair.first << " is " << pair.second << " years old." << std::endl;
    }
    return 0;
}

```