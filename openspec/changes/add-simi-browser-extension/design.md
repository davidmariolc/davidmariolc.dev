# Design

## Context

El catálogo deriva los listados y rutas de categoría a partir de los proyectos publicados por idioma. Velite controla los valores admitidos y los mensajes localizados definen sus etiquetas.

## Goals

Incorporar Simi al catálogo bilingüe y hacer que su categoría se pueda explorar mediante las rutas existentes.

## Decisions

- Añadir `browser-extension` al enum de Velite y a los mensajes de español e inglés. Los listados, enlaces y sitemap consumirán la nueva categoría a través del contenido.
- Usar `simi` como slug en los dos MDX y reutilizar el campo `links.live` para Chrome Web Store y `links.repository` para GitHub.
- Referenciar las imágenes compartidas por sus public IDs existentes en Cloudinary y usar las dimensiones medidas para la portada y la galería.

## Risks / Trade-offs

- El sitio depende de las imágenes externas. Verificar cada recurso en Cloudinary y comprobar sus referencias en la salida compilada.
