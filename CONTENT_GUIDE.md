# Guía para Agregar Contenido

Este documento proporciona instrucciones sobre cómo agregar el contenido desde el sitio web original www.raulnavas.com.ar a este sitio Jekyll.

## Páginas del Sitio

### 1. Página Principal (`index.markdown`)
**URL del sitio:** https://www.raulnavas.com.ar/

**Qué copiar:**
- Presentación personal
- Breve descripción de actividades
- Cualquier texto introductorio

**Cómo editar:**
Edite el archivo `index.markdown` y reemplace el texto entre corchetes con el contenido real.

### 2. Acerca de (`about.markdown`)
**Sección del sitio original:** Acerca de / Biografía

**Qué copiar:**
- Información biográfica
- Formación académica
- Áreas de interés
- Trayectoria profesional

**Cómo editar:**
Edite el archivo `about.markdown` y reemplace el texto entre corchetes con el contenido real.

### 3. Publicaciones (`publicaciones.markdown`)
**Sección del sitio original:** Publicaciones

**Qué copiar:**
- Lista de libros
- Artículos académicos
- Capítulos de libros
- Otras publicaciones

**Cómo editar:**
Edite el archivo `publicaciones.markdown`. El archivo ya incluye ejemplos de formato para diferentes tipos de publicaciones.

### 4. Docencia (`docencia.markdown`)
**Sección del sitio original:** Docencia / Enseñanza

**Qué copiar:**
- Cursos actuales
- Cursos anteriores
- Seminarios dictados
- Actividades de formación

**Cómo editar:**
Edite el archivo `docencia.markdown`. El archivo incluye ejemplos de formato para organizar los cursos y seminarios.

### 5. Contacto (`contacto.markdown`)
**Sección del sitio original:** Contacto

**Qué copiar:**
- Dirección de correo electrónico
- Afiliación institucional
- Dirección postal
- Teléfono (si aplica)

**Cómo editar:**
Edite el archivo `contacto.markdown` y reemplace los marcadores de posición con la información real.

## Secciones Excluidas

⚠️ **NO incluir:** "Materiales de lectura" - Esta sección fue específicamente excluida según los requisitos del proyecto.

## Formato Markdown

Los archivos utilizan formato Markdown. Aquí hay algunos elementos básicos:

- `# Título` - Encabezado nivel 1
- `## Subtítulo` - Encabezado nivel 2
- `### Subtítulo menor` - Encabezado nivel 3
- `**negrita**` - Texto en negrita
- `*cursiva*` - Texto en cursiva
- `[texto del enlace](URL)` - Enlaces
- `- ítem` - Lista con viñetas

Para más información sobre Markdown, consulte: https://www.markdownguide.org/basic-syntax/

## Actualizar Información del Sitio

Si necesita cambiar el título del sitio, email u otra información general, edite el archivo `_config.yml`.

**Importante:** Después de modificar `_config.yml`, debe reiniciar el servidor Jekyll para que los cambios surtan efecto.

## Visualizar Cambios Localmente

1. Haga los cambios en los archivos markdown
2. Ejecute: `bundle exec jekyll serve`
3. Abra su navegador en: http://localhost:4000
4. Verifique que los cambios se vean correctamente

## Publicar Cambios

Después de hacer cambios:

```bash
git add .
git commit -m "Descripción de los cambios realizados"
git push
```

## Recursos Adicionales

- [Documentación de Jekyll](https://jekyllrb.com/docs/)
- [Guía de Markdown](https://www.markdownguide.org/)
- [Tema Minima](https://github.com/jekyll/minima)
