---
name: Editores de Texto
layout: post
post-image: /assets/images/taller/vim.png
description: En esta sesión revisamos las distintas opciones disponibles en Parrot para editar archivos de texto, tanto editores gráficos como editores en la terminal, y repasamos lo visto en la sesión configurando y personalizando nuestra terminal.
tags: Personalización Taller Terminal bashrc Cheatsheet
---

# Sesión

🟡 **Revisa la sección** de abajo respecto a las **correcciones de la sesión** para solucionar lo que quedó pendiente en el vídeo.

<iframe width="560" height="315" src="https://www.youtube.com/embed/H7AxaWqr6M8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## Correcciones de la sesión
- `vimtutor` sí está disponible en español, sigue estos pasos para utilizarlo. El tutor no es interactivo (no te pone los taches y las palomitas):
    1. Ejecuta `sudo apt install vim-runtime`
    2. Ejecuta `vim /usr/share/vim/vim82/tutor/tutor.es.utf-8`. (Puede ser que _`vim82`_ tenga otro nombre, depende de la versión de `vim`, ej. `vim76`, `vim80`, etc.).

- La ruta para los **color-schemes** es: `~/.local/share/konsole/` 

---
# Temas vistos
- Editores de texto gráficos
- Editores de texto en la terminal
- Personalizar la terminal

---
# Cheatsheet
## nano

Uso:
```shell-session
$ nano <archivo>
```

### Teclas

| Acción        | Teclas       |
| ------------- | ------------ |
| Salir         | `Ctrl` + `X` |
| Buscar        | `Ctrl` + `F` |
| Reemplazar    | `Ctrl` + `R` |
| Ir a la línea | `Ctrl` + `G` |
| Deshacer      | `Ctrl` + `Z` |
| Rehacer       | `Ctrl` + `Y` |

## vim
**Sólo se listan las acciones vistas en la sesión**. Para un cheatsheet más completo, visita: [Vim cheatsheet](https://devhints.io/vim).

### Modos

| Modo               | Tecla     |
| ------------------ | --------- |
| Normal (comandos)  | `Esc`     |
| Inserción          | `I` ó `A` |
| Visual (selección) | `V`       |

### Modo normal

| Acción                         | Teclas o comando       |
| ------------------------------ | ---------------------- |
| Salir                          | `:q`                   |
| Salir y guardar                | `:wq`                  |
| Salir sin guardar              | `:q!`                  |
| Mover el cursor arriba         | `k`                    |
| Mover el cursor abajo          | `j`                    |
| Mover el cursor a la izquierda | `h`                    |
| Mover el cursor a la derecha   | `l`                    |
| Eliminar línea                 | `dd`                   |
| Deshacer                       | `u`                    |
| Rehacer                        | `Ctrl` + `r`           |
| Pegar desde el portapapeles    | `Ctrl` + `Shift` + `v` |

<br>
<iframe id="reddit-embed" src="https://www.redditmedia.com/r/vim/comments/hgowyf/quit_now/?ref_source=embed&amp;ref=share&amp;embed=true&amp;theme=dark" sandbox="allow-scripts allow-same-origin allow-popups" style="border: none;" height="489" width="640" scrolling="no"></iframe>
