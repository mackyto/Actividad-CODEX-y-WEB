# 🚀 PUBLICAR EN GITHUB PAGES - GUÍA RÁPIDA

## ⚡ 5 Pasos para Publicar

### 1️⃣ Crear Repositorio en GitHub
- Ve a https://github.com/new
- Nombre: `casa-rural-cadiz` (o el que prefieras)
- Selecciona **Public**
- Sin inicializar (ya tenemos archivos)
- Crea el repositorio

### 2️⃣ Conectar tu Máquina Local
Copia y ejecuta los comandos que GitHub te muestra:

```bash
cd /home/macky/codex-web/Actividad-CODEX-y-WEB

git remote add origin https://github.com/TU_USUARIO/casa-rural-cadiz.git
git branch -M main
git push -u origin main
```

**Nota**: Reemplaza `TU_USUARIO` con tu usuario de GitHub

### 3️⃣ Activar GitHub Pages
- Ve a Settings del repositorio
- Selecciona **Pages** (en el menú lateral)
- Source: **Deploy from a branch**
- Branch: **main**
- Folder: **/ (root)**
- Haz clic en **Save**

### 4️⃣ Esperar Publicación
- GitHub tardará 30 segundos a 2 minutos
- Verás un mensaje verde con la URL: `https://tuusuario.github.io/casa-rural-cadiz/`

### 5️⃣ ¡Listo! 🎉
- Tu web estará disponible en la URL de GitHub Pages
- Se actualiza automáticamente con cada push

---

## 📝 Personalizar Antes de Publicar

En `index.html`, busca y actualiza:

**Número de WhatsApp** (línea 277):
```html
href="https://wa.me/34612345678"
```
Cambia `34612345678` por tu número

**Email de contacto** (línea 267 y footer):
```html
info@casarural.es
```

**Teléfono** (line 268 y footer):
```html
+34 612 345 678
```

---

## 📤 Hacer Cambios Después

Cada vez que hagas cambios:

```bash
cd /home/macky/codex-web/Actividad-CODEX-y-WEB

# Ver cambios
git status

# Añadir cambios
git add .

# Crear commit
git commit -m "Descripción de los cambios"

# Subir a GitHub
git push
```

La web se actualizará automáticamente en 30 segundos.

---

## ❓ Posibles Problemas

### La web no carga
- Espera 2-3 minutos (GitHub Pages tarda)
- Verifica que el repositorio sea **Public**
- Recarga la página (Ctrl+Shift+R)

### Los estilos no aparecen
- Verifica que `style.css` está en la raíz
- Comprueba que el link en HTML es: `<link rel="stylesheet" href="style.css">`

### Las imágenes no cargan
- Usa las URLs de Unsplash (ya incluidas)
- O cambia por otras URLs públicas

---

## 🔗 URLs Útiles

- **Mi web**: https://tuusuario.github.io/casa-rural-cadiz/
- **Configuración**: https://github.com/tuusuario/casa-rural-cadiz/settings/pages
- **Documentación GitHub Pages**: https://pages.github.com/

---

## ✨ Próximos Pasos

Después de publicar, considera:

1. Añadir Google Analytics
2. Mejorar el SEO
3. Validar HTML con https://validator.w3.org/
4. Probar con https://www.responsivedesignchecker.com/
5. Usar dominio personalizado

---

**¡Tu web está lista para publicar! 🎊**
