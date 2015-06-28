---
layout: post
title:  "Es este el problema más fácil"
categories: fácil matemática
---


Un triángulo es una figura geométrica con tres lados positivos. Sin embargo, cualquiera de los tres lados dados no necesariamente forman un triángulo. Los tres lados deben formar una región cerrada. Los triángulos se clasifican en función de los valores de los lados. En este problema se les requiere determinar el tipo de triángulo.

### Entrada

La primera línea de entrada contendrá un número entero positivo $T < 20$, donde T denota el número de casos de prueba. Cada una de las siguientes líneas $T$ contendrá tres enteros de 32 bits con signo.

### Salida
Para cada caso de entrada habrá una línea de salida. Se formatea como:

    Case x: "Tipo de triángulo".

Donde `x` denota el número de caso y `Tipo de triángulo` será uno de los siguientes valores:

- `Invalid` - Los tres lados no pueden formar un triángulo
- `Equilateral` - Los tres lados del triángulo son iguales.
- `Isosceles` - Exactamente dos de los lados de un triángulo son iguales.
- `Scalene` - Sin par de lados iguales.

## Ejemplo

### Entrada

    4
    1 2 5
    1 1 1
    4 4 2
    3 4 5

## Salida

    Case 1: Invalid  
    Case 2: Equilateral  
    Case 3: Isosceles  
    Case 4: Scalene  
