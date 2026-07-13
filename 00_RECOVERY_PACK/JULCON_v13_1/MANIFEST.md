# MANIFEST â€” JULCON v13.1

**Estado:** MANIFEST_CANONICO / USO_INTERNO / NO_EMITIBLE

## 1. PropÃ³sito

Este manifest lista el paquete base que debe leerse al iniciar un proyecto nuevo o retomar un proyecto activo.

## 2. Archivos de arranque

- `CLAUDE.md`
- `00_RECOVERY_PACK/CURRENT.md`
- `00_RECOVERY_PACK/JULCON_v13_1/MANIFEST.md`
- `PLANTILLAS/CLAUDE_BOOTSTRAP_JULCON_v13_1_PROYECTO_NUEVO.md`

## 3. Reglas base obligatorias

Primero leer:

- `00_RECOVERY_PACK/JULCON_v13_1/REGLAS_BASE/README.md`

DespuÃ©s localizar y leer las reglas base canÃ³nicas dentro de `00_RECOVERY_PACK/JULCON_v13_1/REGLAS_BASE/`:

- `REGLA_R0_COBERTURA_DOCUMENTAL_EXHAUSTIVA_INVIOLABLE.md`
- `REGLA_R2_PERTENENCIA_FUENTE.md`
- `REGLA_R3_BARRIDO_SISTEMATICO_FUENTES.md`
- `REGLA_R4_INVENTARIO_ARRANQUE_OBLIGATORIO.md`
- `REGLA_R5_PERTENENCIA_PROBADA_CADENA_CARPETA.md`

Estas reglas son la fuente rectora base (`REGLA_BASE_CANONICA`). No se usa ninguna otra ubicaciÃ³n como semilla.

Al crear un proyecto nuevo, las reglas base canÃ³nicas se copian/adaptan a:

`PROYECTOS/<NOMBRE_PROYECTO>/00_GOBIERNO/`

## 4. JerarquÃ­a

1. R0 [INVIOLABLE]
2. R2
3. R5
4. R4
5. R3
6. R6, si existe en el paquete vigente

## 5. Estado de arranque requerido

DespuÃ©s de leer este manifest y localizar reglas base, el agente debe declarar:

`JULCON_v13.1_BASE_LEIDA / GOBIERNO_BASE_ACTIVO / NO_EMITIBLE_HASTA_BOOTSTRAP_DE_PROYECTO`

