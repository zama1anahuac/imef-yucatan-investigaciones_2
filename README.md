# Plataforma GitHub Pages · IMEF Yucatán × Anáhuac Mayab · V2.2

# Plataforma estática IMEF Yucatán × Anáhuac Mayab — V2.1

**Borrador de revisión académica, no avalado oficialmente.** Incluye Centro de descargas, 36 fichas PDF, 12 propuestas ejecutivas, metodología, matriz pública en Excel y CSV sin registros autorizados.

## Publicación en GitHub Pages

1. **Solicita revisión del profesor antes de hacer pública la web**. GitHub Pages deja accesibles los archivos publicados a cualquier visitante.
2. Descomprime este ZIP y coloca **el contenido** directamente en la raíz del repositorio (index.html debe quedar en la raíz).
3. En GitHub abre Settings → Pages → Deploy from a branch → main → / (root) y guarda.
4. Visita la dirección publicada y entra al apartado **Centro de descargas**.
5. Prueba una ficha (por ejemplo PROP-044), el PDF de las 12, el Excel, el PDF metodológico y el CSV vacío.

## Estructura

```
index.html
style.css
script.js
data/imef_investigaciones.json (proyección pública de la V2)
data/manifest.json
downloads/fichas/PROP-XXX.pdf (36 fichas)
downloads/02_AGENDA_12_PROPUESTAS_PRELIMINARES.pdf
downloads/03_METODOLOGIA_EVALUACION_PRELIMINAR.pdf
downloads/04_MATRIZ_TEMA_PROBLEMA_SECTOR_PUBLICA.xlsx
downloads/05_PROPUESTAS_AUTORIZADAS_DIFUSION.csv (solo encabezados)
POLITICA_DE_PUBLICACION.md
README.md
```

## Cómo funciona

Todos los recursos se derivan automáticamente de `02_MEGABASE_IMEF_V2.json` y mantienen los mismos IDs, títulos, sectores y evaluaciones. Para regenerar descargas cuando haya cambios, usar el proceso de generación; **editar solo el JSON del sitio no modifica archivos PDF/Excel ya generados**. Todos los enlaces utilizan rutas relativas compatibles con GitHub Pages de repositorio.

## Archivos internos y derechos

No se distribuyen fuentes internas, archivos V1, megabase exploratoria ni Excel maestro. No hay autorización de difusión de propuestas en los datos disponibles; el CSV de autorizadas tiene cero filas. Los demás documentos son **fichas de propuesta preliminar** para revisión y consulta, no investigaciones aprobadas ni evidencia de interés institucional.

Prueba local por HTTP: `python3 -m http.server 8000` en la carpeta raíz, luego abrir `http://127.0.0.1:8000`. La publicación real en un dominio `github.io` solo puede verificarse después del despliegue.


## Novedades V2.2

- Se añadieron imágenes editoriales originales en la portada y en las secciones principales.
- Se incorporó la carpeta `assets/images/` con recursos visuales listos para GitHub Pages.
- No se modificó la estructura de datos ni el archivo `data/imef_investigaciones.json`.
