---
name: Comandos Básicos
layout: post
post-image: /assets/images/taller/cat.png
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

| Nombre | Descripción                                                                                                            | Uso                            |
| ------ | ---------------------------------------------------------------------------------------------------------------------- | ------------------------------ |
| cat    | Imprime a la salida estándar (terminal) el contenido de un archivo                                                     | `$ cat <archivo>`              |
| head   | Imprime las primeras 10 líneas de un archivo Se puede modificar el número de líneas visibles con la opción `-n`        | `$ head -n <numero> <archivo>` |
| tail   | Imprime las últimas 10 líneas de un archivo También se puede modificar el número de líneas visibles con la opción `-n` | `$ tail -n <numero> <archivo>` |
| less   | Presenta el contenido de un archivo en un paginador                                                                    | `$ less <archivo>`             |


### Atajos en less

| Tecla | Descripción         |
| ----- | ------------------- |
| `k`   | Una línea arriba    |
| `j`   | Una línea abajo     |
| `u`   | Media página arriba |
| `d`   | Media página abajo  |
| `f`   | Una página arriba   |
| `b`   | Una página abajo    |

## Crear y escribir

| Nombre | Descripción                                                                               | Uso                              |
| ------ | ----------------------------------------------------------------------------------------- | -------------------------------- |
| touch  | Crea uno o más archivos vacíos                                                            | `$ touch <nombre>`               |
| cat    | Crea un archivo y le agrega contenido                                                     | `$ cat > <nombre>`               |
| 🖞      | Utiliza `>` para sobreescribir el contenido del archivo, y `>>` para agregar contenido    | `$ cat >> <nombre>`              |
| echo   | Envía el texto escrito a un archivo. Utiliza `>` y `>>` de la misma forma que con `cat`   | `$ echo "texto" >> <nombre>`     |
| printf | Funciona de la misma forma que `echo` pero no agrega un salto de línea al final del texto | `$ printf "texto\n" >> <nombre>` |

## Creación de directorios

| Nombre | Descripción              | Uso                |
| ------ | ------------------------ | ------------------ |
| mkdir  | Crea un directorio vacío | `$ mkdir <nombre>` |

## Manipular archivos y directorios

| Acción    | Nombre | Descripción                                           | Uso                              |
| --------- | ------ | ----------------------------------------------------- | -------------------------------- |
| Mover     | mv     | Mueve el archivo o directorio a la ruta especificada  | `$ mv <archivo> <ruta>`          |
| Renombrar | mv     | Cambia el nombre del archivo                          | `$ mv <nombre> ./<nuevo_nombre>` |
| Copiar    | cp     | Hace una copia del archivo con el mismo u otro nombre | `$ cp <archivo> <ruta>`          |
| Eliminar  | rm     | Elimina los archivos especificados                    | `$ rm <archivo>`                 |
| 🖞         | 🖞      | Elimina el directorio especificado                    | `$ rm -R <directorio>`           |


