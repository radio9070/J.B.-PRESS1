# J.B. PRESS | Prensa & Difusión del Espectáculo · JB Producciones

Sitio web oficial y Progressive Web App (PWA) de alto impacto visual diseñado para **J.B. PRESS / JB Producciones**. Desarrollado con una estética cinematográfica en modo oscuro, acabados en rojo metálico brillante y cromo pulido 3D, e integración directa con WhatsApp para cotizaciones y atención inmediata.

---

## 🚀 Características Principales

- **Identidad Visual Fiel**: Estilo cromado y rojo rubí reflectivo inspirado fielmente en el logo oficial de JB Producciones.
- **Conexión Directa a WhatsApp**:
  - Botón flotante pulsante siempre visible con acceso directo al número `+54 9 11 5707-2115`.
  - Formulario de contacto inteligente que pre-arma el mensaje con los datos del artista o compañía y lo envía directo a WhatsApp.
- **Sección de Redes Sociales**: Tarjetas de cristal oscuro interactivas para Instagram, Facebook, YouTube, TikTok y canal de WhatsApp.
- **Portafolio / Coberturas con Filtros**: Filtro dinámico e interactivo por categorías (*Todos*, *Teatro*, *Música*, *Eventos*).
- **PWA Ready (`manifest.json`)**: Configurado para que cualquier usuario pueda instalar la web como una aplicación nativa en Android e iOS.
- **100% Responsivo**: Adaptado perfectamente para celulares, tablets y pantallas de escritorio.

---

## 📁 Estructura del Proyecto

```text
├── index.html           # Página web principal completa (HTML5, Tailwind CSS, JS)
├── manifest.json        # Manifiesto de la Progressive Web App (PWA)
├── README.md            # Documentación del proyecto
└── (opcionales)         # Íconos y logo en imágenes locales
    ├── logo.png         # Logo en PNG con fondo transparente
    ├── icon-192.png     # Ícono de app para Android / PWA (192x192)
    └── icon-512.png     # Ícono de app para Android / PWA (512x512)
```

---

## 🛠️ Guía Rápida de Personalización

### 1. Actualizar Redes Sociales
En `index.html`, buscá la sección `<section id="redes">` y actualizá los enlaces de cada tarjeta:

```html
<!-- Instagram -->
<a href="https://instagram.com/TU_PERFIL" target="_blank" rel="noopener noreferrer">
  ...
  <p class="text-xs text-slate-400 mt-1">@tu_usuario_real</p>
</a>

<!-- YouTube, Facebook y TikTok siguen el mismo formato -->
```

### 2. Cambiar o Actualizar el Número de WhatsApp
Si necesitás cambiar el número oficial, buscá y reemplazá en `index.html`:
- En los enlaces `href="https://wa.me/5491157072115"` coloca tu nuevo número con código de país.
- En el script final del formulario, localizá la línea:
  ```javascript
  window.open(`https://wa.me/5491157072115?text=${mensajeWhatsApp}`, '_blank');
  ```
- Y en `manifest.json`, actualizá el enlace del shortcut de WhatsApp.

### 3. Usar tu imagen de Logo local
El sitio incluye por defecto un render vectorial idéntico, pero si querés usar tu archivo PNG directo:
1. Colocá tu archivo `logo.png` en la misma carpeta.
2. En `index.html`, dentro de la sección showroom de inicio, reemplazá el bloque `<svg>...</svg>` por:
   ```html
   <img src="logo.png" alt="JB Producciones" class="w-full max-h-[300px] object-contain mx-auto drop-shadow-[0_10px_25px_rgba(229,9,20,0.6)]">
   ```

---

## 🌐 Cómo Publicar la Web (Hosting Gratuito)

Podés subir la web y tenerla online en minutos usando cualquiera de estas opciones:

### Opción 1: Vercel o Netlify (Recomendado)
1. Creá una cuenta en [Vercel](https://vercel.com) o [Netlify](https://www.netlify.com).
2. Arrastrá la carpeta del proyecto completa directamente en el panel de Netlify Drop o conectá tu repositorio de GitHub.
3. ¡Listo! Te otorgará un enlace HTTPS automático y funcional para compartir como muestra.

### Opción 2: GitHub Pages
1. Subí los archivos `index.html`, `manifest.json` y `README.md` a un repositorio público de GitHub.
2. Ingresá a **Settings** > **Pages**.
3. Seleccioná la rama `main` (rama raíz) y hacé clic en **Save**.
4. En unos segundos tu página estará activa en `https://tuusuario.github.io/nombre-repositorio/`.

---

## 📞 Datos de Contacto Oficiales

- **Nombre**: J.B. PRESS / JB Producciones
- **Especialidad**: Prensa & Difusión del Espectáculo (Teatro, Música, Cine y Eventos)
- **WhatsApp / Tel**: [+54 9 11 5707-2115](https://wa.me/5491157072115)
- **Ubicación**: Buenos Aires, Argentina