THERMOREPORT VOICE PWA 0.1.0 — PROTOTIPO

Incluye:
- index.html: aplicación móvil.
- manifest.webmanifest: configuración instalable.
- sw.js: caché básica de la aplicación.

IMPORTANTE:
1. Para instalarla como PWA necesita servirse desde HTTPS (o localhost). Abrir el HTML directamente desde Archivos no instala la PWA.
2. El reconocimiento de voz depende del navegador/dispositivo y puede requerir conexión a internet. Prueba preferentemente Chrome en Android; Safari/iPhone puede tener limitaciones distintas.
3. La exportación XLSX usa SheetJS desde CDN. La primera carga necesita internet para obtener la librería; si no está disponible, se ofrece CSV compatible con Excel.
4. La app genera Hoja1 con las columnas A–H y encabezado de dos filas, sin columnas auxiliares I–J. Revisa la exportación con una copia de trabajo antes de usarla en ThermoReport.
5. La interpretación automática del dictado es básica: di explícitamente “Equipo…”, “Identificación…” y “Capacidad…”, separados por pausas o comas, y revisa siempre los campos antes de guardar.
6. Los datos quedan guardados en el almacenamiento local del navegador. Exporta respaldos JSON y Excel; borrar los datos del navegador puede eliminarlos.
7. Esto es un prototipo inicial, no una versión validada para uso crítico en campo.

Para instalar en un sitio HTTPS:
- Sube el contenido de esta carpeta a un hosting HTTPS.
- Abre la URL en el celular.
- Android/Chrome: menú ⋮ > Instalar aplicación / Añadir a pantalla principal.
- iPhone/Safari: Compartir > Añadir a pantalla de inicio.

Columnas basadas en el Excel compartido:
A AREA O DEPARTAMENTO
B EQUIPO
C IDENTIFICACIÓN
D CAPACIDAD
E/F ESTADO: On / Off
G PRIORIDAD / PUNTO
H OBSERVACIONES
I/J no se generan porque en el libro de origen son columnas auxiliares con fórmulas.
