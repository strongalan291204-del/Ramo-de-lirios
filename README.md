# Ramo de lirios 💛

Animación en canvas: un cielo nocturno estrellado y un ramo de lirios que se va armando solo.
Al final aparece el mensaje "Para mi flor favorita".

Es un proyecto de un solo archivo (`index.html`): no hay que instalar nada ni compilar.

## Cómo verlo

**Opción 1 (la más simple):** haz doble clic en `index.html` y se abre en el navegador.

**Opción 2 (desde VS Code):**
1. Descomprime el zip y abre la carpeta `ramo-de-lirios` en VS Code (Archivo → Abrir carpeta).
2. Instala la extensión **Live Server** (VS Code te la sugiere al abrir la carpeta).
3. Clic derecho sobre `index.html` → **Open with Live Server**. La página se recarga sola cada vez que guardas.

## Cosas útiles

- Tocar o hacer clic en la pantalla reinicia la floración.
- La letra del mensaje (Dancing Script) se descarga de Google Fonts: hace falta internet para verla. Sin conexión se usa una letra cursiva del sistema.
- Si algo no se ve, abre la consola del navegador (F12 → Console) para ver si hay errores.

## Dónde cambiar cosas (todo en `index.html`)

- **El mensaje:** busca `<div class="message"`.
- **Colores de los lirios:** el objeto `PALETTES`.
- **Cuántos lirios hay y dónde van:** la lista `HEAD_DEFS` (posición `x` / `y`, tamaño `R`, color `pal` y el momento en que se abre `start`).
- **Velocidad de la animación:** los tiempos de `TIMING` y `HEAD_T`.
