## 1. Instalar C++ y usarlo en Visual Studio Code (En Windows)

Aquí vas a aprender a como instalar C++ y usarlo en Visual Studio Code. Usarás Visual Studio Code para editar código C++.

1. Instalar Visual Studio Code. Ve a [https://code.visualstudio.com/Download](https://code.visualstudio.com/Download) y seleciona tu versión adecuada.
2. Una vez tengas instalado Visual Studio Code, descarga esto https://github.com/msys2/msys2-installer/releases/download/2024-01-13/msys2-x86_64-20240113.exe que es una terminal que usaremos para instalar C++.
3. Cuando termines de instalar `msys2`, en su terminal ejecuta el comando `pacman -S --needed base-devel mingw-w64-ucrt-x86_64-toolchain`, el cual instala C++ en tu ordenador.
4. Cuando ejecutes ese comando pulsa `enter` para instalar todas las `packages` y pulsa `Y` cuando te pregunte si seguir con la instalación.
5. Una vez haya terminado de instalarse es necesario que añadas los ejecutables a la variable `PATH` de Windows. En el buscador del menú de inicio, pon `Editar las variables de entorno del sistema`. Posiblemente necesites tener permisos de administrador para editar esa variable. Se te abre una ventana y abajo hay un botón que dice `Variables de entorno...`. Púlsalo y en la lista de abajo te salen las variables para todos los usuarios, ahí busca una variable llamada `PATH`, seleccionala y pulsa el botón `Editar...`. Haz click en el botón `Nuevo` y pega el directorio donde se instaló C++, normalmente `C:\msys64\ucrt64\bin\`.
6. Una vez hayas terminado de instalar y configurar C++ en tu ordenador, en `cmd` por ejemplo pon el comando `g++ --version` para revisar que se configuró correctamente, si no funciona considera repetir el proceso de nuevo.
7. Ahora en Visual Studio Code, inicialo y en el panel lateral izquierdo busca un ícono con cuatro cuadrados, que es un lugar donde instalar extensiones. Ahí busca una extension que se llama `C/C++`. Instalala y tambíen instala otra que se llama `Code Runner` que sirve para compilar y ejecutar archivos rápidamente.
8. Si todo ha ido bien deberías poder usar C++ en Visual Studio Code. Para comprobarlo, crea un archivo pulsando `Control`+`N` y en el escribe lo siguiente: 
```
#include <iostream>

int main() {
    std::cout << "Hello World!" << std::endl;

    return 0;
}
```
Para ejecutarlo, en la esquina superior derecha, hay un icono con el símbolo de play, su lo pulsas se te ejecuta el archivo con el resultado en la terminal `Hello World!`.

Siguiente: [Imprimr, User Input y Variables](https://github.com/eLiteEs/aprender-cpp/blob/main/print-userinput-variables/index.md)