# Reglas del proyecto (para cualquier agente: Antigravity, Claude, Codex)

## Qué es este proyecto
Negocio de Tomás Urrutia: sitios web para locales + tarjetas de reseñas Google (NFC + QR), QR WiFi y cortadores/sellos de galletas impresos en 3D.
Esta carpeta guarda el **sitio web de muestra** del negocio y, después, los sitios de clientes (una subcarpeta por cliente).

## Cómo trabajamos (dos IA + Tomás)
1. **Antigravity construye**: trabaja siempre en una rama nueva (`git checkout -b nombre-tarea`), nunca directo en `main`.
2. Al terminar una tarea, hace **commit** con un mensaje claro en español (qué cambió y por qué).
3. **Claude revisa** esa rama: errores, seguridad, que se vea bien en celular, textos.
4. Se corrige lo que Claude encuentre.
5. **Tomás aprueba** y recién ahí se une a `main` (`git merge`).

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
