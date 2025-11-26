# Selección y Configuración de Vídeo en HTML5

Este proyecto demuestra la selección de formatos de vídeo y configuraciones de reproducción óptimas para garantizar compatibilidad, accesibilidad y experiencia de usuario mejorada en navegadores modernos.

---

## Formatos de Vídeo Soportados

| Formato | Codec | Ventajas | Navegadores Soportados |
|---------|-------|----------|-----------------------|
| MP4     | H.264/AAC | Alta compatibilidad, soportado por casi todos los navegadores | Chrome, Edge, Safari, Firefox, iOS, Android |
| WebM    | VP9/Opus | Libre de licencias, útil en entornos corporativos que bloquean H.264 | Chrome, Firefox en Linux |
| OGG     | Theora/Vorbis | Compatibilidad con navegadores antiguos o de código abierto | Firefox antiguo, navegadores open source |

> Con estos formatos, el vídeo puede reproducirse en cualquier navegador que soporte HTML5 sin necesidad de instalar codecs adicionales.

---

## Configuraciones de Reproducción

- **autoplay:** No se activa para evitar molestias, consumo innecesario de datos y cumplimiento de políticas de navegadores.
- **loop:** Desactivado. El usuario decide si desea reproducir el vídeo de nuevo.
- **preload:** `metadata` por defecto. Descarga solo la información mínima (primeros fotogramas y duración) para acelerar la carga inicial.
- **poster:** `poster.jpg`. Imagen fija mientras el vídeo está pausado, útil para conexiones lentas o modo ahorro de datos.
- **controls:** Siempre visibles. Permiten pausar, silenciar o cambiar la velocidad, facilitando la accesibilidad.

> Se incluye un botón personalizado “Reproducir vídeo” que otorga control adicional al usuario, mejorando la percepción de rapidez de la página y respetando preferencias de accesibilidad.

---

## Impacto en la Experiencia de Usuario

- **Compatibilidad total:** Funciona en cualquier sistema operativo sin instalar software adicional.
- **Carga rápida:** Solo se descarga lo esencial hasta que el usuario interactúa.
- **Navegación predecible:** Sin reproducciones inesperadas ni consumo de batería en segundo plano.
- **Accesibilidad incrementada:** Controles nativos, imagen de cartel y posibilidad de pausar en cualquier momento.

---

## Estructura del Proyecto

> portafolio
> ├── index.html
> └── video
>     ├── tutorial.mp4
>     ├── tutorial.ogg
>     └── tutorial.webm