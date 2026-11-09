# Claude-Mem — copia pendiente de auditoría

Fecha local: 8 de noviembre de 2026.

Estado: NO APROBADO PARA INSTALACIÓN. Pendiente de análisis de seguridad y privacidad. Esto no equivale a afirmar que el proyecto sea malicioso.

## Procedencia y versión

- Repositorio original: https://github.com/thedotmack/claude-mem
- Copia: https://github.com/ughetty/claude-mem
- Rama copiada: main únicamente.
- Commit de origen comprobado en la copia antes de añadir esta nota: 66c8344b9083239fdcffcf9f0d1c6792630d9d74.
- Licencia y atribuciones originales conservadas. No se cambia ni se amplía la licencia de terceros.

## Medidas realizadas

- Se creó un fork en GitHub sin ejecutar instaladores, scripts ni dependencias del proyecto.
- Se desactivó GitHub Actions en Settings / Actions / General y se verificó Disable actions seleccionado tras guardar.
- No se añadieron credenciales, llaves SSH, secretos, historial de trabajo ni archivos privados.
- No se habilitó Claude-Mem como plugin, skill, MCP ni servicio; no se configuraron proveedores ni sincronización.
- Esta nota es el único cambio intencional al contenido copiado. El código original permanece pendiente de revisión.

## Pendientes para una futura auditoría

1. Revisar instalador, scripts de ciclo de vida y dependencias sin ejecutarlos.
2. Revisar hooks, procesos persistentes, API local, autenticación, permisos y rutas de archivos.
3. Verificar en código la telemetría, conservación de imágenes, exclusión de secretos y destino de datos según proveedor; no basta con el README.
4. Revisar cómo se separa la memoria entre proyectos y cómo se evita tratar contenido recuperado como autorización o instrucciones de mayor prioridad.
5. Comprobar actualizaciones, descargas y dependencias transitivas; fijar versiones antes de probar.
6. Si la revisión lo justifica, probar exclusivamente en un entorno desechable sin cuentas conectadas, medios privados ni secretos, con acceso de red restringido.

No instalar desde esta copia ni desde latest hasta terminar la revisión y decidir explícitamente su uso. Copiar o desactivar Actions no certifica la seguridad del código. No se creó una automatización de sincronización con el original; cualquier actualización futura requiere comparar y revisar sus cambios.
