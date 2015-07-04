---
layout: post
title:  "Juego de palabras"
categories: fácil matemática estructura-de-datos fuerza-bruta
---

## Problema

A Cesar le gusta jugar con las palabras y, dada una palabra, quiere saber cuántas diferentes palabras se pueden generar si añadimos exactamente una letra del alfabeto internacional (todas las 26 letras entre la _a_ y la _z_, en este caso omitimos la _ñ_) en cualquier lugar de la palabra.

Las palabras de Cesar generalmente carecen de sentido, así que si el está jugando con la palabra `"a"` se pueden formar las siguientes palabras: `"ab", "ac", ..., "az", "ba", "ca", ..., "za"`, y '"aa"', produciendo 51 palabras distintas.

### Entrada

La entrada es una palabra $s$ ($1 \leq |s| \leq 20$). La palabra $s$ es una cadena formada únicamente por caracteres minúsculos del alfabeto internacional.

### Salida

Número de palabras que podrían ser generadas.

## Ejemplo
#### Entrada
```
a
```
#### Salida
```
51
```

## Ejemplo
#### Entrada
```
ja
```
#### Salida
```
76
```