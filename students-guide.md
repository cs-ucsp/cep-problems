---
layout: page
title: Guia del Estudiante
permalink: /guide/
---

Esta guía resume las necesidades del estudiante para poder comenzar con los ejercicios del curso de Programación.

# Instalación

Si bien la programación va más allá del uso de una computadora, necesitamos aquella **herramienta** que hará que la computadora pueda entender los *algoritmos* que programaremos. Lo único que necesitamos es un programa que lea el _lenguaje de programación C++_.

## Windows

Entre las alternativas de instalación tenemos:

- Visual Studio
- Eclipse
- Codeblocks
- Netbeans
- Quincy 2005

Si alguien tiene alguno de los anteriores, puede seguir el curso sin problemas, pero para los que inician, en este curso utilizaremos el último, **Quincy 2005**, por su fácil instalación y rápido manejo. Seguir los siguientes pasos para su instalación:

1. Descargar el programa en el siguiente link: [Click para Descargar](http://www.codecutter.net/tools/quincy/2005v1.3/Q2005v1_3setup.exe)
2. Ejecutar el programa descargado y sigue dándole `siguiente` o `next` cuando te lo pidan.

---

En cada clase que daremos, por favor abre el anterior programa (**Quincy**) para que estes listo para escribir los programas que se irá enseñando.

<br />  
<br />  

### Linux y Mac OSX

Si usas Windows sigue al siguiente capítulo. No hay necesidad de instalación extra en Linux o Mac OSX.


# Lo Básico

Los programas (_casi todos_) que elaboraremos tendrán la siguiente estructura:

``` cpp
#include<iostream>
#include<string>
using namespace std;

int main(){
  return 0;  
}
```

Siempre que comiences un programa copia el código anterior para luego modificarlo.

### Algoritmo

Un algoritmo es una secuencia de pasos estructurados para resolver un problema. Para ello, recibe unos datos de entrada y genera una salida.

## Variable

Una _variable_ almacena datos o valores bajo un identificador o nombre.

### Tipos

El lenguaje de programación C++ requiere que se indique que _tipo_ de variable vamos a usar, las siguientes son las más comunes:

- `int`: números enteros (ejem: `1, 123, 0, -20, -4454243`).
- `float`: números con decimales (ejem: `1.0, 0.0, 53.2, -421.53225`).
- `char`: cualquier letra o símbolo en texto (ejem: `'a', '_', ' ', 'z', '6', '*'`), siempre van entre comillas simples.
- `string`: secuencia de `char`s (ejem: `"hola", "1233", "frase con espacios"`), siempre van entre comillas dobles.
- `bool`: `true` o `false`, para indicar verdad o falsedad respectivamente.

Los tipos siempre van antes de las **variable**s.

###### Ejemplo 1:

    int variable1 = 542;

En el ejemplo anterior hemos creado una _variable_ llamada `variable1`, del tipo `int` con el valor `542`.

###### Ejemplo 2:

    string variable2 = "mi frase favorita";

En el ejemplo anterior hemos creado una _variable_ llamada `variable2` del tipo `string` con el valor `"mi frase favorita"`.

###### Ejemplo 3:

    bool variable3 = true;

En el ejemplo anterior hemos creado una _variable_ llamada `variable3` del tipo `bool` con el valor `true`.

###### Ejemplo 4:

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


## Operadores
Los utilizamos todo el tiempo para interactuar con variables y modificar los valores que almacenan.

#### Asignación:
Asigna un `valor` a una `variable`. Se utiliza el signo `=`.

###### Ejemplo

  int x=5;

El anterior ejemplo asigna el valor entero `5` a la variable `x`. La asignación siempre se ejecuta de derecha a izquierda y nunca de otra manera.

    int y = 5;
    int x = y;
    int y = 2;

La variable `x` contiene el valor de `5` ya que `y` fue asignado a `x`. Al terminar el anterior ejemplo, `y` contains the value of `2`.

#### Operadores Aritméticos.

- `+`: adición.
- `-`: sustracción o resta.
- `*`: multiplicación.
- `/`: división.
- `%`: módulo o resto (de una división).

###### Ejemplo
    int x = 11 % 5;

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

###### Ejemplo

``` cpp
7 == 5    // false
5 > 3     // false
3 != 2    // true
6 >= 6    // true
5 < 5     // false
```

Estos operadores no son solo para números, y pueden ser utilizados para todos los _tipos_ antes mencionados. Ten mucho cuidado de no confundir el operador de igualdad `==` con el operador de asignación `=`.

#### Operadores Lógicos.

- `!`: negación. Convierte `true` en `false` y viceversa.

###### Ejemplo
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

## Declaraciones
Para que el programa pueda saber tomar decisiones, debemos utilizar declaraciones.

#### Declaraciones de Decisión
Utilizado para determinar si algún bloque de código debe ser ejecutado.
Se utiliza la siguiente sintaxis:

``` cpp
if (condición){
  bloque
}
```

Donde, `bloque` puede ser muchas líneas de código y `condición` es una expresión que devuelve una `bool`. Si `condición` es `true`, entonces `bloque` es ejecutado. Si `condición` es `false`, entonces `bloque` no es ejecutado.

###### Ejemplo

``` cpp
if (x < 100){
  cout<<"x es menor que 100"<<endl;
}
```

En el ejemplo anterior, el mensaje `"x es menor que 100"` es impreso si `x < 100` es `true`, lo que quiere decir que la variable `x` debe contener un valor menor que 100.

<br />  

También se puede utilizar la siguiente sintaxis para especificar que hacer si una `condición` **NO** se satisface. usando la palabra `else`:

``` cpp
if (condición){
  bloque1
}else{
  bloque2
}
```

Donde `bloque1` es ejecutado si `condición` es `true`, y `bloque2` es ejecutado si `condición` es `false`.


###### Ejemplo
``` cpp
if (x < 100){
  cout<<"x es menor a 100"<<endl;
}else{
  cout<<"x es mayor o igual a 100"<<endl;
}
```

En ejemplo ejemplo anterior, si la variable `x` contiene un valor menor a 100, entonces se imprimirá `"x es menor a 100"`, de lo contrario se imprimirá el mensaje `"x es mayor o igual 100"`.

#### Declaraciones de Iteración (Bucles)
Los bucles repiten algún bloque de código por el número de veces que se indique, o mientras una `condición` se mantenga, se utilizan con las palabras `while` y `for`.

- `while`: Su sintaxis es la siguiente:

``` cpp
while(condición){
  bloque
}
```
Donde `bloque` es ejecutado mientras la `condición` sea `true`.

###### Ejemplo

``` cpp
int n = 0;
while(n<5){
  cout<<"n es "<<n<<endl;
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
for(inicialización; condición; incremento){
  bloque
}
```
Muy parecido a `while`, el bucle de `for` repite el código de `bloque` mientras que `condición` sea `true`, pero `for` también ofrece poder inicializar alguna variable e indicar como irá creciendo (o decreciendo).

###### Ejemplo

``` cpp
for(int n=0; n<5; n++){
  cout<<" n es "<<n<<endl;
}
```

El anterior ejemplo ejecuta lo mismo que el ejemplo de `while`, pero de una manera más concisa y entendible. Su salida es exactamente igual al ejemplo anterior de `while`.


---

Con esto ya puedes estar listo para programar algunos problemas simples, asi que ahora solo resuelve los problemas y diviertete aprendiendo cada dia más. A programar!!!!
