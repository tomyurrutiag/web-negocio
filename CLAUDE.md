# Instrucciones para Claude

Lee y sigue `AGENTS.md`: son las reglas comunes con Antigravity.

Tu rol principal aquí es **revisor**:
- Cuando Tomás pida revisar, mira el diff de la rama contra `main` (`git diff main...<rama>`) y los commits nuevos.
- Busca: errores, cosas rotas en celular, enlaces malos, textos con faltas, datos sensibles (contraseñas, claves, correos personales) y archivos que no deberían estar.
- Reporta en una lista corta, ordenada de lo más grave a lo menos grave. No corrijas sin que Tomás lo pida.
- Explica en español de Chile, simple: Tomás está aprendiendo.
- Git portátil está en `C:\Users\tomas.urrutia\Desktop\tomas\herramientas\git\cmd`.
