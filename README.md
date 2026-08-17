# GM Importaciones 🛍️

Sitio web de una tienda de electrodomésticos, audio y tecnología importada, con catálogo de productos, información de contacto y preguntas frecuentes.

🔗 **Demo en vivo:** [tienda-digital-three.vercel.app](https://tienda-digital-three.vercel.app/)

## 📋 Descripción

GM Importaciones es un sitio de 5 páginas que presenta un catálogo de productos importados (electrodomésticos, audio, línea blanca), con información de contacto, sección "Nosotros" y preguntas frecuentes. El sitio es completamente responsive, con diseño adaptado a desktop, tablet y mobile.

## 🛠️ Tecnologías utilizadas

- **HTML5** — estructura semántica de las 5 páginas
- **SASS/SCSS** — preprocesador de CSS, organizado en arquitectura por componentes:
  - `utilities/` — variables, mixins y animaciones reutilizables
  - `components/` — header y footer compartidos entre páginas
  - `pages/` — estilos específicos de cada página
- **CSS Grid & Flexbox** — para los layouts responsive
- **Google Fonts** — tipografía Poppins
- **Git & GitHub** — control de versiones, con flujo de ramas (`sass` para desarrollo, `main` para producción)
- **Vercel** — hosting y deploy automático

## 📁 Estructura del proyecto

```
proyecto_coder/
├── index.html
├── css/
│   └── styles.css          ← compilado automáticamente desde sass/
├── img/
│   └── favicon/
├── pages/
│   ├── productos.html
│   ├── contacto.html
│   ├── nosotros.html
│   └── preguntas.html
└── sass/
    ├── main.scss             ← archivo principal, importa todo lo demás
    ├── utilities/
    │   ├── _variables.scss
    │   ├── _mixins.scss
    │   └── _animation.scss
    ├── components/
    │   ├── _header.scss
    │   └── _footer.scss
    └── pages/
        ├── _home.scss
        ├── _productos.scss
        ├── _contacto.scss
        └── _nosotros.scss
```

## 💻 Instalación y uso local

1. Cloná el repositorio:
```bash
git clone https://github.com/Guillemeza/Tienda-Digital.git
cd Tienda-Digital
```

2. Instalá Sass globalmente (si no lo tenés):
```bash
npm install -g sass
```

3. Corré el compilador de SASS en modo watch, para que los cambios en `.scss` se reflejen automáticamente en el `.css`:
```bash
cd sass
sass --watch main.scss:../css/styles.css
```

4. Abrí `index.html` con Live Server (extensión de VS Code) o directamente en el navegador para ver el sitio.

## ✨ Características

- Diseño responsive (desktop, tablet, mobile) con media queries organizados en mixins de SASS
- Menú de navegación con submenú desplegable
- Grid de productos adaptable según el tamaño de pantalla
- Animaciones sutiles: fade-in en el hero de la página principal, efecto hover en cards de producto, botón flotante de WhatsApp animado
- SEO básico: meta descriptions y títulos únicos por página
- Favicon completo (incluyendo Apple Touch Icon y manifest)

## 👤 Autora

Guillermina Meza

## 📄 Licencia

Proyecto educativo, desarrollado como práctica del curso de Desarrollo Web.