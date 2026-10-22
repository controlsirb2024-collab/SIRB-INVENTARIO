# SIRB · Almacén

https://controlsirb2024-collab.github.io/SIRB-INVENTARIO/

Inventario, entradas, salidas e historial con usuarios y contraseñas propios. La información se guarda en el servidor Sites de SIRB y requiere iniciar sesión; no está almacenada en este repositorio.

El administrador crea cuentas desde **Usuarios**, define su perfil y asigna una contraseña temporal de al menos 12 caracteres. Cada usuario cambia esa contraseña al entrar por primera vez. **Desactivar** bloquea una cuenta; **Restablecer contraseña** revoca sus sesiones y asigna una nueva contraseña temporal. **Mi contraseña** permite cambiar la propia.

Operador: gestiona materiales y movimientos. Administrador: además gestiona usuarios. No existe registro público. El primer administrador se crea con un enlace privado de activación entregado al dueño; nunca subir ese enlace aquí.

Archivos compilados de la interfaz. Para actualizar: modificar el proyecto fuente SIRB y ejecutar `npm run build:pages`; publicar los archivos de `pages-dist`. API y base de datos: https://sirb-almacen-inventario.controlsirb2024.chatgpt.site. El servidor debe permanecer disponible.


## Sucursales y transferencias

El admin general selecciona Querétaro o San Luis Potosí. Cada encargado administra solo su sucursal asignada.

En Transferencias, el origen registra material, cantidad, responsable y fecha. La solicitud queda pendiente sin modificar existencias. El destino confirma la recepción: se descuenta del origen y se suma al destino en una sola operación con validación de stock. El origen puede cancelar solicitudes pendientes. Los movimientos vinculados conservan la trazabilidad y no se eliminan por separado.
