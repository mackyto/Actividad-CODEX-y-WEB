# 🎨 GUÍA DE CUSTOMIZACIÓN

Este documento te ayuda a personalizar la web según tus necesidades.

## 🔤 Cambiar Textos

### Título Principal
**Archivo**: `index.html` línea 15

```html
<h1 class="header-title">Casa Rural de Pruebas - Actividad CODEX</h1>
```

Cambio: Reemplaza "Actividad CODEX" por tu nombre

### Subtítulo
**Archivo**: `index.html` línea 16

```html
<p class="header-subtitle">Una experiencia rural inolvidable en Cádiz</p>
```

### Hero Text (Sección Principal)
**Archivo**: `index.html` líneas 34-37

```html
<h2>Bienvenido a nuestro refugio rural</h2>
<p>Descubre la paz y la naturaleza en el corazón de Cádiz</p>
```

### Características
**Archivo**: `index.html` líneas 46-96

Cada característica tiene formato:
```html
<div class="caracteristica-card">
    <div class="caracteristica-icon">🛏️</div>
    <h3>4 Dormitorios</h3>
    <p>Descripción...</p>
</div>
```

---

## 📞 Cambiar Información de Contacto

### Número de WhatsApp
**Archivo**: `index.html` línea 277

```html
<a href="https://wa.me/34612345678?text=Hola">
```

Formato: `https://wa.me/[CÓDIGO_PAÍS][NÚMERO_SIN_ESPACIOS]`

Ejemplos:
- España: `https://wa.me/34612345678`
- México: `https://wa.me/525551234567`
- Argentina: `https://wa.me/541123456789`

### Email
Busca y reemplaza `info@casarural.es` en:
- Línea 267 (botón contacto)
- Línea 356 (footer)
- Archivos `.md` (políticas)

### Teléfono
Busca y reemplaza `+34 612 345 678` en:
- Línea 268 (ubicación)
- Línea 356 (footer)
- Documentos legales

---

## 🗺️ Cambiar Ubicación del Mapa

**Archivo**: `index.html` línea 170

Actual:
```html
<iframe 
    src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3147.7889757575584!2d-5.760938!3d36.7381!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0xd0d5d5d5d5d5d5d5%3A0x1234567890!2sArcos%20de%20la%20Frontera%2C%20C%C3%A1diz!5e0!3m2!1ses!2ses!4v1234567890"
```

### Cómo cambiar la ubicación:

