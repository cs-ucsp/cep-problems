---
layout: page
title: Operadores | Guía del Estudiante
---

Los utilizamos todo el tiempo para interactuar con variables y modificar los valores que almacenan.

## Asignación:
Asigna un `valor` a una `variable`. Se utiliza el signo `=`.

#### Ejemplo

``` cpp
int x=5;
```

El anterior ejemplo asigna el valor entero `5` a la variable `x`. La asignación siempre se ejecuta de derecha a izquierda y nunca de otra manera.

``` cpp
int y = 5;
int x = y;
int y = 2;
```

La variable `x` contiene el valor de `5` ya que `y` fue asignado a `x`. Al terminar el anterior ejemplo, `y` contains the value of `2`.

## Operadores Aritméticos.

- `+`: adición.
- `-`: sustracción o resta.
- `*`: multiplicación.
- `/`: división.
- `%`: módulo o resto (de una división).

#### Ejemplo

``` cpp
int x = 11 % 5;
```

En el ejemplo anterior, la variable `x` contiene el valor de `1` (el resto de la división entre `11` y `5`).

#### Operadores Relacionales o de Comparación.
Dos expresiones pueden ser comparadas usando estos operadores. Por ejemplo para saber si 2 valores son iguales o si uno es mayor o menor que el otro.

El resultado de tal operación es `true` o `false` (un valor `bool`).

Los operadores de comparación son los siguientes:

- `==`: igual a
- `!=`: diferente a
- `<`: menor que
- `>`: mayor que
- `<=`: menor o igual a
- `>=`: mayor o igual a

#### Ejemplo

``` cpp
7 == 5    // false
5 > 3     // false
3 != 2    // true
6 >= 6    // true
5 < 5     // false
```

Estos operadores no son solo para números, y pueden ser utilizados para todos los _tipos_ antes mencionados. Ten mucho cuidado de no confundir el operador de igualdad `==` con el operador de asignación `=`.

## Operadores Lógicos.

- `!`: negación. Convierte `true` en `false` y viceversa.

#### Ejemplo
``` cpp
!(5==5)   // false
!true     // false
!false    // true
!(6<=4)   // true
```

- `&&`: operador lógico de `y`, sigue la siguiente tabla de verdad:

| a        | b           | a && b |
| ------------- |:------:| :-----: |
| true      | true | true |
| true      | false | false |
| false      | true | false |
| false      | false | false |

- `||`: operador lógigico de `o`, sigue la siguiente tabla de verdad:

| a        | b           | a &#124;&#124; b |
| ------------- |:---------:| :-----: |
| true      | true | true |
| true      | false | true |
| false      | true | true |
| false      | false | false |


<br />

[← Regresar]({{ site.baseurl }}/guide/)
