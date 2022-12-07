---
name: Aplicación para Tomar Notas
layout: post
post-image: https://jonethanrichards.com/wp-content/uploads/2020/09/Obsidian-md.png
description: Comparación entre aplicaciones para tomar notas, enfocado a la organización de el flujo de trabajo de un pentester. Se sugiere la instalación de Obsidian como aplicación para organizar nuestras notas.
tags: Guia Notas Organización Configuración
---

# ¿Para qué tomar notas?
- Para guardar conceptos nuevos y temas relevantes
- Para elaborar nuestras `cheatsheets`
- Para llevar un control de los métodos aplicados en la resolución de máquinas.
- Organizar nuestro aprendizaje.

# Aplicaciones para tomar notas

| Aplicación | Ventajas                                                                                                      | Desventajas                                                                                                              |
| ---------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| OneNote    | - Sincronización<br>- Fácil organización de ideas<br>- Intuitivo                                              | - Precio<br>- Poca personalización<br>- Poco adecuado para realizar reportes de Pentesting<br>- Flujo de trabajo lento   |
| Evernote   | - Sincronización<br>- Intuitivo<br>- Funciona para organizar actividades básicas                              | - Limitaciones en la cuenta básica<br>- Poca escalabilidad<br>- Flujo de trabajo lento<br>- Puede llegar a ser caótico   |
| Obsidian   | - Gratuito<br>- Muchas opciones de personalización<br>- Gran cantidad de plugins<br>- Flujo de trabajo rápido | - No tiene sincronización nativa gratis<br>- Es necesario aprender [Markdown](https://www.markdownguide.org/cheat-sheet) |

---
# Obsidian

## Instalación
1. Descarga para Windows, Linux y mac: https://obsidian.md/
2. Ejecutar el `.exe`


### Baúl
1. Da en `Create new vault`
2. Elige el nombre y la ruta donde se almacenará. Si tienes `Dropbox`, `One Drive` u otro servicio de respaldo en la nube, puedes escoger esa ruta para que tus notas se puedan sincronizar entre dispositivos.

![Obsidian Menú](/assets/images/obsidian_menu.png)


## Configuración
> Optimizado para registrar la resolución de máquinas y el trabajo de pentesting.

Puedes probar distintas configuraciones y distintos plugins para otros baules con otro propósito.


### General

| Instrucción                                                                                                                                                                                                                                                    | Imagen                               |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------ |
| Ve a `Settings` en la esquina inferior izquierda                                                                                                                                                                                                               | ![Botón de Settings](/assets/images/obsidian_settings.png) |
| En la sección `Editor`:<br> -Escoge entre las opciones de `Default editing mode` (se recomienda `Source Mode`)<br>- Activa la opción `Show line number`                                                                                                        | ![Configurar Editor](/assets/images/obsidian_conf_editor.png)  |
| En la sección `Files & Links`:<br>- En `Default location for new notes` escoge `Same folder as current file`<br>- En `Default location for new attachments` escoge `In subfolder under current folder`<br>- Escribe en `Subfolder name` el nombre que quieras. |![Configurar Archivos y Links](/assets/images/obsidian_conf_links.png)|




### Plugins
Ve a `Settings` y a la sección de `Community plugins`. Da click en `Turn on community plugins`. Cuando se activen, de en `Browse`. En el buscador que se abre podrás encontrar plugins que la comunidad desarrolla para complementar las funciones de Obsidian.
> Para todos los siguientes plugins que quieras usar, además de dar en  `Install` tienes que dar tambien en `Enable`.


| Plugin              | Utilidad                                                                                                   |
| ------------------- | ---------------------------------------------------------------------------------------------------------- |
| Advanced Tables     | Hace más sencillo el manejo de tablas. Da `Tab` para ir a la siguiente celda y `Enter` para una nueva fila |
| Image Toolkit       | Proporciona un visor de imágnes al dar click sobre una imagen (estando en modo `Lectura`)                  |
| Clear Unused Images | Elimina las imagenes que no están insertadas en ninguna nota                                               |



### Personalización
Ve a `Settings` y a la sección de `Appearance`. En `Themes` da click en `Manage`.  Busca y selecciona algún tema que te guste y da en `Install and use`.
Temas recomendados (Dark themes):
- Obsidian Nord
- Dark Graphite Pie
- Sanctum

---

## Aplicación para tomar Screen Shots (extra)
Screen Cloud: [screencloud.net](https://screencloud.net/)

## Características
<ul>
<li>Cuenta con atajos de teclado para capturas de:</li>
<ul>
	<li>Pantalla completa</li>
	<li>Sección</li>
	<li>Aplicación activa</li>
</ul>
<li>Guardar, copiar al porta papeles o subir a la nube</li>
</ul>
