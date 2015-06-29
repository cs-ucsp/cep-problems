---
layout: page
title: Variables | Guía del Estudiante
---

Una _variable_ almacena datos o valores bajo un identificador o nombre.

# Tipos

El lenguaje de programación C++ requiere que se indique que _tipo_ de variable vamos a usar, las siguientes son las más comunes:

- `int`: números enteros (ejem: `1, 123, 0, -20, -4454243`).
- `float`: números con decimales (ejem: `1.0, 0.0, 53.2, -421.53225`).
- `char`: cualquier letra o símbolo en texto (ejem: `'a', '_', ' ', 'z', '6', '*'`), siempre van entre comillas simples.
- `string`: secuencia de `char`s (ejem: `"hola", "1233", "frase con espacios"`), siempre van entre comillas dobles.
- `bool`: `true` o `false`, para indicar verdad o falsedad respectivamente.

Los tipos siempre van antes de los nombres de las variables.

#### Ejemplo 1:

``` cpp
int variable1 = 542;
```

En el ejemplo anterior hemos creado una _variable_ llamada `variable1`, del tipo `int` con el valor `542`.

#### Ejemplo 2:

``` cpp
string variable2 = "mi frase favorita";
```

En el ejemplo anterior hemos creado una _variable_ llamada `variable2` del tipo `string` con el valor `"mi frase favorita"`.

#### Ejemplo 3:

``` cpp
bool variable3 = true;
```

En el ejemplo anterior hemos creado una _variable_ llamada `variable3` del tipo `bool` con el valor `true`.

#### Ejemplo 4:

``` cpp

int mi_numero = 5;
int mi_segundo_numero = 34;
bool terrible_mentira = mi_numero == mi_segundo_numero;
bool tremenda_verdad = 8.5 < 50.3;
```

El ejemplo anterior es más sofisticado, hemos creado 4 variables.

1. `mi_numero`: de tipo `int` con el valor `5`.
2. `mi_segundo_numero`: de tipo `int` con el valor `34`.
3. `terrible_mentira`: de tipo `bool` que almacena la comparación de igualdad (`==`) entre las variables `mi_numero` y `mi_segundo_numero`.
4. `tremenda_verdad`: de tipo `bool` que almacena la comparación de menor (`<`) entre los `float` `8.5` y `50.3`.

Aqui podemos darnos cuenta que el resultado de `terrible_mentira` es `false` y `tremenda_verdad` es `true`.

<br />

[← Regresar]({{ site.baseurl }}/guide/)
