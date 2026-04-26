# Guía de Configuración: Portafolio Académico (Club de Robótica ESPOL)

Esta guía detalla los cambios realizados sobre la plantilla original para adaptarla a un perfil de ingeniería y mecatrónica. Sigue estas instrucciones para mantener tu portafolio actualizado.

---

## 1. Configuración de Identidad (`_config.yml`)
Abre `_config.yml` en la raíz para personalizar tu información:
* **Author:** Cambia `name`, `bio` y `location`.
* **Social:** Agrega tus enlaces de LinkedIn, GitHub y Google Scholar.
* **Email:** Cambia el correo en la sección de links para que el botón de contacto funcione con tu cuenta de ESPOL.

---

## 2. Publicación de Contenido (Carpeta `_posts`)
Todo el contenido dinámico (Proyectos, Research y Papers) se gestiona creando archivos `.md` en la carpeta `_posts`.

### Reglas de Oro:
1. **Nombre del archivo:** Debe empezar con la fecha: `YYYY-MM-DD-titulo.md`.
2. **Fecha:** Si el post no aparece, asegúrate de que la fecha sea de "hoy" o del pasado (Jekyll oculta fechas futuras).

### Categorías disponibles:
Dependiendo de qué escribas en `categories:` dentro del archivo, el post irá a una sección u otra:

* **`projects`**: Para proyectos de clase, botes autónomos, baches, etc. (Incluye imagen `teaser`).
* **`research`**: Para investigaciones formales o proyectos del club. (Incluye imagen `teaser`).
* **`publications`**: Para papers y artículos.

---

## 3. Formato Especial: Publications
A diferencia de las otras secciones, **Publications** está optimizada para mostrarse como una lista bibliográfica académica.

Para agregar una, crea un post con este encabezado:
```yaml
---
title: "Título Interno"
categories:
  - publications
pub_status: "paper" # Usa "paper" para publicados o "review" para revisión
---
[1] Apellido, Nombre. "Título del Paper", Revista/Conferencia, Año.