---
layout: page
title: Vectores | Guía del Estudiante
---

¿Qué hacemos si nuestro programa requiere como entrada varios datos? Si son cinco, podríamos
hacer algo como:

``` cpp
int a1, a2, a3, a4, a5;
```

¿Y si necesitáramos diez o cien o un millón? Podemos ver que esta estrategia no escala. Además,
¿como podríamos obtener el valor de un elemento arbitrario? Podemos acceder al primer elemento con
la variable `a1`, el cuarto con la variable `a4`. Pero... ¿qué hay de un elemento "`i`-ésimo"?

Para resolver estos problemas introducimos una de las
[estructuras de datos](https://es.wikipedia.org/wiki/Estructura_de_datos) más simples: el vector o
arreglo.

## ¿Qué es?

Un vector nos permite tener una cantidad variable de datos indexados por números enteros no
negativos, de tal forma que podemos expresar cosas como "primero", "último", "quinto", "elemento
anterior", "elemento siguiente", "elemento subsiguiente", etc.

## Uso

### Requisitos previos

Para poder usar vectores debemos incluir su librería:

``` cpp
#include <vector>
```

En cualquier lugar antes de la línea

``` cpp
using namespace std;
```

Nota importate: Algunas de las operaciones que vamos a realizar son características nuevas de C++.
Para poder usarlas debes activarlas. Para ello, puedes
[ver la guía]({{ site.baseurl }}/guide/installation.html#activando-c-11).

### Declaración

Un vector puede almacenar cualquier tipo de dato, lo que se especifica en su declaración:

``` cpp
vector<int> v1;  // un vector vacío
vector<float> v2(3);  // un vector de 3 decimales con valor 0
vector<char> v3(6, 'a');  // un vector de 6 caracteres 'a'
vector<int> v3{5, 6, 8, -1, 0};  // un vector con los elementos especificados
```

Revisa atentamente los ejemplos anteriores para entender cuándo usar paréntesis y cuándo llaves.

### Acceso a elementos

Como se mencionó anteriormente, los datos son indexados por enteros no negativos (de cero a más):

``` cpp
vector<int> v{54, 56, 9, 23, -5, 45, -16, 12, -23};
v[0] = 5;  // asignamos el valor de 5 al primer elemento
int a = v[7];  // asignamos el octavo elemento a la variable a
v[8] = v[3];  // el noveno elemento toma el valor del tercer elemento
cin >> v[2];  // leemos el tercer elemento
cout << v[8];  // imprimimos el noveno elemento
```

Nuevamente, los datos se indexan comenzando con cero (0). También podemos acceder a posiciones
variables:

``` cpp
vector<int> v(20);
v[0] = 1;
v[1] = 1;
for (int i = 2; i < 20; ++i) {
  v[i] = v[i-1] + v[i-2];
}
```
¿Puedes deducir qué hace este programa?

También tienes disponibles los siguientes accesos rápidos:

``` cpp
v.front();  // primer elemento, equivalente a v[0]
v.size();   // devuelve el tamaño del vector
v.back();  // último elemento, equivalente a v[v.size() - 1]
```

**¡Vamos, intenta modificar y ejecutar los ejemplos que has visto hasta ahora!**

¿Cómo podrías leer desde teclado todos los elementos de un vector? ¿Qué hay de imprimirlos en
la pantalla?

Pista: _Usa un bucle `for` con una instrucción `cin` o `cout` dentro_.

### Modificando el vector

Ya has visto que usando corchetes puedes leer y modificar elementos específicos del vector. ¿Será
posible variar su tamaño?

``` cpp
vector<int> v{3, -2, 0};
v.push_back(5);  // añade el valor 5 al final: {3, -2, 0, 5}
v.resize(10);  // ahora el vector tiene tamaño 10
v.pop_back();  // eliminamos el último elemento (y el vector tiene tamaño 9)
```

Eso es todo (por ahora)... una enorme cantidad de problemas esperan ser resueltos por ti :)

Dos preguntas finales: ¿será posible hacer un vector de vectores? ¿Qué utilidad podría tener?

<br>
<hr>

Nota: Existe una forma más tradicional de declarar arreglos. Puedes leer sobre ella más
[aquí](http://c.conclase.net/curso/?cap=010), pero el concepto de vector que hemos revisado te
resultará más fácil de manejar.

[← Regresar]({{ site.baseurl }}/guide/)
