# Reglas del proyecto (para cualquier agente: Antigravity, Claude, Codex)

## Qué es este proyecto
Negocio de Tomás Urrutia: sitios web para locales + tarjetas de reseñas Google (NFC + QR), QR WiFi y cortadores/sellos de galletas impresos en 3D.
Esta carpeta guarda el **sitio web de muestra** del negocio y, después, los sitios de clientes (una subcarpeta por cliente).

## Cómo trabajamos (tres IA + Tomás, desde el 27-11)
Tomás le habla a Claude; Claude reparte. Nombres en Herdr: `claude-conecta`, `codex-conecta`, `agy-conecta`.

**Roles según fortalezas:**
- **Antigravity / Gemini (agy) — construye el diseño.** Maqueta y estilo visual, secciones nuevas, imágenes y textos de venta; investiga en internet referencias y competencia.
- **Codex — parte técnica.** JavaScript (idiomas, botones de WhatsApp, formularios), rendimiento, accesibilidad, que nada se rompa; además es el segundo revisor técnico.
- **Claude — jefe y revisor final.** Reparte las tareas, revisa cada rama (errores, seguridad, celular, textos en español) y le resume a Tomás.

**Pasos:**
1. Quien construye trabaja siempre en una rama nueva (`git checkout -b nombre-tarea`), nunca directo en `main`.
2. Al terminar una tarea, hace **commit** con un mensaje claro en español (qué cambió y por qué).
3. **Codex y Claude revisan** esa rama (Codex lo técnico; Claude lo final).
4. Se corrige lo que encuentren.
5. **Tomás aprueba** y recién ahí se une a `main` (`git merge`).
6. Dos IA no editan el mismo archivo al mismo tiempo.

## Reglas
- Idioma del sitio y de los commits: **español de Chile**, simple y claro.
- **Nunca** escribir contraseñas, claves de WiFi, tokens ni datos personales en archivos del proyecto ni en commits. Van en el gestor de contraseñas de Tomás.
- Todo sitio debe verse bien en **celular** primero.
- Cada cambio, pequeño y en su propio commit. No mezclar tareas distintas en un mismo commit.
- No borrar archivos de otra tarea sin preguntar.
- Si algo no está claro, preguntar a Tomás antes de inventar.

## Estructura
- `muestra/` — sitio de muestra del negocio de Tomás.
- `clientes/<nombre-cliente>/` — un sitio por cliente.
- `docs/` — notas, cotizaciones y guías.

## Bitácora compartida (27-11)
- Todas las IA usan `docs/bitacora-equipo.md`: **leen las últimas entradas antes de empezar** y **agregan una entrada arriba al terminar** cada tarea (fecha y hora, quién, qué hizo, archivos, qué falta). Así cada una sabe lo que hicieron las otras, y Tomás lo lee en Obsidian.
