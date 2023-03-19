---
name: Búsquedas
layout: post
post-image: /assets/images/taller/codigos_salida.png
description: En esta sesión se muestran las diferentes formas con las que se puede filtrar información cuando se busca algo específico en archivos y directorios.
tags: Bandit Comandos Linux Taller CTF
---

# Sesión
<iframe width="560" height="315" src="https://www.youtube.com/embed/-izu5zbHVjs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

---
# Temas vistos
- Pipes
- Filtrar información
- Wildcards
- Más bandit

---
# Cheatsheet
## Comandos

### pipes
Nos permiten redireccionar la salida o entrada estándar de un comando y redirigirlo a otro comando. Se representan con el símbolo `|`.

```shell-session
$ comando1 | comando2
$ fortune | cowsay
$ echo "cuántas palabras hay en esta oración?" | wc -c
```

### grep
Busca una palabra/patrón en un texto.

```shell-session
$ grep -i "Gerardo" rockyou.txt
$ ls --help | grep "sort" 
```

### wildcards
Son símbolos que tienen un significado especial para los sistemas Linux.

| Símbolo | Significado             |
| ------- | ----------------------- |
| `*`     | Todos los carácteres    |
| `?`     | Un carácter             |
| `[]`    | Un conjunto de caráctes |

#### Ejemplo
Ruta: `/usr/share/wordlists/SecLists/Miscellaneous/security-questions-answers/us-colleges`

```shell-session
$ ls -l A*  # colegios que empiezan con A
$ ls -l M?ss*  # colegios que empiezan con M, tienen un caracter cualquiera y continuan con ss
$ ls -l [GH]*  # colegios que empiezan con G ó H
```

### find
Busca los archivos o directorios que coincidan con los filtros establecidos.

```shell-session
$ cd /usr/share/wordlists/
$ find ./ -type f -name *sql*  # busca una wordlist para sql
$ find ./ -type f -name *sql*.txt -size -1000c -exec less {} \;  # busca una wordlist para php
```

### sort & uniq
Ordena (`sort`) y encuentra las líneas únicas (`uniq -u`).

```shell-session
$ sort data.txt | uniq -u
```

### tr
Modifica cadenas de texto, eliminando, cambiando o agregando carácteres.
```shell-session
$ echo "aaabbbccc" | tr "a" "x"
$ echo "aaabbbccc" | tr [abc] [xyz]o

# cifra caesar
$ echo "mensaje no cifrado" | tr [a-wx-z] [d-za-c] > cifra_caesar.txt
$ cat cifra_caesar.txt | tr [d-za-c] [a-wx-z]
```

---
![Cowsay a joke](/assets/images/taller/cowsay_a_joke.png)
