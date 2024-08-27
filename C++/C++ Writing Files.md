- [[C++]]
```C++
#include <iostream>
#include <fstream>

int main(){
	std::ofstream datei("beispiel.txt");

	if(!datei){
		std::cerr << "Fehler beim Öffnen der Datei!" << std::endl;
		return 1;
	}
	datei << "Dies ist ein Beispieltext" << std::endl;
	datei.clode();
	std::cout << "Text wurde erfolgreich in die Datei geschrieben!" << std::endl;
	return 0;
}
```