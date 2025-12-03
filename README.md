# Silvia Birthday Page

Página web estática de felicitación de cumpleaños para Silvia, con una galería animada, efectos visuales y música de fondo. Pensada para publicarse fácilmente con GitHub Pages.

## Características
- Galería tipo línea de tiempo generada dinámicamente.
- Imágenes combinadas `.jpg` y `.png` según disponibilidad.
- Efectos de entrada al hacer scroll y pequeños detalles interactivos (flores y abejas).
- Reproducción de música de fondo tras interacción del usuario.

## Estructura del proyecto
- `Regalito_HBS.html`: página principal.
- `images/`: carpeta con las imágenes (`FCS_1.png`, `FCS_2.jpg`, ...).
- `README.md`: este documento.

## Ver en local
Puedes abrir el archivo HTML directamente en tu navegador, o servirlo con un servidor HTTP simple para probar rutas relativas.

```
# Desde la carpeta del proyecto
cd "c:/Users/MRilt/Desktop/SILLVIAHB"

# Opción A: abrir directamente el archivo
# Haz doble clic en Regalito_HBS.html

# Opción B: servidor simple (Python)
python -m http.server 8080
# Luego visita: http://localhost:8080/Regalito_HBS.html
```

## Publicar con GitHub Pages
1. Crea un repositorio en GitHub (por ejemplo, `SILLVIAHB`).
2. Añade el remoto y sube el contenido:
   ```
   cd "c:/Users/MRilt/Desktop/SILLVIAHB"
   git init
   git checkout -b main
   git add -A
   git commit -m "Initial commit: birthday page"
   git remote add origin https://github.com/<tu-usuario>/<tu-repo>.git
   git push -u origin main
   ```
3. En GitHub, ve a `Settings` → `Pages`.
4. En `Build and deployment` selecciona:
   - `Source`: `Deploy from a branch`.
   - `Branch`: `main` y carpeta `/ (root)`.
5. Guarda. Tras unos minutos, tu sitio estará disponible en:
   - `https://<tu-usuario>.github.io/<tu-repo>/Regalito_HBS.html`

Si usas el nombre especial de repo `<tu-usuario>.github.io`, la URL será:
- `https://<tu-usuario>.github.io/Regalito_HBS.html`

## Notas sobre imágenes
- Las imágenes `FCS_1`, `FCS_3` y `FCS_5` son `.png`; el resto son `.jpg`.
- El código detecta la extensión correcta automáticamente al generar la galería.

## Personalización rápida
- Cambia textos en el arreglo `timelineData` dentro del `<script>` de `Regalito_HBS.html`.
- Sustituye imágenes en `images/` manteniendo el patrón `FCS_<n>.<ext>`.
- Ajusta estilos en el bloque `<style>` del HTML.

## Créditos
- Fuentes: Google Fonts (`Pacifico`, `Quicksand`).
- Emojis y efectos visuales creados con HTML/CSS/JS nativo.
# Silvia Birthday Page

Static page for GitHub Pages deployment.