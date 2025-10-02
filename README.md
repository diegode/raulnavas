# Raúl Navas - Sitio Web

Este es el repositorio del sitio web personal de Raúl Navas, creado con Jekyll.

## Requisitos

- Ruby 3.x
- Bundler

## Instalación

```bash
bundle install
```

## Desarrollo local

Para ejecutar el sitio localmente:

```bash
bundle exec jekyll serve
```

El sitio estará disponible en `http://localhost:4000`

## Construcción

Para construir el sitio estático:

```bash
bundle exec jekyll build
```

Los archivos generados estarán en el directorio `_site/`.

## Estructura del sitio

- `index.markdown` - Página principal
- `about.markdown` - Página "Acerca de"
- `publicaciones.markdown` - Publicaciones académicas
- `docencia.markdown` - Actividad docente
- `contacto.markdown` - Información de contacto

## Nota

Este sitio fue creado basándose en la estructura de www.raulnavas.com.ar, excluyendo la sección "Materiales de lectura" como fue solicitado.

Para agregar el contenido del sitio original:
1. Visite https://www.raulnavas.com.ar/
2. Copie el contenido de cada sección
3. Actualice los archivos markdown correspondientes en este repositorio