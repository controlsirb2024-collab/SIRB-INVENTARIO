# SIRB · Almacén

Inventario: https://controlsirb2024-collab.github.io/SIRB-INVENTARIO/

Interfaz web responsiva de inventario, entradas, salidas e historial. Identidad SIRB: Especialistas en chillers.

Los archivos de esta carpeta son la interfaz compilada. La información se guarda en la base de datos del servidor https://sirb-almacen-inventario.controlsirb2024.chatgpt.site; no se guarda en este repositorio ni únicamente en el navegador. Ambas direcciones consultan los mismos datos. El servidor original debe permanecer disponible.

Para actualizar: modificar el proyecto fuente SIRB, ejecutar `npm run build:pages` y subir el contenido de `pages-dist`. Los archivos principales del proyecto fuente son `app/page.tsx` (interfaz), `app/globals.css` (estilos), `public/sirb-logo.png` (logo) y `app/api/inventory/route.ts` (servidor). Evitar editar manualmente los archivos compilados index-*.js.

GitHub Pages publica la rama main y la carpeta raíz. No se necesita App Store.
