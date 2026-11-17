# Explorador de prompts WildChat

Página web para explorar los primeros mensajes de usuarios reales de WildChat en español, clasificados con un juez LLM (v13.1). Permite filtrar por país, dominio, categoría, tipo de tarea y dimensión de sesgo, ver conteos y descargar un Excel con el filtro aplicado.

**Países procesados:** Chile, México, Perú, Argentina, Ecuador, Venezuela y Bolivia. No son todos los países de Latinoamérica.

## Archivos
- `index.html`: la página (no cambia).
- `datos.json`: los prompts y sus anotaciones. Se genera en el repo del pipeline con `extras/construir_explorador.py`.

## Publicar (GitHub Pages)
Settings → Pages → Branch `main`, carpeta `/ (root)`.

## Actualizar los datos
Reemplaza `datos.json` por el nuevo y haz commit.

## Ver en local
`python -m http.server` en esta carpeta y abrir `http://localhost:8000` (con doble clic no carga `datos.json`).

## Privacidad
`datos.json` contiene mensajes reales de usuarios de WildChat. Revisa los términos de uso de WildChat antes de hacer público el repositorio (GitHub Pages es público).
