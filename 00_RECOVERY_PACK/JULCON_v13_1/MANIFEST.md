# MANIFEST — JULCON v13.1

**Estado:** MANIFEST_CANONICO / USO_INTERNO / NO_EMITIBLE

## 1. Propósito

Este manifest lista el paquete base que debe leerse al iniciar un proyecto nuevo o retomar un proyecto activo.

## 2. Archivos de arranque

- `CLAUDE.md`
- `00_RECOVERY_PACK/CURRENT.md`
- `00_RECOVERY_PACK/JULCON_v13_1/MANIFEST.md`
- `PLANTILLAS/CLAUDE_BOOTSTRAP_JULCON_v13_1_PROYECTO_NUEVO_GITHUB_ONLY.md`

## 3. Reglas base obligatorias

Leer primero:

- `00_RECOVERY_PACK/JULCON_v13_1/REGLAS_BASE/README.md`

Después leer todas las reglas presentes en `00_RECOVERY_PACK/JULCON_v13_1/REGLAS_BASE/`, incluyendo como mínimo:

- R0, R2, R3, R4, R5 y R7
- R20 — inicialización y fuente rectora
- R21 — actualización en sitio
- R22 — homologación de fuga
- R23 — auditoría de cantidades
- R24 — ingenierías obligadas vs ofrecidas
- R25 — revisión independiente por especialista senior

Al crear un proyecto nuevo, las reglas se copian o adaptan al gobierno del proyecto. Al retomar un proyecto activo, se relee HEAD y se resincroniza el motor de reglas sin borrar contexto técnico, RFIs, inventarios, hallazgos ni decisiones.

## 4. Compuertas

R0 gobierna la cobertura. R7 gobierna referencias normativas. R20 gobierna inicialización y fuente rectora. R21-R24 gobiernan edición, aislamiento, cantidades e ingenierías. R25 exige una segunda revisión técnica independiente antes de ratificar entregables críticos.

## 5. Estado de arranque requerido

`JULCON_v13.1_BASE_LEIDA_DESDE_GITHUB_PUBLICO / GOBIERNO_BASE_ACTIVO / R20_R25_ACTIVAS / NO_EMITIBLE_HASTA_BOOTSTRAP_DE_PROYECTO`