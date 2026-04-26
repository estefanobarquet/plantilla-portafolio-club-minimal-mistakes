# Guía Rápida: Configuración del Portafolio Académico

¡Bienvenidos! Esta es una plantilla optimizada para documentar tus proyectos de robótica, visión computacional e ingeniería. Hemos adaptado el tema original (Minimal Mistakes) para darle un perfil más académico e investigativo.

Sigue estos pasos para personalizar tu página.

---

## 1. Configuración Básica (`_config.yml`)
El archivo `_config.yml` es el cerebro de tu portafolio. Abre este archivo y modifica lo siguiente:

* **url y baseurl:** * Si tu repositorio se llama `tu-usuario.github.io`, deja `baseurl: ""` (vacío).
  * Si tu repositorio tiene otro nombre (ej. `mi-portafolio`), pon `baseurl: "/mi-portafolio"`.
* **Datos personales (sección `author`):**
  * Cambia el `name`, `bio` (ej. *Mechatronics Engineering Student*), y `location`.
* **Contacto y Redes (sección `links`):**
  * Coloca el enlace de tu LinkedIn y Google Scholar.
  * **Email:** Ya está configurado con un script para que al hacer clic se copie al portapapeles. Solo busca la línea del correo y cambia `tu-correo@espol.edu.ec` por el tuyo.

---

## 2. Ajuste de Tamaños y Diseño (CSS)
Si sientes que la letra es muy grande o muy pequeña, puedes ajustarla fácilmente:
1. Ve a la ruta: `_includes/head/custom.html`.
2. Verás un bloque `<style>`. Cambia los valores de `font-size` (por ejemplo, subir de `15px` a `16px`) según tu preferencia. 
3. Guarda los cambios. *Nota: Presiona `Ctrl + Shift + R` en tu navegador para ver los cambios aplicados y limpiar el caché.*

---

## 3. Cómo Subir tu Contenido

### A. Projects y Research (Automático)
Las secciones de "Projects" y "Research" se actualizan automáticamente cuando creas un archivo en la carpeta `_posts`.

1. Entra a la carpeta `_posts`.
2. Crea un archivo con este formato estricto de fecha: `YYYY-MM-DD-nombre-del-proyecto.md` (ej. `2026-04-25-lidar-navigation.md`).
3. Pega este encabezado al inicio de tu archivo:

    ```yaml
    ---
    title: "Nombre de tu Proyecto o Investigación"
    categories: projects  # Cambia a 'research' si es una investigación
    header:
      teaser: /assets/images/tu-miniatura.jpg # Imagen pequeña que saldrá en la lista
    ---
    ```
4. Debajo de ese encabezado, escribe tu reporte técnico, sube diagramas, bloques de código, etc. ¡Aparecerá mágicamente en la página que elegiste!

### B. Publications (Manual)
Las publicaciones (papers, artículos en revisión) llevan un formato de citación más estricto, por lo que se ingresan manualmente.

1. Ve al archivo `publications.md` que está en la raíz del repositorio.
2. Añade tu publicación escribiendo directamente en formato Markdown, siguiendo el formato de citación IEEE.
   * *Ejemplo:* `[1] Tu Apellido, "Título del Paper", Año. Available: https://...`

---
*Plantilla adaptada del tema original Minimal Mistakes por Michael Rose.*