---
layout: page
title: Declaraciones Condicionales | Guía del Estudiante
---

Para que el programa pueda saber tomar decisiones, debemos utilizar declaraciones.

Las **declaraciones condicionales** se utilizan para determinar si algún bloque de código debe ser
ejecutado o no. Se utiliza la siguiente sintaxis:

``` cpp
if (condicion) {
  bloque
}
```

Donde, `bloque` puede ser muchas líneas de código y `condición` es una expresión que devuelve un `bool`. Si `condición` es `true`, entonces `bloque` es ejecutado. Si `condición` es `false`, entonces `bloque` no es ejecutado.

#### Ejemplo

``` cpp
if (x < 100) {
  cout << "x es menor que 100" << endl;
}
```

En el ejemplo anterior, el mensaje `"x es menor que 100"` es impreso si `x < 100` es `true`, lo que quiere decir que la variable `x` debe contener un valor menor que `100`.

<br />  

También se puede utilizar la siguiente sintaxis para especificar que hacer si una `condición` **NO** se satisface. Usando la palabra `else`:

``` cpp
if (condicion) {
  bloque1
} else {
  bloque2
}
```

Donde `bloque1` es ejecutado si `condición` es `true`, y `bloque2` es ejecutado si `condición` es `false`.


#### Ejemplo
``` cpp
if (x < 100) {
  cout<<"x es menor a 100"<<endl;
} else {
  cout<<"x es mayor o igual a 100"<<endl;
}
```

En ejemplo ejemplo anterior, si la variable `x` contiene un valor menor a 100, entonces se imprimirá `"x es menor a 100"`, de lo contrario se imprimirá el mensaje `"x es mayor o igual 100"`.


<br />

[← Regresar]({{ site.baseurl }}/guide/)
