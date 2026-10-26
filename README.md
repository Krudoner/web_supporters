# Web Jovent Gironí

Web responsive multipágina para el **Jovent Gironí**, grada de animación del Girona FC. Proyecto realizado para la agrupación de aficionados: HTML semántico, Tailwind CSS y JavaScript sin frameworks, con foco en rendimiento, accesibilidad y SEO.

**Demo:** [jovent-gironi17.netlify.app](https://jovent-gironi17.netlify.app/)

## Lighthouse / PageSpeed

100 en las cuatro categorías (informe de escritorio):

![Resultado de Lighthouse: 100 en Rendimiento, Accesibilidad, Prácticas recomendadas y SEO](docs/lighthouse.png)

## Páginas

| Página | Contenido |
| --- | --- |
| `index.html` | Portada con slider de imágenes y bloques de noticias destacadas |
| `identitat.html` | Quiénes son, qué hacen y convocatoria de nuevos miembros |
| `noticies.html` | Noticias y crónicas de desplazamientos |
| `botiga.html` | Catálogo de productos del grupo |
| `galeria.html` | Galería de imágenes con filtros por categoría |
| `contacte.html` | Formulario de contacto e información |
| `404.html` | Página de error personalizada |

## Qué incluye

- **Diseño responsive** mobile-first con Tailwind CSS y menú hamburguesa adaptado a móvil.
- **JavaScript propio (vanilla):** menú con `aria-expanded`, slider automático, filtros de galería y botones "Leer más / Leer menos".
- **Accesibilidad:** enlace "saltar al contenido", textos alternativos, etiquetas ARIA y contraste cuidado.
- **Rendimiento:** imágenes en WebP con `srcset`/`sizes`, precarga de la imagen principal y fuentes en `woff2`.
- **SEO:** metadatos por página, `sitemap.xml` y `robots.txt`.
- **Formularios** gestionados con Formspree, sin backend propio.
- **Despliegue** en Netlify.

## Tecnologías

HTML5 · Tailwind CSS 3.4 (CLI) · JavaScript · Formspree · Netlify

## Estructura

```
├── index.html, identitat.html, noticies.html,
│   botiga.html, galeria.html, contacte.html, 404.html
├── src/            input.css, fonts.css y output.css (compilado)
├── img/            Imágenes optimizadas
├── font/           Montserrat y Roboto (woff2)
├── docs/           Captura de Lighthouse
├── tailwind.config.js
├── sitemap.xml
└── robots.txt
```

## Desarrollo local

Requiere Node.js. El sitio es estático, así que basta con abrir `index.html` o usar una extensión como Live Server.

Para modificar estilos:

```bash
npm install
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
```

Para generar el CSS de producción minificado:

```bash
npx tailwindcss -i ./src/input.css -o ./src/output.css --minify
```

## Aviso

Proyecto personal de portfolio, desarrollado de forma voluntaria para el Jovent Gironí. El nombre, el logotipo y las fotografías pertenecen al Jovent Gironí y a sus autores; el Girona FC y su escudo son propiedad de sus titulares. El código no está pensado para reutilizar esos materiales.

## Autor

Victor Alcrudo Abad · [GitHub](https://github.com/Krudoner) · [LinkedIn](https://www.linkedin.com/in/v-alcrudo-5710b3350)
