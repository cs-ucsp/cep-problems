---
layout: page
title: Instalación | Guía del Estudiante
---

Para poder programar requieres de un programa que sea capaz de entender los _algoritmos_ que diseñes.
A estos programas se los conoce como compiladores (en el caso del lenguaje de programación C++).
Estos vienen incluidos en los programas que listamos a continuación.

## Windows

Entre las alternativas de instalación tenemos:

- Visual Studio
- Eclipse
- Codeblocks
- Netbeans
- Quincy 2005

Si ya tienes algunos de los anteriores, puedes seguir el curso sin problemas. Pero para los que inician, en este curso utilizaremos el último, **Quincy 2005**, por su fácil instalación y rápido manejo.

Sigue los siguientes pasos para su instalación:

1. Descargar el programa en el siguiente link: [Click para Descargar](http://www.codecutter.net/tools/quincy/2005v1.3/Q2005v1_3setup.exe)
2. Ejecutar el programa descargado y sigue dándole `siguiente` o `next` cuando te lo pidan.

---

En cada clase que daremos, por favor abre el anterior programa (**Quincy**) para que estes listo para escribir los programas que se irá enseñando.

<br />

## Linux y Mac OSX

Si usas Windows ignora esta sección. No hay necesidad de instalación extra en Linux o Mac OSX.

<br />

## Activando C++11

### Codeblocks

1. Ir al menú `Settings` -> `Compiler...`
2. En la pestaña `Compiler Flags`, activa la opción que dice:

        Have g++ follow the C++11 ISO C++ language standard [-std=c++11]

    Nota: el mensaje puede variar un poco dependendiendo de tu versión.

3. Da click en OK

### Linux (g++)

Cuando compiles, añade la opción `-std=c++11`. Ejemplo:

    g++ archivo.cpp -std=c++11 -o ejecutable

[← Regresar]({{ site.baseurl }}/guide/)
