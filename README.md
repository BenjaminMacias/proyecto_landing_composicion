# Proyecto Landing: Composición

Landing page estática enfocada en **composición visual**, jerarquía tipográfica y maquetado responsive. Ideal para presentar un producto/servicio con secciones como *hero*, beneficios, testimonios y CTA.

---

## 🧠 Descripción

- Diseño pensado en **composición**: bloques claros, ritmo vertical (espaciados coherentes), contraste tipográfico y uso de grillas.
- **Responsive** (mobile-first) con puntos de corte simples.
- Código limpio: HTML semántico, CSS modular (utilidades y componentes) y un poco de JS opcional para interacciones (si aplica).

---

## 🧰 Tecnologías utilizadas

- **HTML5** (semántico, metas para SEO básico)
- **CSS3** (Flexbox/Grid, variables CSS, reset/normalize)
- **JavaScript Vanilla** (solo si el proyecto incluye pequeñas interacciones)
- (Opcional) **GitHub Pages** para despliegue

---

## ⚙️ Instrucciones de instalación y uso

> Este proyecto es **estático**. No requiere build. Puedes abrir `index.html` directamente o servirlo con un servidor local para evitar problemas de rutas.

### Opción A — Abrir directo
1. Clona el repo:
   ```bash
   git clone https://github.com/BenjaminMacias/proyecto_landing_composicion.git
   cd proyecto_landing_composicion
Abre index.html con tu navegador (doble clic o Ctrl/Cmd+O).

Opción B — Servidor local (recomendado)
Usa cualquiera de estos:

VS Code + Live Server
Clic derecho sobre index.html → Open with Live Server.

http-server (Node.js):

bash
Copiar
Editar
npx http-server -p 5173
# abre http://localhost:5173
Python (3.x):

bash
Copiar
Editar
python -m http.server 5173
# abre http://localhost:5173
🧪 Ejemplos de uso / Personalización
Edita el contenido en index.html y los estilos en css/ (ajusta los nombres si tu repo usa otros).

1) Cambiar textos del hero
En index.html:

html
Copiar
Editar
<section class="hero">
  <h1>Mejora tu rendimiento con NovaFit</h1>
  <p>Ropa técnica, ligera y diseñada para durar.</p>
  <a class="btn btn-primary" href="#contacto">Empezar</a>
</section>
2) Ajustar paleta y tipografía
En css/variables.css (o el archivo principal de estilos):

css
Copiar
Editar
:root{
  --color-bg: #0B0C10;
  --color-text: #C5C6C7;
  --color-accent: #66FCF1;
  --font-base: 'Lexend', system-ui, sans-serif;
}
body{
  background: var(--color-bg);
  color: var(--color-text);
  font-family: var(--font-base);
}
3) Grid de beneficios
html
Copiar
Editar
<section class="features grid">
  <article class="card">
    <h3>Ligero</h3>
    <p>Materiales transpirables para entrenar más cómodo.</p>
  </article>
  <article class="card">
    <h3>Duradero</h3>
    <p>Costuras y telas pensadas para alto rendimiento.</p>
  </article>
  <article class="card">
    <h3>Estético</h3>
    <p>Diseño minimal con foco en la composición.</p>
  </article>
</section>
4) Breakpoints (ejemplo)
css
Copiar
Editar
/* Mobile-first */
.grid{
  display: grid;
  gap: 1rem;
  grid-template-columns: 1fr;
}

@media (min-width: 640px){
  .grid{ grid-template-columns: repeat(2, 1fr); }
}
@media (min-width: 1024px){
  .grid{ grid-template-columns: repeat(3, 1fr); }
}
📁 Estructura sugerida
csharp
Copiar
Editar
proyecto_landing_composicion/
├─ index.html
├─ css/
│  ├─ variables.css
│  ├─ base.css       # reset/normalize + estilos globales
│  └─ main.css       # layout y componentes
├─ js/
│  └─ main.js        # interacciones mínimas (si aplica)
└─ assets/
   ├─ img/
   └─ icons/
Si tu repo usa otros nombres/archivos, ajusta las rutas de acuerdo con tu estructura real.

🚀 Despliegue (GitHub Pages)
Haz commit y push en main.

En GitHub: Settings → Pages → Source: Deploy from a branch.

Branch: main, folder: /root.

Guarda. Se publicará en: https://TU_USUARIO.github.io/proyecto_landing_composicion/.

📝 Notas
Mantén la jerarquía visual con márgenes consistentes (ritmo vertical).

Usa etiquetas semánticas (header, main, section, footer) para accesibilidad/SEO.

Optimiza imágenes en assets/img/ (webp/jpg comprimido).

makefile
Copiar
Editar
::contentReference[oaicite:0]{index=0}