1. Ve a [Google Maps](https://www.google.com/maps)
2. Busca tu ubicación
3. Haz clic en el icono de compartir (↗️)
4. Selecciona "Insertar un mapa"
5. Copia el código iframe completo
6. Reemplaza el iframe anterior

---

## 🖼️ Cambiar Imágenes

### Foto Hero (Principal)
**Archivo**: `index.html` línea 32

```html
<img src="https://images.unsplash.com/photo-1613395877344-13d4a8e0d49e?w=1200&h=600&fit=crop">
```

Alternativas libres:
- [Unsplash.com](https://unsplash.com) - Busca "rural house"
- [Pexels.com](https://www.pexels.com) - Busca "casa rural"
- [Pixabay.com](https://pixabay.com) - Busca "farmhouse"

### Galería de Fotos
**Archivo**: `index.html` líneas 202-237

6 imágenes diferentes. Cada una:

```html
<div class="galeria-item">
    <img src="https://images.unsplash.com/photo-1564013799919-ab600027ffc6?w=400&h=300&fit=crop" 
         alt="Descripción" 
         class="galeria-img">
</div>
```

Para cambiar:
1. Ve a Unsplash/Pexels/Pixabay
2. Busca una imagen
3. Copia la URL pública
4. Pega en `src=""`
5. Actualiza el `alt=""`

---

## 🎨 Cambiar Colores

**Archivo**: `style.css`

### Colores principales:

```css
/* Azul/Púrpura */
#667eea

/* Púrpura oscuro */
#764ba2

/* Verde WhatsApp */
#25d366

/* Gris oscuro */
#333

/* Fondo claro */
#f8f9fa

/* Footer oscuro */
#2c3e50
```

### Dónde cambiarlos:

1. **Header/Footer**: Líneas 28, 355
2. **Botones**: Líneas 334, 341
3. **Links**: Línea 67
4. **Tarjetas**: Línea 119
5. **Reseñas**: Línea 281

### Herramientas:
- [Coolors.co](https://coolors.co) - Generador de paletas
- [ColorHexa.com](https://www.colorhexa.com) - Información de colores

---

## 📱 Cambiar Tamaños de Fuente

**Archivo**: `style.css`

### Puntos clave:

```css
/* Título grande */
.header-title { font-size: 2.5rem; }  /* Línea 36 */

/* Títulos de sección */
.section-title { font-size: 2rem; }  /* Línea 137 */

/* Textos normales */
body { font-size: 1rem; }  /* Implícito en line-height: 1.6 */

/* Tamaños de pantalla pequeña */
@media (max-width: 480px) {
    .header-title { font-size: 1.4rem; }  /* Línea 553 */
}
```

---

## ⭐ Cambiar Reseñas

**Archivo**: `index.html` líneas 254-294

Estructura de cada reseña:

```html
<div class="resena-card">
    <div class="estrellas">⭐⭐⭐⭐⭐</div>
    <p class="resena-texto">"Texto de opinión..."</p>
    <p class="resena-autor"><strong>Nombre Persona</strong></p>
    <p class="resena-fecha">Visitó en Mes de Año</p>
</div>
```

Para cambiar:
1. Reemplaza el número de estrellas (máximo 5)
2. Cambia el texto de opinión
3. Actualiza el nombre del cliente
4. Modifica la fecha de visita

---

## 🔧 Cambiar Características

**Archivo**: `index.html` líneas 46-96

Estructura:
```html
<div class="caracteristica-card">
    <div class="caracteristica-icon">🛏️</div>  <!-- Emoji -->
    <h3>Título</h3>
    <p>Descripción</p>
</div>
```

Emojis útiles:
- 🛏️ Camas/Dormitorios
- 🚿 Baños
- 🍳 Cocina
- 🛋️ Salón
- 🌳 Terraza/Naturaleza
- 🏊 Piscina
- 🌡️ Climatización
- 🔐 Seguridad
- 📶 WiFi
- 🚗 Parking

---

## 📝 Cambiar Documentos Legales

### Política de Privacidad
**Archivo**: `politica-privacidad.md`

Cambios mínimos necesarios:
- Línea 17: Nombre de la empresa
- Línea 27: Email de contacto
- Línea 28: Teléfono
- Línea 29: Dirección
- Línea 91: Email para reclamaciones

### Aviso Legal
**Archivo**: `aviso-legal.md`

Cambios importantes:
- Líneas 5-9: Datos de la empresa
- Línea 34: URL del sitio
- Línea 157: Email para contacto

### Política de Cookies
**Archivo**: `cookies.md`

Cambios:
- Línea 90-100: Tabla de cookies (si añades más)
- Línea 132: Email de contacto

---

## 🔍 Añadir Google Analytics

1. Ve a [analytics.google.com](https://analytics.google.com)
2. Crear nuevo proyecto
3. Copia el ID de seguimiento (formato: G-XXXXXXXXXX)
4. Añade antes de `</head>` en `index.html`:

```html
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

---

## 🤖 Añadir Formulario Funcional

Actualmente, el formulario es simulado. Para hacerlo real:

### Opción 1: Formspree (Recomendado)
1. Ve a [formspree.io](https://formspree.io)
2. Registrate
3. Crea nuevo formulario
4. Obtén el endpoint
5. Cambia `onsubmit="enviarFormulario(event)"` por:

```html
<form method="POST" action="https://formspree.io/f/TU_ID">
```

### Opción 2: EmailJS
1. Ve a [emailjs.com](https://www.emailjs.com)
2. Registrate
3. Sigue su documentación

---

## 🚀 Optimizaciones Avanzadas

### 1. Agregar Favicon
```html
<link rel="icon" href="favicon.ico">
```

### 2. Open Graph (Redes Sociales)
```html
<meta property="og:title" content="Casa Rural">
<meta property="og:description" content="...">
<meta property="og:image" content="...">
<meta property="og:url" content="...">
```

### 3. Schema.org Markup
```html
<script type="application/ld+json">
{
  "@context": "https://schema.org/",
  "@type": "LocalBusiness",
  "name": "Casa Rural",
  ...
}
</script>
```

---

## 📞 Soporte

Si necesitas ayuda:
1. Revisa los comentarios en el código
2. Lee el README.md
3. Consulta la documentación de GitHub Pages
4. Valida HTML en [validator.w3.org](https://validator.w3.org/)

---

**¡Disfruta personalizando tu web! 🎨**
