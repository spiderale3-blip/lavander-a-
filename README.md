# Lavanderías Unidas de Colombia · Gestión

Sistema web para administrar clientes, servicios, órdenes, abonos, recibos, inventario, proveedores, personal y gastos. Funciona con HTML, CSS y JavaScript, sin instalación de dependencias.

## Archivos

- `index.html`: página de entrada.
- `style.css`: diseño y estilos para impresión.
- `app.js`: formularios, órdenes, recibos, cálculos y almacenamiento.
- `excel.js`: generación de archivos Excel .xlsx sin servicios externos.
- `.nojekyll`: permite servir estos archivos directamente en GitHub Pages.
- `.gitignore`: excluye respaldos y archivos de trabajo para reducir subidas accidentales de datos.

## Subir al repositorio

1. Descomprime el ZIP.
2. Crea tu repositorio en GitHub.
3. Sube el contenido de esta carpeta a la raíz del repositorio: `index.html` debe quedar directamente en la raíz, junto a los demás archivos.
4. Guarda los cambios en el repositorio.
5. Si quieres abrirla mediante una dirección web, configura un alojamiento estático, por ejemplo GitHub Pages, para servir la raíz de la rama donde subiste los archivos. Un repositorio por sí solo almacena el código; no publica automáticamente la página.

Para editarla, modifica los archivos del repositorio y guarda una nueva versión. Los enlaces a estilos y scripts son relativos, por lo que funcionan también cuando el alojamiento utiliza una subcarpeta del repositorio.

## MUY IMPORTANTE: código y datos son diferentes

**GitHub guarda los archivos de la aplicación. Los clientes, órdenes, recibos y demás registros de esta versión se guardan en el navegador, no en GitHub.**

Esta entrega no incluye registros introducidos en la página alojada: no se han extraído del navegador. Incluye los datos de empresa y el catálogo inicial incorporados en el código. Las tarifas quedan pendientes de confirmar.

Para trasladar registros existentes:

1. Abre la página actual en el navegador donde los registraste.
2. En **Excel y respaldos**, descarga el respaldo JSON.
3. Abre la nueva dirección de tu página.
4. En **Excel y respaldos**, selecciona **Restaurar JSON** y carga ese archivo.
5. Comprueba las órdenes, recibos y saldos antes de seguir trabajando.

Conserva el respaldo en una ubicación privada. No lo subas al repositorio ni a la carpeta pública de la página. Lo mismo aplica a Excel descargados con datos de clientes o del negocio. `.gitignore` ayuda cuando utilizas Git; no impide subir archivos manualmente por la web de GitHub.

Mantener la misma dirección y navegador conserva normalmente los datos al actualizar los archivos, pero borrar los datos del navegador, cambiar de perfil, dispositivo o dirección deja de acceder al mismo almacenamiento. Descarga respaldos regularmente y antes de actualizar.

## Acceso y uso compartido

Esta aplicación no tiene inicio de sesión ni base de datos compartida. La privacidad del alojamiento actual no se transfiere automáticamente a GitHub Pages u otro alojamiento: revisa quién podrá visitar la nueva página. Un repositorio privado por sí solo no añade un inicio de sesión a la aplicación.

Para que varias personas vean y editen la misma información desde distintos equipos, la siguiente etapa es conectar una base de datos en línea, autenticación, permisos y respaldos automáticos. No se deben incrustar contraseñas ni claves privadas en estos archivos públicos.

## Funciones

- Clientes y catálogo editable de servicios.
- Órdenes consecutivas con varios servicios, responsable, estado y entrega.
- Pagos parciales y saldos; recibos consecutivos que pueden anularse con motivo.
- Impresión de órdenes y recibos; el navegador permite guardar como PDF.
- Descarga de documentos HTML independientes.
- Inventario con entradas, salidas y mínimo de existencias.
- Proveedores, personal y gastos.
- Excel actualizado de 13 hojas con los datos guardados.
- Respaldo/restauración JSON e importación de respaldos del borrador original.
- Datos de empresa y logo configurables.

Los recibos son comprobantes internos. No procesan pagos y no son facturas electrónicas. No se han incorporado usuarios, sincronización ni conexión con la DIAN.

## Primer uso

Confirma los datos de **Empresa** y las tarifas de **Servicios**. Registra un cliente, crea una orden y registra abonos desde esa orden. Los pagos antiguos no se deducen de órdenes importadas del primer borrador porque este no registraba pagos.

## Verificación

Se comprobaron cálculos de órdenes, pagos parciales, anulaciones, inventario, importación del borrador y estructura del Excel generado. Queda pendiente comprobar visualmente la impresión y abrir una descarga en Microsoft Excel antes del uso operativo.
