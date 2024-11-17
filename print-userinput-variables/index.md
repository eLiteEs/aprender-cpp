## 2. Imprimir

Para imprimir texto, usas la "función" `cout` y los carácteres `<<` (Que significan output de texto, una forma clara de entenderlo es que si las flechas van a la izquierda, el programador le dice algo a la máquina y al revés la máquina le dice algo al programador).
Ejemplo:
```std::cout << "Hello World!";```

Una cosa, si directamente en el archivo de C++ pones eso, no se va a ejecutar correctamente, ya que en C++ tienes que poner una función `main` en el archivo, como en Java . Asi que el archivo quedaría algo así:
```
// Importar una librería de C++
#include <iostream>

// Función que se ejecuta por defecto en el programa
int main() {
    // El código que se ejecuta en el programa
    std::cout << "Hello World!" << std::endl;
}
```
Las líneas del código acaban en `;`. Y hay una forma de escribir eso más rápido, en ese código puedes ver que antes de `cout` y `endl` está el texto `std::`, se puede quitar poniendo antes del `int main` `using namespace std;`. Y quedaría algo así:
```
#include <iostream>

// Usar la librería de C++ std
using namespace std;

int main() {
    cout << "Hello World!" << endl;
}
```