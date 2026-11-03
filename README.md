# Ensamble — sitio estático para Dokploy

Archivos: `index.html` (web completa) y `Dockerfile` (Nginx en puerto 80).

## Publicar

1. Sube el contenido de esta carpeta a la raíz de un repositorio GitHub/Git.
2. En Dokploy, crea Project > Application y selecciona el servidor de despliegue.
3. En Source, conecta el repositorio y la rama principal.
4. En Build Type selecciona Dockerfile (`./Dockerfile`) y despliega.
5. En Domains, añade tu dominio y configura `Container Port = 80`, `Path = /`, `HTTPS = ON`, `Certificate = Let's Encrypt`.
6. En tu proveedor DNS crea `A @ -> IP pública del servidor que aloja la aplicación` (y opcionalmente `CNAME www -> @`).
7. Comprueba el certificado, el configurador y el enlace a WhatsApp.

Para usar server1, agrégalo a Dokploy de server0 como Deployment Server (SSH) y selecciona server1 en la app; el DNS debe apuntar a la IP pública de server1.

## Consideraciones

El sitio contiene imágenes integradas en el HTML (render residencial). Las imágenes de referencia externas (Unsplash) y tipografías Google necesitan conexión a internet. El botón de WhatsApp utiliza +52 686 397 1874. No hace falta un backend ni base de datos.
