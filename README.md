# Espacio Glow ✨ — Sitio web

Sitio web elegante de una sola página para **Espacio Glow**, centro estético
Anti-Age en Santiago de Chile, con contacto directo por **WhatsApp**.

- Instagram: https://www.instagram.com/espacioglow.cl/
- WhatsApp: **+56 9 6226 2223** (`https://wa.me/56962262223`)

---

## Estructura

```
Glow/
├── index.html        → Todo el contenido del sitio
├── css/styles.css    → Diseño, colores y responsive
├── js/main.js        → Menú, animaciones y scroll
└── assets/           → (Aquí van tus fotos)
```

No necesita instalación ni dependencias: es HTML, CSS y JavaScript puros.

---

## Imágenes incluidas

Las imágenes de la galería y de la sección "Nosotros" son **referenciales,
tomadas del propio Instagram de [@espacioglow.cl](https://www.instagram.com/espacioglow.cl/)**,
y se guardan localmente en `assets/`:

| Archivo | Uso |
|---|---|
| `espacio-glow-plasma.jpg` | Foto principal de "Nosotros" |
| `dna-led.jpg` | Galería · Tecnología LED |
| `prp-power.jpg` | Galería · PRP |
| `pink-glow.jpg` | Galería · Pink Glow |
| `catalogo-glow.jpg` | Galería · Catálogo |
| `espacio-mirror.jpg` | Galería · Espacio |
| `toxina-botox.jpg` | Galería · Toxina |

> Reemplaza cualquiera de estos archivos por tus propias fotos manteniendo
> el mismo nombre, o cambia la ruta en `css/styles.css`.

---

## Cómo verlo

**Opción 1 — Abrir el archivo:** haz doble clic en `index.html`.

**Opción 2 — Servidor local (recomendado):**

```bash
cd /Users/rhm/Desktop/PROYECTOS/Glow
python3 -m http.server 8765
```

Luego abre `http://localhost:8765` en tu navegador.

---

## Personalización rápida

### 1. Cambiar el número de WhatsApp

Busca y reemplaza **`56962262223`** por tu número (sin `+`, sin espacios)
en `index.html`. Aparece en varios enlaces `wa.me`.

El texto que se escribe automáticamente se controla con el parámetro
`?text=...` de cada enlace (está codificado en URL).

### 2. Cambiar redes sociales

Reemplaza `https://www.instagram.com/espacioglow.cl/` por tu perfil.

### 3. Poner tus fotos

**Foto "Nosotros":** en `index.html`, busca `about-img` y cambia el
`style` por tu imagen:

```html
<div class="about-img" style="background-image:url('assets/espacio.jpg')"></div>
```

**Galería:** cada recuadro es un `<a class="g-item g-a">`. Agrega el estilo
de imagen directamente:

```html
<a class="g-item g-a reveal" href="https://www.instagram.com/espacioglow.cl/"
   style="background-image:url('assets/foto-1.jpg');background-size:cover;background-position:center;">
  <span class="g-tag">Espacio</span>
</a>
```

> Si no pones foto, se muestra un degradado elegante como respaldo.

### 4. Editar tratamientos, opiniones, textos

Todo el texto está escrito directamente en `index.html`, agrupado por
secciones comentadas (`<!-- ============ TRATAMIENTOS ============ -->`, etc.).
Solo edita el texto que quieras.

### 5. Colores y tipografía

En `css/styles.css`, dentro de `:root`, ajusta la paleta:

```css
--rose:      #D9A7A0;   /* rosa empolvado */
--gold:      #C9A46A;   /* dorado */
--charcoal:  #2E2A2B;   /* carbón */
--cream:     #FBF6F3;   /* crema de fondo */
```

---

## Publicar el sitio

Puedes subirlo gratis a cualquiera de estas opciones arrastrando la carpeta:

- **Netlify** → https://app.netlify.com/drop
- **Vercel** → https://vercel.com
- **GitHub Pages** → sube el repo y activa Pages
- **Hosting propio** → sube los archivos por FTP

No requiere configuración especial; `index.html` es la página de inicio.

---

## Incluye

- Diseño responsive (celular, tablet y escritorio)
- Botón flotante de WhatsApp siempre visible
- Menú hamburguesa en móvil
- Animaciones suaves al hacer scroll
- SEO básico y etiquetas Open Graph
- 13 puntos de contacto por WhatsApp distribuidos en el sitio
