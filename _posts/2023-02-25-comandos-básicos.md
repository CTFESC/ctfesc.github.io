---
name: Comandos Básicos
layout: post
post-image: /assets/images/cat.png
description: Uso de comandos para la manipulación de archivos y directorios. Se demuestra el funcionamiento de comandos con los que podemos ver el contenido de un archivo, crear archivos nuevos y darles contenido, así como mover, renombrar, copiar y eliminar archivos y directorios desde la terminal.
tags: Comandos Taller Terminal Administración Linux
---

# Sesión
<iframe width="560" height="315" src="https://www.youtube.com/embed/3mrvgfN8r7g" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

---
# Temas vistos
- Manipulación de archivos y directorios
- Práctica de comandos básicos

---
# Cheatsheet

## Leer
### cat
Imprime a la salida estándar (terminal) el contenido de un archivo.
```shell-session
$ cat <archivo>
```

### head
Imprime a la salida estándar las primeras 10 líneas de un archivo. Se puede modificar el número de líneas visibles con la opción `-n`.
```shell-session
$ head <archivo>
$ head -n 20 <archivo>
```

### tail
Imprime a la salida estándar las últimas 10 líneas de un archivo. Al igual que con `head`, se puede modificar el el número de líneas visibles con la opción `-n`.
```shell-session
$ tail <archivo>
$ tail -n 20 <archivo>
```

### less
Presenta el contenido de un archivo en un paginador.
```shell-session
$ less <archivo>
```

Utiliza las teclas `k` y `j` para moverte una línea hacia abajo y una línea hacia arriba, respectivamente. Utiliza las teclas `d` y `u` para desplazarte media página abajo o media página arriba, y utilizar `f` y `b` para desplarte una página arriba y una página abajo, respectivamente.

## Crear y escribir
### touch
Crea uno o más archivos vacíos.
```shell-session
$ touch <archivo>
```

### cat
Se puede redireccionar la salida de `cat` hacia un archivo.
Utiliza `>` para sobreescribir el contenido del archivo, y `>>` para agregar contenido.

```shell-session
$ cat >> <archivo>
Este archivo fue creado usando cat.
^C
```

### echo y printf
Se puede redireccionar el texto que echo y printf nos devuelve hacia un archivo.
```shell-session
$ echo "Archivo creado con echo" >> <archivo>

$ printf "Archivo creado con printf" >> <archivo>
```

## Creación de directorios
### mkdir
Crea un directorio vació.
```shell-session
$ mkdir nuevo-directorio
```

## Manipular archivos y directorios
### Mover y renombrar
Mueve el archivo o directorio a la ruta especificada, si se especifica la misma ruta, el archivo cambiara de nombreal indicado.
```shell-session
$ mv <archivo> <nueva ruta>  # mover
$ mv <archivo-viejo> ./<archivo-nuevo>  # renombrar
```

### copiar
Hace una copia del archivo en la ruta especificada.
```shell-session
$ cp <archivo> <ruta>
```

### Eliminar
Elimina el o los archivos especificados. Agrega la opción -R para eliminar directorios. **Cuidado**, esta acción no se puede deshacer.
```shell-session
$ rm <archivo>
$ rm -R <directorio>
```


