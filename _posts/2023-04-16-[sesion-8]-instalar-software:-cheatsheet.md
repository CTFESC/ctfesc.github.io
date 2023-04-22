---
name: Instalar software
layout: post
post-image: /assets/images/taller/apt.png
description: En esta sesión revisamos algunos de los métodos más populares para instalar software en Linux, concretamente en distribuciones basadas en Debian.
tags: Linux Software Comandos
---

# Sesión
<iframe width="560" height="315" src="https://www.youtube.com/embed/S1NuNzN6g8w" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

---
# Temas vistos
- apt
- flatpak
- appimages

---
# Cheatsheet

## apt

Todos los siguientes comandos (con excepción de `search`) requieren el `sudo`. Los comandos `apt` y `apt-get` son equivalentes.

| Acción                                 | Comando                          |
| -------------------------------------- | -------------------------------- |
| Actualizar repos                       | apt update                       |
| Buscar paquete                         | apt search \<paquete>            |
| Instalar                               | apt install \<paquete>           |
| Instalar un paquete `.deb`             | apt install /ruta/al/paquete.deb |
| Desinstalar sin eliminar dependencias  | apt remove \<paquete>            |
| Desinstalar junto con las dependencias | apt purge \<paquete>             |
| Eliminar dependencias sin uso          | apt autoremove                   |
| Actualizar los paquetes instalados     | apt upgrade                      |


## flatpak

### Instalación

```shell-session
$ sudo apt install flatpak
$ flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
```

Para instalar una aplicación, una vez **reiniciado** el equipo, copiar el comando que se proporciona en el [Hub de applicaciones](https://flathub.org/). Ejemplo para instalar spotify:

```shell-session
$ flatpak install flathub com.spotify.Client
```

## appimages

Una vez descargado el archivo `.AppImage` es necesario darle permisos de ejecución para poder usar el programa:

```shell-session
$ chmod +x archivo.AppImage
$ ./archivo.AppImage
```
<br>
Para integrar el `.AppImage` en el sistema se necesita un launcher, este fue desarrollado por [TheAssassin](https://github.com/TheAssassin/AppImageLauncher/releases). Una vez instalado, cada vez que se abra una appimage nueva, preguntará si queremos integrarlo en el sistema.

---

<blockquote class="reddit-embed-bq" style="height:500px" data-embed-theme="dark" data-embed-height="500">      <a href="https://www.reddit.com/r/linuxmemes/comments/r1heh0/for_extra_brrrr_i_use_apt_list_upgradable/">For extra brrrr., I use apt list --upgradable</a><br> by      <a href="https://www.reddit.com/user/thehotshotpilot">u/thehotshotpilot</a> in      <a href="https://www.reddit.com/r/linuxmemes/">linuxmemes</a>    </blockquote><script async="" src="https://embed.reddit.com/widgets.js" charset="UTF-8"></script>

