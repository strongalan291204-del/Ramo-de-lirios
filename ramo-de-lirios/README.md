# Ramo de lirios 💛

Animación en canvas: un cielo nocturno estrellado y un ramo de lirios que se va armando solo,
con música de fondo y un botón para reproducirla o pausarla. Al final aparece el mensaje
"Para mi flor favorita".

No hay que instalar nada ni compilar, pero ahora son **dos archivos que deben ir juntos**:
`index.html` y `cancion.mp3`. Si mueves uno sin el otro, la música no sonará.

## Cómo verlo

**Opción 1 (la más simple):** haz doble clic en `index.html` y se abre en el navegador.

**Opción 2 (desde VS Code):**
1. Descomprime el zip completo (no solo el `.html`) y abre la carpeta `ramo-de-lirios` en VS Code (Archivo → Abrir carpeta).
2. Instala la extensión **Live Server** (VS Code te la sugiere al abrir la carpeta).
3. Clic derecho sobre `index.html` → **Open with Live Server**. La página se recarga sola cada vez que guardas.

## Cosas útiles

- El botón circular de abajo a la derecha reproduce o pausa `cancion.mp3`; la canción se repite en bucle. No empieza sola porque los navegadores no dejan reproducir audio con sonido sin que la persona haga clic primero.
- Tocar o hacer clic en el fondo (fuera del botón) reinicia la floración.
- La letra del mensaje (Dancing Script) se descarga de Google Fonts: hace falta internet para verla. Sin conexión se usa una letra cursiva del sistema.
- Si algo no se ve o no suena, abre la consola del navegador (F12 → Console) para ver si hay errores. Si `cancion.mp3` no está junto al `index.html`, el botón se deshabilita solo.
- ¿Quieres otra canción? Reemplaza el archivo `cancion.mp3` por el tuyo (con ese mismo nombre) o cambia el nombre en `<audio id="song" src="cancion.mp3" ...>` dentro de `index.html`.

## Dónde cambiar cosas (todo en `index.html`)

- **El mensaje:** busca `<div class="message"`.
- **Colores de los lirios:** el objeto `PALETTES`.
- **Cuántos lirios hay y dónde van:** la lista `HEAD_DEFS` (posición `x` / `y`, tamaño `R`, color `pal` y el momento en que se abre `start`).
- **Velocidad de la animación:** los tiempos de `TIMING` y `HEAD_T`.
