+++
author = "Mauricio Saavedra"
title = "Usando MarkDown"
date = "2022-09-16"
description = "Traduciendo y probando MarkDown"
tags = [
    "MarkDown",
    "Practica",
]
+++

<!--Para poner una cabecera con MarkDown ocupamos los #, un signo es igual al número en los h1, si queremos un H6 ocupamos ###### Así, pero solo ocuparé uno-->
# Aprendiendo de MarkDown
### Estos son los clásicos H's de HTML, a continuación un paragrafo:

<!--Para escribir un paragrafo solo hace falta escribirlo:-->
El aprendizaje de HUGO ha sido bastabte entretenido, lo más importante es ver las fuentes primero del tirón, y luego con estas nociones ir viendo fuentes y avanzando, ya después me lanzó a hacer las cosas por mi cuenta a la vez que voy viendo cambios para saber como es que funcionan las cosas.

<!--Ahora veré los BLOCKQUOTES, y de paso veremos como usar *cursiva* y **negritas**, asi como el remarcado de las palabras foote, que se hace con las comas inversas: ``-->
#### Blockquotes:
Blockquotes: el elemento *blockquote* representa contenido que se cita de otra fuente; opcionalmente con una cita que debe estar dentro de un pie de página (`footer`) o elemento de cita (`cite`), y opcionalmente con cambios en línea como anotaciones y abreviaturas.

#### Blockquote sin atribución:

> Para esto únicamente estamos empezando la línea del paragrafo con >.

<!--Este es un apartado importante, pues mem sería de mucha ayuda para poner citas de autores o películas:-->
#### Blockquote con atribución:

>  las historias son una herramienta poderosa que nos ha permitido ser lo que actualmente somos como especie, podríamos decir que para eso y por eso contamos historias.<br>
> — <cite>Marina Golondrina[^1]</cite>

[^1]: El texto de arriba esta tomado de Marina Golondrina, de su [video](https://www.youtube.com/watch?v=47WyabHczVk&list=FLCpnQbC0cBTMD92_jMRWwPg&index=37) One Piece | Ussop y el valor de la fincción, 2021.

## Tablas

Realmente no hay tablas en MakDown, pero HUGO las soporta fuera de la casa.

   Libro    | Páginas
------------|------
   Morbo->  | 200
 ¿¿¿??? ->  | 250

## Bloques de Código
<!--Hay tres maneras de poner el código:
1.-Con fondo negro, usando triples comas invertidas:
```Ponemos el lenguaje
salto de línea y el código```
2.- Sin el fondo negro únicamente vamos escribiendo el código pero con tabulador a cada renglón.
3.-
-->
#### Bloque de código con fondo negro:

```python
#Vamos a hacer la serie de Fibonacci:
a, b, c = 0, 1, int(input("Favor de poner un número que detenga la serie: "))
while a < c:
    print(a)
    a, b = b, a+b
```
#### Bloque de Código con el resaldado interno de HUGO:
{{< highlight python >}}
a, b, c = 0, 1, int(input("Favor de poner un número que detenga la serie: "))
while a < c:
    print(a)
    a, b = b, a+b
{{< /highlight >}}
Por fuera no hay diferencia, pero por dentro lo que cambia es él como se le avisa a HUGO y a MarkDown lo que deben de procesar.

## Tipos de lista

#### Ordenada:

1. Socrates
2. Aristocles (Platón)
3. Aristoteles

#### Desordenada:

* Leche
* Jamón
* Pan de caja

#### Identada:

* Frutas:
  * Manzana
  * Naranja
  * Platanos
* Higiene:
  * Jabón
  * Crema
  * Shampoo

Aparecen otros elementos pero parecen no funcionar muy bien, así que veré si ha habido actualizaciones para ponelos yo.