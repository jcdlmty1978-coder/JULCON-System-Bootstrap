# CLAUDE BOOTSTRAP — JULCON v13.1 / PROYECTO NUEVO / GITHUB ONLY

**Estado:** PLANTILLA_CANONICA_GITHUB_ONLY / NO_EMITIBLE / USO_INTERNO

## 1. Mandato

Para proyecto nuevo o chat activo, la fuente del sistema se toma desde GitHub público y se relee desde HEAD vigente.

No usar memoria de chat como verdad operativa. No reutilizar reglas antiguas sin releer GitHub. No leer documentos del cliente durante la carga o resincronización del gobierno.

## 2. Fuente obligatoria

Repositorio fuente público:

`jcdlmty1978-coder/JULCON-System-Bootstrap`

Leer en este orden:

1. `CLAUDE.md`
2. `00_RECOVERY_PACK/CURRENT.md`
3. `00_RECOVERY_PACK/JULCON_v13_1/MANIFEST.md`
4. `00_RECOVERY_PACK/JULCON_v13_1/REGLAS_BASE/README.md`
5. `PLANTILLAS/CLAUDE_BOOTSTRAP_JULCON_v13_1_PROYECTO_NUEVO_GITHUB_ONLY.md`
6. Todas las reglas base canónicas presentes en `REGLAS_BASE/`.

Como mínimo deben quedar leídas y activas R0, R2, R3, R4, R5, R7 y R20-R25.

## 3. Proyecto activo

Si el chat ya contiene trabajo técnico:

- preservar contexto, RFIs, inventarios, hallazgos y decisiones;
- comparar las reglas activas contra HEAD vigente;
- sustituir únicamente el motor de reglas;
- continuar desde el punto previo aplicando las reglas actualizadas.

GitHub prevalece sobre reglas recordadas por el chat.

## 4. Gate de revisión senior

Para trabajos críticos, activar R25 y separar:

- `ROL_CONSTRUCTOR`
- `ROL_REVISOR_SENIOR_INDEPENDIENTE`

El revisor debe consultar fuentes directamente, comprobar cálculos y cantidades cuando existan, revisar interfaces y riesgos, y emitir uno de los estados autorizados por R25.

La revisión por IA no sustituye firma profesional, aprobación regulatoria ni ratificación del director EPC.

## 5. Reporte

Reportar commit HEAD, rutas, estado de lectura, blob SHA cuando esté disponible, reglas nuevas o modificadas y confirmación de preservación del proyecto.

## 6. Estados esperados

Proyecto nuevo:

`JULCON_v13.1_BASE_LEIDA_DESDE_GITHUB_PUBLICO / GOBIERNO_BASE_ACTIVO / R20_R25_ACTIVAS / NO_EMITIBLE_HASTA_BOOTSTRAP_DE_PROYECTO`

Proyecto activo:

`JULCON_v13.1_REGLAS_ACTUALIZADAS_DESDE_GITHUB / GOBIERNO_RESINCRONIZADO / R20_R25_ACTIVAS / PROYECTO_PRESERVADO / LISTO_PARA_CONTINUAR`