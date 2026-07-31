# El Caldero Chorreante

Sitio web estático de un **café-librería mágico ficticio** inspirado en el universo de Harry Potter. Proyecto final del curso de Desarrollo Web (Coderhouse).

> **Aviso:** Este es un proyecto académico de ficción. No está afiliado a Warner Bros., J.K. Rowling ni a ninguna marca oficial.

## Sitio en producción

**Deploy (Vercel):** _(Actualizá esta línea con tu URL)_

```
https://TU-SITIO.vercel.app
```

## Páginas

| Archivo | Descripción |
|---------|-------------|
| `index.html` | Inicio — hero de marca y propuesta de valor |
| `pages/carta.html` | Carta de bebidas, dulces y platos |
| `pages/eventos.html` | Agenda de club de lectura, trivia y talleres |
| `pages/nosotros.html` | Historia, valores y equipo |
| `pages/contacto.html` | Formulario, horarios y datos del local |

## Estructura

```
mi-proyecto/
├── index.html
├── pages/
├── scss/           # Fuentes SCSS (partials + main.scss solo con @use)
├── styles/         # CSS compilado
├── assets/images/  # Multimedia
├── vercel.json     # Configuración de deploy en Vercel
└── README.md
```

## Checklist rúbrica

- [x] 5 HTML semánticos (`index` + 4 en `pages/`)
- [x] SEO: `title`, `meta description` y `meta keywords` únicos + `alt` en imágenes
- [x] Navbar Bootstrap con hamburguesa, estilizada en SCSS
- [x] SCSS: variables, nesting, mixins con parámetros, `@extend`, partials + `@use`
- [x] `main.scss` solo importa partials
- [x] Responsive mobile / tablet / desktop
- [x] Animación nativa (keyframes + transition) + AOS
- [x] Repo Git con al menos 2 commits descriptivos
- [ ] Deploy público en Vercel + link en este README

## Tecnologías

- HTML5 semántico
- SCSS (variables, nesting, mixins, `@extend`, `@use`)
- Bootstrap 5
- AOS
- Vercel (deploy)

## Cómo compilar SCSS

```bash
npm install
npm run sass
# o en modo watch:
npm run sass:watch
```

## Publicar (GitHub + Vercel)

### 1. Subir a GitHub

Desde esta carpeta (`mi-proyecto`):

```bash
# Creá un repo vacío en github.com (público), luego:
git remote add origin https://github.com/TU-USUARIO/el-caldero-chorreante.git
git push -u origin main
```

### 2. Deploy en Vercel

1. Entrá a [https://vercel.com](https://vercel.com) e iniciá sesión con GitHub.
2. **Add New… → Project** → importá el repositorio.
3. Ajustes:
   - **Framework Preset:** Other
   - **Build Command:** `npm run sass` (o dejá el de `vercel.json`)
   - **Output Directory:** `.` (raíz del proyecto)
4. **Deploy** → copiá la URL (`*.vercel.app`).
5. Pegá la URL arriba en **Sitio en producción** y hacé un commit:

```bash
git add README.md
git commit -m "Documenta URL de deploy en Vercel"
git push
```

## Autor

**Agustín Farber** — Proyecto final · Coderhouse · Desarrollo Web Flex
