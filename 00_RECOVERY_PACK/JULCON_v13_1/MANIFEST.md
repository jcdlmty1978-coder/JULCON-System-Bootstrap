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

Primero leer:

- `00_RECOVERY_PACK/JULCON_v13_1/REGLAS_BASE/README.md`

Después localizar y leer **todas** las reglas base canónicas presentes dentro de `00_RECOVERY_PACK/JULCON_v13_1/REGLAS_BASE/`, incluyendo como mínimo:

- `REGLA_R0_COBERTURA_DOCUMENTAL_EXHAUSTIVA_INVIOLABLE.md`
- `REGLA_R2_PERTENENCIA_FUENTE.md`
- `REGLA_R3_BARRIDO_SISTEMATICO_FUENTES.md`
- `REGLA_R4_INVENTARIO_ARRANQUE_OBLIGATORIO.md`
- `REGLA_R5_PERTENENCIA_PROBADA_CADENA_CARPETA.md`
- `REGLA_R7_VERIFICACION_OBLIGATORIA_NORMA_ESPECIFICACION_FUENTE_PRIMARIA.md`
- `REGLA_R20_INICIALIZACION_AGENTES_MOTORES_Y_FUENTE_RECTORA.md`
- `REGLA_R21_ACTUALIZACION_EN_SITIO_PRESERVANDO_ESTETICA.md`
- `REGLA_R22_HOMOLOGACION_FUGA_VALOR_MAS_SEVERO.md`
- `REGLA_R23_AUDITORIA_CANTIDADES_CONTRA_RECTOR.md`
- `REGLA_R24_COTEJO_INGENIERIAS_OBLIGADAS_VS_OFRECIDAS.md`

Estas reglas son la fuente rectora base (`REGLA_BASE_CANONICA`). No se usa ninguna otra ubicación como semilla.

Al crear un proyecto nuevo, las reglas se copian/adaptan al gobierno del proyecto. Al retomar un proyecto activo, se relee HEAD y se resincroniza el motor de reglas sin borrar contexto técnico, RFIs, inventarios, hallazgos ni decisiones vigentes.

## 4. Jerarquía y compuertas

1. R0 [INVIOLABLE]
2. R2
3. R5
4. R4
5. R3
6. R6, si existe en el paquete vigente
7. R7 para toda norma o especificación
8. R20 como inicialización obligatoria y selección de fuente rectora
9. R21 para edición de entregables existentes
10. R22 para homologación de distancia de fuga en diseño AT
11. R23 para auditoría de cantidades y unidades cotizables
12. R24 para cotejo de ingenierías obligadas vs ofrecidas

## 5. Estado de arranque requerido

Después de leer este manifest y localizar las reglas base, el agente debe declarar:

`JULCON_v13.1_BASE_LEIDA_DESDE_GITHUB_PUBLICO / GOBIERNO_BASE_ACTIVO / R20_R24_ACTIVAS / NO_EMITIBLE_HASTA_BOOTSTRAP_DE_PROYECTO`