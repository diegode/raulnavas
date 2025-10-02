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
- `about.markdown` - Página "Acerca de" (Perfil)
- `publicaciones.markdown` - Publicaciones académicas
- `docencia.markdown` - Actividad docente
- `contacto.markdown` - Información de contacto
- `assets/css/style.scss` - Estilos personalizados (tema oscuro)
- `assets/images/` - Imágenes del sitio (incluye fondo Nighthawks)

## Tema y Diseño

El sitio usa un tema oscuro/nocturno con la pintura "Nighthawks" de Edward Hopper como fondo, replicando el diseño del sitio original.

### Configurar la imagen de fondo:

1. Descargue una imagen de alta calidad de "Nighthawks" de Edward Hopper
2. Guárdela como `assets/images/nighthawks.jpg`
3. La imagen debería ser de al menos 1920px de ancho para buena calidad

Ver `assets/images/README.md` para instrucciones detalladas sobre cómo obtener la imagen.

## Despliegue

Este sitio está configurado para ser alojado en **raulnavas.com.ar**.

### GitHub Pages

Si usa GitHub Pages:
1. El archivo `CNAME` ya está configurado con el dominio `raulnavas.com.ar`
2. Configure los registros DNS de su dominio:
   - Tipo A: Apunte a las IPs de GitHub Pages:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - O Tipo CNAME: Apunte a `diegode.github.io`
3. En la configuración del repositorio en GitHub, active GitHub Pages
4. Especifique el dominio personalizado `raulnavas.com.ar`

### Otro hosting

Para otros servicios de hosting:
1. Ejecute `bundle exec jekyll build`
2. Suba el contenido del directorio `_site/` a su servidor
3. Configure su servidor web para servir los archivos estáticos

## Nota

Este sitio incluye todo el contenido de www.raulnavas.com.ar, excluyendo la sección "Materiales de lectura" como fue solicitado.