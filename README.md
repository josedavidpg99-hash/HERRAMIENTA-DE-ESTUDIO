# PrepSeguro Utah — Plataforma universal de estudio

Plataforma gratuita de estudio para el examen de seguros de **salud, vida y accidentes** en Utah.
Practica con un banco de **155 preguntas**, haz simulacros de examen y sigue tu progreso por tema,
todo directamente en tu navegador y sin necesidad de internet.

## Cómo usarla

**Opción 1 — En tu computadora o teléfono (sin instalar nada):**
1. Descarga esta carpeta.
2. Abre el archivo `index.html` con doble clic (se abre en tu navegador).
3. ¡A estudiar! Tu progreso se guarda automáticamente en ese navegador.

**Opción 2 — Publicarla con GitHub Pages:**
1. Sube estos archivos a un repositorio de GitHub.
2. En el repositorio ve a *Settings → Pages* y activa la publicación desde la rama principal.
3. Recibirás un enlace para abrir la plataforma desde cualquier dispositivo, incluso instalarla
   como app gracias al manifiesto PWA y al *service worker* incluido.

## Características

- 📝 **155 preguntas** de práctica sobre salud, vida y accidentes con **nivel de dificultad real de examen**: las 4 opciones tienen longitud similar y las incorrectas son distractores plausibles (inversiones sutiles, números cercanos, confusiones clásicas), así que hay que analizar, no adivinar por descarte. Cada pregunta incluye un **recuadro de contexto** 🧠 en español que explica el concepto a fondo y por qué cada distractor es incorrecto.
- 🎯 **Simulacro de examen** (25, 50, 100 preguntas o el banco completo), sin respuestas visibles.
- 📚 **Práctica por tema**: elige uno o varios temas y estudia con guía de repaso.
- 🔥 **Modo reforzar**: practica automáticamente tus áreas más débiles.
- 📊 **Diagnóstico por tema**: ve tu porcentaje de acierto en cada área.
- 💾 **Progreso guardado** solo en tu navegador (nadie más ve tus resultados).
- 📱 **Diseño móvil**: botones grandes y navegación al alcance del pulgar.
- 🌐 **Funciona sin internet** una vez cargada (PWA instalable).
- ♿ **Accesible**: botones con etiquetas descriptivas y foco automático en cada pregunta
  para lectores de pantalla.

## Estructura de archivos

```
├── index.html        Página principal (carga los archivos de abajo)
├── css/
│   └── styles.css    Todos los estilos
├── js/
│   ├── preguntas.js  Banco de las 155 preguntas (const ALL_Q)
│   └── app.js        Lógica de la app: modos de estudio, progreso, estadísticas
├── manifest.json     Manifiesto PWA (nombre, colores, íconos)
├── sw.js             Service worker: caché para uso sin internet
├── favicon.svg       Ícono de la app
├── README.md         Este archivo
├── LICENSE           Licencia MIT
└── .gitignore        Archivos a ignorar en git
```

## Privacidad

Tus respuestas y tu progreso se guardan únicamente en el `localStorage` de tu propio
navegador. Nada se envía a ningún servidor.

## Licencia

MIT — ver el archivo `LICENSE`.
