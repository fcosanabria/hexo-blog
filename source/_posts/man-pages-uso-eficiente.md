---
title: Uso eficiente de las paginas del Manual - Man Pages
date: 2021-09-19 13:30:05
tags:
- linux
categories:
- tutorial
---

Considero que para cualquier persona que se encuentre especializando y afinando su conocimiento en Linux, sabe que las Man Pages en algún momento u otro se tienen que saber usar.

Hoy vamos a aprender algunos trucos y consejos sencillos para leer las páginas de manual de forma eficaz. Como ya sabrá, una página de manual se divide en varias partes, cada una con un encabezado distinto.
Es posible que tengamos que movernos hacia abajo durante bastante tiempo cuando estemos buscando algún tipo información en particular sobre el flag u opción específica. Es una tarea realmente ineficiente y que requiere de mucho tiempo. Por eso es importante aprender a usar las páginas de manual de manera eficiente para averiguar qué es exactamente lo que deseamos saber.

Primero comencemos abriendo un man page de uno de los comandos más sencillos; `mkdir`. Para eso escribimos en la terminal:

```bash
man mkdir
```

Así se ve una página del manual para el comando de `mkdir`:

![manmkdir](https://i.imgur.com/bm59ESQ.png)

Y asi es como la mayoria de las veces se logra ver una pagina de manual, y las lineas mostradas en la captura de pantalla obedecen al comportamiento y diseno usual de las paginas del manual, cambian a para pocas excepcionies, pero usualmente asi se ven todas. 

Pero aprendamos a como leerlas, por que la sintaxis para cada una de ellas es igual para todas, y ademas tambien cumple con el formato standard de un comando basado en Unix.


## Estructura de las páginas de manual

Una pagina de manual se divide en varias secciones; usualmente dirigidas para cada seccion del manual, en donde se puede ver categorias como:

- **NAME**,
- **SYNOPSIS**,
- **CONFIGURATION**,
- **DESCRIPTION**,
- **OPTIONS**,
- **EXIT STATUS**,
- **RETURN VALUE**,
- **ERRORS**,
- **ENVIRONMENT**,
- **FILES**,
- **VERSIONS**,
- **CONFORMING TO**,
- **NOTES**,
- **BUGS**,
- **EXAMPLE**,
- **AUTHORS** y
- **SEE ALSO**.
  
Algunos man pages como comentaba ahora, suelen tener todas estas secciones y otras no, dependiendo de que tan bien esté documentado el comando referido.

Ahora analicemos lo como se tiene que leer el formato de las man pages. El formato hace que todo lo que dice las paginas del manual cobren un sentido logico. Usualmente los autores la mayoria de las veces van asumir el uso comun de los comandos en Linux y ademas de eso asumirán que sabemos como interpretar el formato, haciendo referencia a esta estrategia para poder nosotros descifrar como usar el comando, y llegar a reemplazar o complementar los valores, argumentos o flags requeridas.
