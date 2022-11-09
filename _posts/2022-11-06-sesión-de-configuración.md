---
name: Sesión de Configuración
layout: post
post-image: https://parrotlinux.org/_next/static/image/src/containers/HomeContainers/ToolsSection/assets/anonsurf.844c14233c8ff740daeb31ad9bf91b58.png
description: En esta sesión se revisarán las distintas opciones para el uso de Parrot, con sus ventajas y desventajas respectivas. En esta guía se presentan esas opciones para que escojas dependiendo de los recursos de tu equipo y de lo que se te adapte mejor a ti.
tags: Guía Elemental Configuración
---
# Parrot OS
[Parrot OS](https://www.parrotsec.org/) es un sistema operativo basado en Linux que está enfocado en la ciberseguridad. Su instalación normal viene con las herramientas más utilizadas para pentesting y análisis forense.
## Requerimientos para la instalación
Las especificaciones mínimas oficiales para la instalación de Parrot son las siguientes:

| Procesador | Gráfica                              | RAM  | Almacenamiento |
| ---------- | ------------------------------------ | ---- | -------------- |
| Dual Core  | No se necesita aceleramiento gráfico | 1 GB | 20 GB               |

Sin embargo, **en ocasiones la instalación da problemas cuando se está cerca de los requerimientos mínimos**. Por eso hacemos esta guía, para que dependiendo de las características de tu equipo puedas escoger lo que mejor te convenga.

---
# Opciones para utilizar Parrot
## Instalación en máquina virtual
> Si tu equipo tiene **8 GB o más de RAM**, te conviene esta opción. Los equipos de 4 GB también pueden llegar a soportar una máquina virtual (poco recomendado), pero puedes probar si después de la instalación, y mientras la máquina virtual está activa, el rendimiento de tu equipo es aceptable.

Con este método se utiliza software de virtualización para crear una máquina virtual dentro del sistema operativo (SO) principal.

| Ventajas                               | Desventajas                            |
| -------------------------------------- | -------------------------------------- |
| Sin costo                              | Impacta el rendimiento del equipo      |
| Funciona como si fuera tu SO principal | Impacta el almacenamiento de tu equipo |
| _Desisntalación_ de Parrot fácil       |                                        |


## Dual boot
> Si tienes una **copia de seguridad** de tus archivos o de tu SO y quieres que tu equipo tenga **el mejor desempeño**, te recomendamos esta opción. Si nunca has instalado un sistema operativo antes, te recomendamos revisar la guía de instalación antes, para que consideres si el proceso será complicado para ti.

Con este método instalas Parrot OS junto a tu SO principal. A través de un menú seleccionas con qué SO quieres iniciar tu equipo en el momento del encendido. 

| Ventajas                                            | Desventajas                                                           |
| --------------------------------------------------- | --------------------------------------------------------------------- |
| Máximo aprovechamiento de las capacidades tu equipo | Posible daño a tu SO principal si sigues mal la guía                  |
| Sin costo                                           | Más difícil de _desinstalar_ (borrar) Parrot que en los otros métodos |


## Parrot a Través de Pwnbox
> Si ninguno de los otros métodos son convenientes para ti y estás dispuesto a **pagar una suscripción mensual**, pwnbox puede ser una alternativa para empezar. 

HTB Academy es una plataforma de entrenamiento en ciberseguridad, amigable para principiantes, muy completa e interactiva. Se puede acceder a ella de forma gratuita, sin embargo, la máquina virtual que te proporciona sólo está disponible por 2 hrs al día.
Si te registras o agregas un correo institucional válido (correos de `comunidad.unam.mx` son válidos), la plataforma te hace un descuento en el plan de estudiante (pagas $8 USD mensuales) y tienes acceso ilimitado a la pwnbox a través del navegador además de otros beneficios.


| Ventajas                                                                 | Desventajas                                                            |
| ------------------------------------------------------------------------ | ---------------------------------------------------------------------- |
| No necesita instalación                                                  | Se necesita una suscripción a la plataforma                            |
| No tiene mucho impacto sobre el rendimiento del equipo                   | Los atajos de teclado no funcionan para esta máquina virtual           |
| Se accede a través del navegador                                         | Las configuraciones y archivos no se guardan cuando se apaga el equipo |
| Te da acceso a la academia de HTB con módulos prácticos sobre Pentesting |                                                                        |


## Parrot Live
> Este método es conveniente si tu equipo **no cuenta con mucha memoria RAM** o si no puedes acceder a Parrot de ninguna de las otras formas.

Con este método usarás una unidad USB como si fuera el disco duro donde está almacenado tu sistema operativo, y podrás usar Parrot como si fuera tu SO principal sin hacer cambios en él. 

| Ventajas                                       | Desventajas                                                                                                |
| ---------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| No necesita instalación                        | Los cambios (configuraciones y archivos) no se guardan.                                                    |
| No hace cambios en el SO                       | Cada vez que se inicia Parrot se tiene que configurar la distribución del teclado (`xkbmap -layout latam`) |
| Se aprovecha la mayoría de recursos del equipo |                                                                                                            |
| Es portable                                    |                                                                                                            |

