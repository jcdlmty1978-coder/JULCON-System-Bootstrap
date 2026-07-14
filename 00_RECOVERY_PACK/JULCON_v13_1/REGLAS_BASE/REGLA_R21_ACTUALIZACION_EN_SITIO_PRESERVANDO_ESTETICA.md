# REGLA R21 — ACTUALIZACIÓN EN SITIO PRESERVANDO ESTÉTICA

**Sistema:** JULCON v13.1  
**Ámbito:** REGLA_GLOBAL / REGLA_BASE_CANONICA  
**Estado:** REGLA_PROTEGIDA / ACTIVA

## 1. Criterio rector

Al actualizar el Libro Maestro o cualquier entregable existente, se debe editar el archivo vigente **EN SITIO**, preservando su estética y plantilla: fuentes, colores, fills, merges, anchos de columna, alturas de fila, orden de hojas, estructura, logotipos e imágenes embebidas.

## 2. Cláusulas obligatorias

1. Prohibido reconstruir el entregable en un archivo nuevo con formato propio del agente. La actualización debe ser quirúrgica y heredar el estilo existente.
2. Si la extensión es engañosa, se debe detectar el tipo real mediante firma o *magic bytes* y usar la herramienta correcta.
3. Antes de guardar, se debe verificar que la herramienta preserva medios embebidos, drawings y relaciones. Si no los preserva, se debe usar parcheo XML directo u otro método no destructivo.
4. La verificación post-edición es obligatoria: diff celda a celda contra el original. Solo pueden diferir las celdas intencionalmente modificadas; se debe contar y reportar cada diferencia.
5. Se debe conservar una copia binaria íntegra del original.
6. No hay cumplimiento si se pierden imágenes, logotipos, fórmulas, nombres definidos, vínculos, formatos condicionales, validaciones o configuración de impresión.

## 3. Evidencia mínima

- Archivo original identificado.
- Tipo real verificado.
- Método de edición registrado.
- Conteo de celdas modificadas.
- Confirmación de preservación de medios.
- Comparación post-edición.

## 4. Estado operativo

`R21_ACTIVA / ACTUALIZACION_EN_SITIO / ESTETICA_Y_MEDIOS_PRESERVADOS / DIFF_POST_EDICION_OBLIGATORIO`