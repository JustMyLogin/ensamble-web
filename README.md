# Ensamble V26 — compatible con archivos en raíz de GitHub

Este paquete está diseñado para repositorios en los que `index.html`, `Dockerfile` y las imágenes `.webp` están todos en la raíz (sin carpeta `assets`).

## Pasos
1. Sube los archivos del ZIP directamente a la raíz del mismo repositorio en GitHub, reemplazando `index.html`.
2. Conserva el `Dockerfile` (puerto 80), sube todos los WebP si faltan.
3. Vuelve a desplegar en Dokploy. Si aparece la versión antigua, fuerza un recargado (Ctrl + F5).

El código usa rutas relativas a la raíz como `hero-ensamble.webp` y `ensamble-logo.webp`.
