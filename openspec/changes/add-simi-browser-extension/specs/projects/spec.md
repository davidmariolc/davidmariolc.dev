## ADDED Requirements

### Requirement: Categoría de extensiones de navegador

The portfolio MUST support `browser-extension` as a project category and display its label in the current locale.

#### Scenario: Simi en el catálogo bilingüe
- **WHEN** el visitante abre el índice de proyectos en español o inglés
- **THEN** encuentra la ficha de Simi y puede llegar a ella desde el listado de extensiones de navegador en el mismo idioma

#### Scenario: Detalle de Simi
- **WHEN** el visitante abre `/es/projects/simi` o `/en/projects/simi`
- **THEN** ve el caso en el idioma de la ruta, con la portada, dos imágenes de galería y enlaces a Chrome Web Store y al repositorio
