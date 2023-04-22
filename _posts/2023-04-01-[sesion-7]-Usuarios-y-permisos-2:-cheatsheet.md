---
name: Usuarios y permisos II
layout: post
post-image: /assets/images/taller/sudo.png
description: En esta sesión terminamos el tema Usuarios y Permisos. Se explica cuál es la diferencia entre un usuario normal y el usuario root y cómo podemos utilizar su poder dentro de un sistema Linux. Además se resuelve una máquina de Try Hack Me para repasar lo visto.
tags: Linux Usuarios Permisos Máquinas CTF
---

# Sesión
<iframe width="560" height="315" src="https://www.youtube.com/embed/_jfcJDkVqFk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

---
# Temas vistos
- Usuario root
- Sudo
- THM: Pickle Rick [máquina]

---
# Cheatsheet

## Usuario root

```shell-session
$ sudo su
password:

$ whoami
root
```

## sudo

```shell-session
$ sudo <comando>
$ sudo whoami
$ sudo cat /etc/shadow
```

Comprobar nuestra capacidad de uso de `sudo`:
```shell-session
$ sudo -l
```


## Try Hack Me

### nmap
```shell-session
$ nmap <ip>
$ nmap localhost  # analizar los puertos locales
$ nmap inlanefreight.com  # sitio de prueba
```

---

