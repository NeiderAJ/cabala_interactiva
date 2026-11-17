# Cábala interactiva · V1.1

Sitio educativo interactivo: Árbol de la Vida, diez sefirot y correspondencias cabalísticas, angélicas y simbólicas. La ficha de Kéter incorpora un video de YouTube sobre los serafines, sin abandonar la página.

## Instalación y publicación

Se busca crear un **repositorio de código privado** en `NeiderAJ/cabala_interactiva` y una **página accesible públicamente mediante enlace** en `https://neideraj.github.io/cabala_interactiva/`.

**Advertencias:**
- GitHub Pages en repositorios privados requiere **GitHub Pro o un plan compatible**; si tu cuenta solo tiene GitHub Free, la publicación no funcionará desde el repositorio privado.
- Una página pública de GitHub Pages **no es privada**: no exige conocer el enlace ni autenticarse. El meta `noindex` reduce la indexación por buscadores que lo respetan, pero no ofrece control de acceso.
- La reproducción del video de YouTube requiere acceso a internet y depende de que el autor permita la inserción.

### Opción A: script guiado (Ubuntu / Linux)

1. Descomprime el ZIP.
2. Instala y autentica GitHub CLI si hace falta: `gh auth login` (https://cli.github.com/).
3. Abre una terminal en la carpeta extraída y ejecuta `bash publicar_en_github.sh`.
4. Si GitHub no habilita Pages automáticamente, entra a `https://github.com/NeiderAJ/cabala_interactiva/settings/pages`, selecciona **GitHub Actions** en *Build and deployment*, y vuelve a ejecutar la acción en **Actions**.
5. Consulta el enlace del sitio en *Settings → Pages*.

### Opción B: manual

1. Crea un repositorio **privado** llamado `cabala_interactiva` desde https://github.com/new.
2. Sube a la rama `main` los archivos de este proyecto, incluida la carpeta `.github/workflows/`.
3. En **Settings → Pages**, selecciona **GitHub Actions**.
4. En **Actions**, ejecuta **Publicar Cábala interactiva** si no se lanza automáticamente.

## Cambios y mantenimiento

`index.html` contiene todo el sitio en un solo archivo. Para modificar el contenido, actualiza `index.html`, crea un commit y haz push a `main`; GitHub Actions vuelve a desplegar la web automáticamente.

## Versionado

Punto de partida: V1.1. No se cambió el diseño ni el funcionamiento de la página; solo se añadió una directiva `noindex` de indexación web.
