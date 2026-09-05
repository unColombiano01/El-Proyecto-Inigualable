# Portafolio — Fray Emilio Garcia Garnica

Portafolio personal, 100% estático (HTML + CSS + JavaScript), sin backend ni
base de datos. Al no depender de ningún servidor propio, el sitio queda
disponible de forma permanente para cualquiera que abra el enlace: GitHub
Pages sirve los archivos directamente desde este repositorio.

**Demo en vivo:** `https://unColombiano01.github.io/NOMBRE-DEL-REPOSITORIO/`
*(reemplaza `NOMBRE-DEL-REPOSITORIO` por el nombre real una vez publicado el repo).*

## Contenido

- `index.html` — estructura semántica de la página (header, hero, secciones, footer).
- `css/style.css` — sistema de diseño ("plano técnico"), estilos y responsive.
- `js/script.js` — menú móvil, año dinámico del footer y animación de revelado al hacer scroll.
- `assets/img/` — foto de perfil optimizada (`.webp` con fallback `.jpg`).

## Secciones de la página

1. **Hero** — presentación, rol y llamados a la acción (ver proyectos / escribir correo).
2. **Sobre mí** — resumen de formación y enfoque profesional.
3. **Skills** — Java, Spring Boot, HTML, CSS, JavaScript, SQL, Python, PSeInt, Git, n8n.
4. **Herramientas** — Visual Studio, NetBeans, IntelliJ IDEA, DBeaver y n8n.
5. **Proyectos** — seis repositorios del entrenamiento, con enlace directo a cada uno.
6. **Contacto** — correo (`mailto:`), GitHub y LinkedIn.

## Cómo verlo en local

No requiere instalación ni dependencias. Basta con abrir `index.html` en el
navegador, o servirlo con cualquier servidor estático:

```bash
# Opción 1: abrir directamente
open index.html          # macOS
xdg-open index.html      # Linux

# Opción 2: servidor local simple
python3 -m http.server 8080
# luego visita http://localhost:8080
```

## Despliegue en GitHub Pages

1. Sube este proyecto a un repositorio en GitHub (ver flujo de Git más abajo).
2. Entra a **Settings → Pages** del repositorio.
3. En **Source**, selecciona la rama `main` y la carpeta `/root`.
4. Guarda. GitHub publicará la URL pública en unos minutos.
5. Cada vez que hagas `push` a `main`, el sitio se actualiza automáticamente.

Al ser un sitio estático servido por la CDN de GitHub Pages, el enlace
permanece siempre accesible para cualquier visitante, sin necesidad de tener
un servidor propio encendido.

## Flujo de trabajo con Git (Git Flow simplificado)

```bash
# Rama principal: main       → siempre desplegable
# Ramas de trabajo: feature/*, fix/*, docs/*

git checkout -b feature/nueva-seccion
# ... trabajo ...
git add .
git commit -m "feat: agrega sección de herramientas"
git push origin feature/nueva-seccion
# Luego abrir un Pull Request hacia main
```

### Commits convencionales

Este proyecto sigue la convención [Conventional Commits](https://www.conventionalcommits.org/es/):

| Prefijo     | Uso                                             |
|-------------|--------------------------------------------------|
| `feat:`     | Nueva funcionalidad o sección                    |
| `fix:`      | Corrección de errores                            |
| `style:`    | Cambios de estilo/CSS que no afectan la lógica   |
| `docs:`     | Cambios en documentación (README, comentarios)   |
| `refactor:` | Reestructuración de código sin cambiar comportamiento |
| `chore:`    | Tareas de mantenimiento (assets, configuración)  |

Ejemplos usados en este proyecto:

```
feat: estructura base del portafolio con HTML semántico
feat: agrega sección de skills con Java y Spring Boot
feat: agrega sección de herramientas de desarrollo
style: aplica sistema de diseño "plano técnico"
feat: agrega menú responsivo y animación de revelado
docs: agrega README con instrucciones de despliegue
```

## Checklist de requisitos cumplidos

- [x] Responsive (móvil, tablet, escritorio)
- [x] Contraste de color cuidado (paleta oscura + acento ámbar sobre texto claro)
- [x] Imágenes optimizadas (WebP + fallback JPEG, tamaños reducidos)
- [x] HTML semántico (`header`, `nav`, `main`, `section`, `article`, `footer`)
- [x] Navegación clara con anclas a cada sección y menú móvil
- [x] Listo para GitHub Pages (sin dependencias de build)
- [x] Animaciones y transiciones (hover, revelado al scroll, respeta `prefers-reduced-motion`)
- [x] Redirección a correo electrónico (`mailto:`)
- [x] README con documentación del proyecto

## Contacto

- Correo: garciafray05@gmail.com
- GitHub: [github.com/unColombiano01](https://github.com/unColombiano01)
- LinkedIn: [Fray Emilio Garcia Garnica](https://www.linkedin.com/in/fray-emilio-garcia-garnica-7458bb3b6/)
