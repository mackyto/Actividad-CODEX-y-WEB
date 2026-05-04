# ✅ GUÍA DE TESTING Y VALIDACIÓN

Antes de publicar tu web, verifica que todo funciona correctamente.

---

## 🔍 Validación de Código

### HTML Validation
1. Ve a [validator.w3.org](https://validator.w3.org/)
2. Opción "By File Upload"
3. Sube `index.html`
4. Verifica que no hay errores críticos

### CSS Validation
1. Ve a [jigsaw.w3.org/css-validator](https://jigsaw.w3.org/css-validator/)
2. Opción "By File Upload"
3. Sube `style.css`
4. Verifica que los estilos son válidos

---

## 📱 Responsive Testing

### En el Navegador (Chrome/Firefox/Edge)
1. Abre `index.html` en el navegador
2. Abre Developer Tools (F12)
3. Haz clic en el icono de dispositivo móvil
4. Prueba diferentes tamaños:
   - **Móvil**: 375x667 (iPhone SE)
   - **Móvil grande**: 414x896 (iPhone 12)
   - **Tablet**: 768x1024 (iPad)
   - **Desktop**: 1920x1080 (Pantalla grande)

### Herramientas Online
- [ResponsiveDesignChecker.com](https://www.responsivedesignchecker.com/)
- [GoogleMobileTest](https://search.google.com/test/mobile-friendly)
- [BrowserStack](https://www.browserstack.com/)

### Checkpoints
- ✅ Navegación se ve bien en todos los tamaños
- ✅ Imágenes se cargan correctamente
- ✅ Botones son clicables y responden
- ✅ Texto es legible (sin zoom)
- ✅ Videos/mapas funcionan
- ✅ Formulario es accesible

---

## 🎨 Pruebas Visuales

### Colors & Contrast
1. Comprueba que el contraste es suficiente
2. Usa [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)
3. Ratio mínimo recomendado: 4.5:1

### Fuentes
- Verifica que las fuentes se cargan correctamente
- Título (header): clara y visible
- Texto de cuerpo: legible
- Elementos pequeños: distinguibles

### Espaciado
- Padding/margin entre elementos
- Alineación consistente
- No hay elementos superpuestos

---

## ⚡ Rendimiento

### Google Lighthouse
1. Abre Developer Tools (F12)
2. Ve a "Lighthouse"
3. Haz clic en "Generate report"
4. Analiza los resultados:

**Objetivos:**
- Performance: > 80
- Accessibility: > 80
- Best Practices: > 80
- SEO: > 80

### PageSpeed Insights
1. Ve a [pagespeed.web.dev](https://pagespeed.web.dev/)
2. Introduce tu URL de GitHub Pages
3. Revisa Mobile y Desktop scores

### Tiempo de Carga
- Objetivo: < 3 segundos
- Ideal: < 2 segundos

---

## 🔗 Funcionalidad de Links

### Enlaces Internos
- ✅ Navegación funciona (scroll suave)
- ✅ Enlaces a secciones (#caracteristicas, #galeria, etc.)
- ✅ Footer links a documentos `.md`

### Enlaces Externos
- ✅ WhatsApp link abre el cliente
- ✅ Redes sociales abren correctamente
- ✅ Google Maps se carga

### Formulario
- ✅ Botón "Enviar Consulta" abre formulario
- ✅ Validación de campos (required)
- ✅ Botón "Cancelar" cierra formulario
- ✅ Email correcta (info@casarural.es)

---

## 🔐 Seguridad

### SSL/HTTPS
- ✅ GitHub Pages siempre usa HTTPS
- ✅ Sin avisos de seguridad

### Información Personal
- ✅ No se recopila información sensible
- ✅ Formulario está documentado
- ✅ Políticas de privacidad disponibles

---

## ♿ Accesibilidad

### Checklist WCAG
- ✅ Texto alternativo en imágenes
- ✅ Elementos con etiquetas semánticas
- ✅ Colores con suficiente contraste
- ✅ Enfoque visible en elementos interactivos
- ✅ Navegación por teclado funciona

### Test de Accesibilidad
1. Instala [WAVE Extension](https://wave.webaim.org/extension/)
2. Ejecuta en tu página
3. Revisa recomendaciones

---

## 🌐 Compatibilidad de Navegadores

### Navegadores Soportados

| Navegador | Versión Mín. | Estado |
|-----------|--------------|--------|
| Chrome | 90+ | ✅ Totalmente |
| Firefox | 88+ | ✅ Totalmente |
| Safari | 14+ | ✅ Totalmente |
| Edge | 90+ | ✅ Totalmente |
| Opera | 76+ | ✅ Totalmente |

### Pruebas Recomendadas
- Chrome últimas 2 versiones
- Firefox últimas 2 versiones
- Safari en Mac/iPhone
- Edge en Windows

### Testing Online
- [BrowserStack.com](https://www.browserstack.com)
- [LambdaTest.com](https://www.lambdatest.com/)

---

## 📊 Checklist Final Antes de Publicar

### Contenido
- ✅ Título correcto: "Casa Rural de Pruebas - Actividad CODEX"
- ✅ Número de WhatsApp actualizado
- ✅ Email de contacto correcto
- ✅ Teléfono actualizado
- ✅ Ubicación del mapa es correcta
- ✅ Imágenes se cargan correctamente
- ✅ Reseñas son coherentes
- ✅ Características descriptas correctamente

### Técnico
- ✅ HTML valida sin errores
- ✅ CSS valida sin errores
- ✅ Responsive en todos los tamaños
- ✅ Formulario funciona
- ✅ Enlaces funcionan
- ✅ Sin errores en console (F12)
- ✅ Sin warnings de seguridad

### SEO Básico
- ✅ Meta description presente
- ✅ Título único y descriptivo
- ✅ Alt text en imágenes
- ✅ Headings en orden jerárquico
- ✅ Sin enlaces rotos

### Performance
- ✅ Lighthouse score > 80
- ✅ Tiempo carga < 3s
- ✅ Imágenes optimizadas
- ✅ CSS minificado (opcional)

### Seguridad
- ✅ HTTPS habilitado (GitHub Pages)
- ✅ Sin contraseñas en código
- ✅ Sin información personal
- ✅ Validación de formulario

### Documentación
- ✅ README.md completo
- ✅ Políticas legales correctas
- ✅ Comentarios en código
- ✅ PUBLICAR.md listo

---

## 🐛 Debugging

### Errores Comunes

**Las imágenes no cargan:**
- Verifica URL de Unsplash
- Comprueba que la URL es https://
- Usa una URL pública (no local)

**Estilos CSS no aplican:**
- Verifica que `style.css` está en la raíz
- Link correcto: `<link rel="stylesheet" href="style.css">`
- No usar rutas relativas como `./style.css`

**Formulario no funciona:**
- Verifica que JavaScript está habilitado
- Revisa console (F12) para errores
- Botón debe tener tipo correcto

**Página carga lentamente:**
- Reduce tamaño de imágenes
- Usa URLs externas en lugar de locales
- Comprime CSS/JS (si es necesario)

**Scroll suave no funciona:**
- Navegadores nuevos lo soportan
- En navegadores viejos, carga normal
- Verifica `html { scroll-behavior: smooth; }`

---

## 📈 Después de Publicar

### Monitorear
1. Google Analytics (opcional)
2. Google Search Console
3. GitHub Pages status
4. Uptime monitoring

### Actualizar Regularmente
- Nuevas imágenes
- Cambios en características
- Actualizar reseñas
- Cambios de precios
- Información de contacto

---

## 📞 Soporte

Si encuentras problemas:
1. Revisa este documento
2. Lee la consola del navegador (F12)
3. Valida código en W3C
4. Prueba en otro navegador
5. Limpia caché (Ctrl+Shift+Del)

---

**¡Tu web está lista para el mundo! 🌍**
