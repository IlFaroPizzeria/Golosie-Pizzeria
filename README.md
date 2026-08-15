# 🍕 Golosie — Web oficial

Web profesional y básica para **Golosie**, pizzería en el Paseo Marítimo de Torrox Costa (Málaga).

Sitio estático (HTML + CSS + JS puro, sin frameworks ni build), listo para editar en VS Code, subir a GitHub y publicar en Vercel.

## 📁 Estructura del proyecto

```
golosie-web/
├── index.html          → Toda la web (una sola página con secciones)
├── css/
│   └── style.css       → Estilos (colores, tipografías, responsive)
├── js/
│   └── script.js       → Menú móvil, pestañas de la carta, etc.
├── assets/img/         → Imágenes (favicon, galería...)
├── vercel.json         → Configuración de despliegue en Vercel
└── package.json        → Solo para poder previsualizar en local
```

## ✏️ Qué tienes que editar tú

1. **Fotos reales** — sustituye los archivos de `assets/img/` (`gallery-1.svg`…`gallery-4.svg`, `interior.svg`) por tus propias fotos. Puedes usar `.jpg` o `.png`; solo tienes que actualizar las rutas en `index.html` (busca `assets/img/`).
2. **Carta / menú** — en `index.html`, busca la sección `<!-- ===== CARTA ===== -->` y edita los platos, descripciones y precios. Los que hay ahora son orientativos (solo pude confirmar los "Entrantes" con la información pública disponible).
3. **Reseñas de Google** — en `<!-- ===== RESEÑAS ===== -->` hay tarjetas de ejemplo. Cuando tengas las reseñas reales, sustituye el texto y el nombre en cada `.review-card`. También puedes cambiar el enlace de "Ver reseñas en Google Maps" por el enlace directo de tu ficha de Google Business.
4. **Redes sociales** — en el `<footer>`, los enlaces de Instagram y Facebook están como `href="#"`. Cámbialos por tus URLs reales.
5. **Teléfono / dirección** — actualmente:
   - Teléfono: `611 21 83 24` (botón de reservar → llama directamente)
   - Dirección: Urb. Centro Internacional, Paseo Marítimo, Bloque 75, Bajo 11, 29793 Torrox Costa
   
   Si algo no es exacto, edítalo en `index.html` (aparece varias veces: cabecera, hero, sección de contacto y footer). El teléfono también está en los enlaces `tel:+34611218324` — recuerda mantener el mismo formato si lo cambias.

## 💻 Cómo abrir y editar en VS Code

1. Descarga/descomprime la carpeta `golosie-web`.
2. Abre VS Code → `Archivo > Abrir carpeta...` → selecciona `golosie-web`.
3. Instala la extensión **Live Server** (de Ritwick Dey) desde el marketplace de VS Code.
4. Clic derecho sobre `index.html` → **"Open with Live Server"** → se abrirá en el navegador con recarga automática al guardar cambios.

## 🐙 Subir el proyecto a GitHub

Desde la terminal, dentro de la carpeta `golosie-web`:

```bash
git init
git add .
git commit -m "Primera versión de la web de Golosie"
```

Luego, en [github.com](https://github.com), crea un repositorio nuevo (vacío, sin README) llamado por ejemplo `golosie-web`, y ejecuta lo que GitHub te indique, similar a:

```bash
git branch -M main
git remote add origin https://github.com/TU-USUARIO/golosie-web.git
git push -u origin main
```

> Si prefieres usar GitHub Desktop en vez de la terminal, simplemente abre la carpeta desde la app y sigue el asistente para publicar el repositorio.

## ▲ Publicar en Vercel

1. Entra en [vercel.com](https://vercel.com) e inicia sesión (puedes hacerlo con tu cuenta de GitHub).
2. Pulsa **"Add New... > Project"**.
3. Selecciona el repositorio `golosie-web` que acabas de subir.
4. Vercel detectará automáticamente que es un sitio estático — no hace falta configurar nada (Framework Preset: "Other" está bien). Pulsa **Deploy**.
5. En 1-2 minutos tendrás la web publicada en una URL tipo `golosie-web.vercel.app`.
6. Si quieres tu propio dominio (por ejemplo `golosietorrox.com`), ve a **Project Settings > Domains** en Vercel y sigue los pasos para conectarlo.

A partir de ahora, cada vez que hagas `git push` a la rama `main`, Vercel volverá a publicar la web automáticamente con los cambios.

## 👀 Previsualizar en local (opcional)

Si tienes Node.js instalado, puedes levantar un servidor local:

```bash
npm run dev
```

Y abrir `http://localhost:3000` en el navegador.

## 📋 Datos usados en la web (verificar)

Esta información se obtuvo de fuentes públicas (Just Eat, directorios de restaurantes) y debe confirmarse:

- **Dirección:** Urb. Centro Internacional, Paseo Marítimo, Bloque 75, Bajo 11, 29793 Torrox Costa, Málaga
- **Teléfono:** 611 21 83 24
- **Email:** sesepizzata1512@icloud.com
- **Horario:** Lun–Vie y Dom 9:00–22:00, Sáb 9:00–22:30

Revísalos y corrígelos en `index.html` si no son exactos.
# Golosie-Pizzeria
