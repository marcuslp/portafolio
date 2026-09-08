# Portafolio — Marcos Lopez Pascual

Sitio estático (HTML5 + CSS3 + JS puro, sin frameworks ni build step) listo para publicarse con GitHub Pages.

## Archivos

- `index.html` — contenido y estructura
- `styles.css` — todos los estilos
- `script.js` — menú móvil y resaltado de sección activa

## Cómo publicarlo en GitHub Pages

**Opción A — repo dedicado al portafolio (recomendada)**

1. Crea un repositorio nuevo en GitHub, por ejemplo `portafolio`.
2. Sube estos 3 archivos (`index.html`, `styles.css`, `script.js`) a la raíz del repo.
   - Puedes arrastrarlos directo en la interfaz web de GitHub ("Add file" → "Upload files"), o con Git:
     ```bash
     git init
     git add index.html styles.css script.js
     git commit -m "Primera versión del portafolio"
     git branch -M main
     git remote add origin https://github.com/marcuslp/portafolio.git
     git push -u origin main
     ```
3. Entra al repo en GitHub → **Settings** → **Pages** (en el menú lateral).
4. En "Build and deployment", selecciona **Deploy from a branch**, rama `main`, carpeta `/ (root)`.
5. Guarda. En 1-2 minutos tu sitio estará disponible en:
   `https://marcuslp.github.io/portafolio/`

**Opción B — como tu página de perfil de GitHub**

Si en vez de eso quieres que tu portafolio viva en `https://marcuslp.github.io/` (sin subcarpeta), el repo debe llamarse exactamente `marcuslp.github.io`. El resto del proceso es igual.

## Actualizar contenido más adelante

Todo el texto está directamente en `index.html` (no hay CMS ni base de datos). Para editar experiencia, stack o certificaciones, abre ese archivo y busca la sección correspondiente (`<!-- EXPERIENCIA -->`, `<!-- STACK -->`, etc.) y modifica el texto entre las etiquetas. Cada vez que hagas `git push`, GitHub Pages actualiza el sitio automáticamente.
