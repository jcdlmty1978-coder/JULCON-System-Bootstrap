# JULCON — Compatibilidad de arranque v13.1 / avance v13.2
**Corte de control:** 2026-10-30 · **Estado:** INTERNO / NO EMITIBLE · **Ámbito:** información de arranque, no liberación de producto.

## Regla de precedencia
- **Pack canónico para proyecto nuevo:** `JULCON_v13_1`, señalado en `00_RECOVERY_PACK/CURRENT.md`. Este documento **NO cambia** `PACK_ACTIVO`.
- **v13.2:** desarrollo y pruebas controladas. Su presencia en ramas, pruebas o laboratorios **no** autoriza uso de motores sobre ingeniería real ni emisión.
- Aplicar R0, R2, R3, R4, R5, R7 y R20–R25 del pack vigente. Verificar reglas de proyecto y fuentes primarias antes de cualquier conclusión.
- Si las fuentes no demuestran un dato, reportarlo como `TBD`; separar `CONFIRMADO`, `INTERPRETACIÓN`, `SUPUESTO` y `TBD`.

## Matriz de disponibilidad para proyectos
| Capacidad | Disponibilidad de arranque | Límite |
|---|---|---|
| Gobierno documental y reglas v13.1 | DISPONIBLE | Sin suponer cobertura total si no se inventariaron todas las raíces |
| Reconocimiento preliminar de centro de carga | DISPONIBLE · PERFIL DE CAMPO | Observación autorizada; no equivalencia a ingeniería final |
| Action Register / ELT / Readiness | Desarrollo integrado en rama privada de auditoría | No convertir evidencia de laboratorio en autorización EPC real |
| Priority / Motor 4 | CANDIDATO P0 SINTÉTICO | Revisión independiente humana R25 pendiente |
| EDE / decisión ejecutiva | LABORATORIO SINTÉTICO | Recomienda; no decide ni emite |
| Document Intelligence / cálculos / dossier | EXPERIMENTAL | WORK-006 en aceptación; NO-GO hasta auditoría del candidato exacto |
| Publicación Windows F-06 | PENDIENTE | Publicación externa no habilitada |
| Catálogo de especialistas EPC | EXPERIMENTAL | Cobertura declarada no equivale a especialistas operativos |

## Integración con el cierre de hitos
| Hito | Condición objetiva | Estado al corte |
|---|---|---|
| H0: Bootstrap de visita de campo | Guía de inicio, checklist y reglas compatibles disponibles | PERFIL PREPARADO; uso específico requiere datos y autorización del proyecto |
| H1: WORK-006 | Auditoría independiente y disposición de fallos del candidato exacto, Linux/Windows y controles de consumo | PENDIENTE / NO-GO |
| H2: Priority | R25 humano válido y ratificación separada | PENDIENTE |
| H3: F-06 | Publicador Windows seguro, pruebas E2E y aceptación | PENDIENTE |
| H4: Integración de cinco capacidades | Fuente, contratos, pruebas y permisos consolidados en una versión revisada | LABORATORIO, NO PRODUCTIVO |
| H5: Piloto EPC real | Acceso/documentación autorizados, controles de integridad y validación humana | NO AUTORIZADO POR ESTA GUÍA |

## Nuevo proyecto: procedimiento permitido
1. Leer `CLAUDE.md`, `CURRENT.md`, MANIFEST y reglas base **desde GitHub**, fijando commit y hashes.
2. Iniciar expediente de proyecto en **ubicación privada autorizada** (nunca almacenar planos, RPU, fotos, datos de clientes ni archivos confidenciales en este repositorio público).
3. Para una visita inicial: `PLANTILLAS/CENTROS_DE_CARGA/ARRANQUE_PRELIMINAR_JULCON.md` y `CHECKLIST_VISITA_CENTRO_CARGA.md`.
4. Reportar universo realmente observado, vacíos y acciones pendientes; no certificar R0 exhaustivo por una visita parcial.
5. No activar motores v13.2, cálculos automáticos de emisión, RFQ/CAPEX o dictámenes por la sola lectura de este documento.

**Prohibido:** declarar v13.2 en producción, reemplazar el pack vigente, modificar Core, autoemitir R25, cerrar WORK-006 por resultados declarados por el constructor o tomar decisiones técnicas sin evidencia primaria.
