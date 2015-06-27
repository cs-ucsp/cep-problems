---
layout: page
title: Declaraciones Iterativas | Guía del Estudiante
---

Para que el programa pueda saber tomar decisiones, debemos utilizar declaraciones.

Las **declaraciones iterativas** (conocidas comunmente como **bucles**) repiten algún bloque de código por el número de veces que se indique, o mientras una `condición` se mantenga. Se utilizan con las palabras `while` y `for`.

- `while`: Su sintaxis es la siguiente:

``` cpp
while (condicion) {
  bloque
}
```
Donde `bloque` es ejecutado mientras la `condición` sea `true`.

#### Ejemplo

``` cpp
int n = 0;
while (n < 5) {
  cout << "n es " << n << endl;
  n = n + 1;
}
```

En el anterior ejemplo, el programa imprimirá la siguiente salida:

```
n es 0
n es 1
n es 2
n es 3
n es 4
```

Y luego terminará, ya que la variable `n` fue creciendo desde `0` hasta llegar a `5`, donde ya no cumple la `condición` del `while`.

- `for`: Su sintaxis es la siguiente:

``` cpp
for (inicializacion; condicion; incremento) {
  bloque
}
```
Muy parecido a `while`, el bucle de `for` repite el código de `bloque` mientras que `condición` sea `true`, pero `for` también ofrece poder inicializar alguna variable e indicar como irá creciendo (o decreciendo).

#### Ejemplo

``` cpp
for(int n = 0; n < 5; n++) {
  cout << " n es " << n <<endl;
}
```

El anterior ejemplo ejecuta lo mismo que el ejemplo de `while`, pero de una manera más concisa y entendible. Su salida es exactamente igual al ejemplo anterior de `while`.


<br />

[← Regresar]({{ site.baseurl }}/guide/)
