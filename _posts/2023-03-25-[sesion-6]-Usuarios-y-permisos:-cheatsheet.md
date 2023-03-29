---
name: Usuarios y permisos
layout: post
post-image: /assets/images/taller/usuarios_permisos.png
description: En esta sesión se explicó qué son los permisos en Linux y cómo se interpretan, así como la manera de cambiarlos.
tags: Linux Taller Shell Comandos
---

# Sesión
<iframe width="560" height="315" src="https://www.youtube.com/embed/gxGa23qs4qk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

---
# Temas vistos
- HTB Academy: Filter Contents (Tema 5)
- Permisos (Tema 6)
- Cambiar permisos (Tema 6)

---
# Cheatsheet
## HTB Academy: Filter Contents

| Comando | Descripción                                                                                                             |
| ------- | ----------------------------------------------------------------------------------------------------------------------- |
| netstat | Muestra las conexiones de red del sistema                                                                               |
| ps      | Muestra los procesos activos en el sistema                                                                              |
| curl    | Transfiere información desde o hacia un servidor. Si sólo se especifica una url, obtendrá el código fuente de la página |


## Permisos
### Usuario y permisos

| Letra | Significado         | Valor numérico |
| ----- | ------------------- | -------------- |
| r     | read (lectura)      | 4              |
| w     | write (escritura)   | 2              |
| x     | execute (ejecución) | 1               |

| Letra | Se refiere a...                                               |
| ----- | ------------------------------------------------------------- |
| u     | El usuario dueño del archivo (generalmente quien lo creó)     |
| g     | Los usuarios que pertenecen al grupo que posee el archivo     |
| o     | Todos los usuarios que no caen en las dos primeras categorías |

### Mostrar permisos

| Comando        | Descripción                                              |
| -------------- | -------------------------------------------------------- |
| ls -l          | Muestra los permisos de todos los archivos especificados |
| stat \<archivo> | Muestra los permisos del archivo en formato numérico     |

### Cambiar permisos
```shell-session
$ chmod u+rx-w,g+rx-w,o+x-rw <archivo>
$ chmod 551 <archivo>
``` 
<br>

---
<blockquote class="reddit-embed-bq" data-embed-theme="dark" data-embed-height="500">      <a href="https://www.reddit.com/r/vpnnetwork/comments/11dnsb7/touch_cannot_touch_woman_access_denied/">Touch: cannot touch 'woman' access denied</a><br> by      <a href="https://www.reddit.com/user/SpaceyAndrew">u/SpaceyAndrew</a> in      <a href="https://www.reddit.com/r/vpnnetwork/">vpnnetwork</a>    </blockquote><script async="" src="https://embed.reddit.com/widgets.js" charset="UTF-8"></script>
