---
name: Introducción a CTF
layout: post
post-image: /assets/images/taller/ctf.png
description: En esta sesión se presentó la introducción a CTF (Capture The Flag), una modalidad trasladada de los videojuegos al pentesting y que nos sirve como método de aprendizaje y práctica. Así mismo, se resolvieron algunos niveles de los laboratorios Bandit, y la primer máquina de Try Hack Me.
tags: Máquinas CTF Linux Pentesting Cheatsheet
---

# Sesión

🟡 **Revisa la sección de aclaraciones** para algunas correcciones en el vídeo.

<iframe width="560" height="315" src="https://www.youtube.com/embed/FSB9-uzHjsE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## Aclaraciones de la sesión
- La respuesta que se ingresa en la pregunta de la _Task 1_ es la frase que se muestra en el panel, no el balance de la cuenta.

---

# Temas vistos
- ¿Qué es CTF?
- Overthewire: Bandit (0-4)
- Try Hack Me: Hack FakeBank

---
# Cheatsheet
## Linux

### cat
Mostrar contenido de archivos que su nombre comienza con `-`.

```shell-session
$ cat ./-
$ cat <ruta_absoluta>/-
```
<br>
Mostrar contenido de archivos con espacios en el nombre.
```shell-session
$ cat spaces\ in\ this\ filename
$ cat "spaces in this filename"
```

### ls
Listar archivos ocultos.

```shell-session
$ ls -a
$ ls -A
```

### file
Muestra el tipo de archivo.
```shell-session
$ file <archivo>
```

## Redes

### openvpn
Realiza la conexión a una VPN a través de un archivo de configuración `.ovpn`.

```shell-session
$ sudo ovpn <archivo>.ovpn
```


### ping
Realiza una prueba de alcance entre la máquina y un host remoto.
```shell-session
$ ping <host>
$ ping 1.1.1.1
$ ping parrotsec.org
```

## Pentesting

### gobuster
```shell-session
$ gobuster <modo> -u <url> -w <wordlist>
$ gobuster dir -u http://10.10.20.10 -w rockyou.txt
$ gobuster -u http://fakebank.com -w wordlist.txt dir
```

---

# Proceso de CTF ilustrado
![Proceso de CTF](/assets/images/taller/ctf.png)

