# web-negocio

Proyecto de Tomás Urrutia trabajado entre **Antigravity** (construye) y **Claude** (revisa), con **Git** guardando cada paso.

## El ciclo (repetir en cada tarea)
1. En Antigravity: "crea la rama `tarea-x` y haz ___". Él trabaja y hace commit.
2. En Claude: "revisa la rama `tarea-x`".
3. Se corrige lo que salga.
4. Tú apruebas y se une a `main`.

## Comandos Git que vas a usar (en la terminal)
| Comando | Qué hace |
|---|---|
| `git status` | Qué archivos cambiaron |
| `git checkout -b tarea-x` | Crea una rama nueva para una tarea |
| `git add .` | Prepara todos los cambios |
| `git commit -m "mensaje"` | Guarda una "foto" de los cambios |
| `git log --oneline` | Lista de fotos guardadas |
| `git checkout main` | Vuelve a la rama principal |
| `git merge tarea-x` | Une la tarea aprobada a `main` |

## Carpetas
- `muestra/` sitio de muestra · `clientes/` un sitio por cliente · `docs/` notas
