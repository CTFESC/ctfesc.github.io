---
name: Introducción a Linux
layout: post
post-image: /assets/images/Estructura_Linux.png
description: Introducción a la interfaz de Parrot OS, la shell y a comandos básicos. También se explica cómo se utilizan las rutas absolutas y relativas con comnados para movernos por el sistema desde la terminal.
tags: Taller Comandos Introducción Terminal Shell
---

# Sesión
<iframe width="560" height="315" src="https://www.youtube.com/embed/H6OepWNnRMc?start=58" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

---
# Temas vistos
- La Shell
- Prompt
- Estructura de Linux
- Rutas
- Comandos elementales
- Encontrar ayuda

---
# Cheatsheet

## Comandos ilustrativos
### Fecha
Muestra la fecha y hora en la que fue ejecutado el comando.
```shell-session
$ date
```

### Usuario actual
Muestra quién es el usuario que ejecutó el comando.
```shell-session
$ whoami
```

### bc
_basic calculator_

Ejecuta una calculadora interactiva desde la terminal.
```shell-session
$ bc
```

### cat
Duplica el mensaje escrito.
```shell-session
$ cat
```


### free
Muestra información actual sobre la memoria RAM.
```shell-session
$ free
```


### Procesos
Lista los procesos que se están ejecutando en el sistema.
```shell-session
$ top
$ htop
```

### Características del sistema
Muestra el logo de la distribución y las características del sistema.
```shell-session
$ neofetch
```

## Comandos de movimiento
### pwd
_present working directory_

Nos dice en dónde nos encontramos actualmente

```shell-session
$ pwd
```
### ls
_list_

Muestra el contenido de un directorio

```shell-session
$ ls
```

### cd
_change directory_

Cambia de directorio de trabajo

```shell-session
$ cd <ruta>
```

### tree
Muestra el contenido de un directorio en formato de arbol

```shell-session
$ tree <ruta>
```

---
## Comandos de ayuda
### Ayuda rápida
Muestra una breve descripción del comando y sus múltiples opciones. Si la opción `-h` no da resultados, utiliza `--help`.
```shell-session
$ <comando> -h
$ <comando> --help
```

### Ayuda detallada
Muestra toda la información del comando, su utilización y todas la opciones disponibles para ese comando.
```shell-session
$ man <comando>

q  # salir
```


<br>

<iframe id="reddit-embed" src="https://www.redditmedia.com/r/linuxmemes/comments/jqca9u/classic_linux/?ref_source=embed&amp;ref=share&amp;embed=true&amp;theme=dark" sandbox="allow-scripts allow-same-origin allow-popups" style="border: none;" height="528" width="640" scrolling="no"></iframe>

