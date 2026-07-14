# REGLAS_BASE — JULCON v13.1

**Estado:** INDICE_BASE / USO_INTERNO / NO_EMITIBLE

Esta carpeta concentra las reglas base que debe activar todo proyecto nuevo.

Reglas base canónicas (`REGLA_BASE_CANONICA`) presentes en esta carpeta:

- `REGLA_R0_COBERTURA_DOCUMENTAL_EXHAUSTIVA_INVIOLABLE.md` — Cobertura documental exhaustiva [INVIOLABLE].
- `REGLA_R2_PERTENENCIA_FUENTE.md` — Pertenencia de fuente.
- `REGLA_R3_BARRIDO_SISTEMATICO_FUENTES.md` — Barrido sistemático de fuentes.
- `REGLA_R4_INVENTARIO_ARRANQUE_OBLIGATORIO.md` — Inventario de arranque obligatorio.
- `REGLA_R5_PERTENENCIA_PROBADA_CADENA_CARPETA.md` — Pertenencia probada por cadena de carpeta.
- `REGLA_R7_VERIFICACION_OBLIGATORIA_NORMA_ESPECIFICACION_FUENTE_PRIMARIA.md` — Verificación obligatoria de norma/especificación en fuente primaria.

Esta carpeta es la fuente rectora base. Para un proyecto nuevo, el agente copia/adapta estas reglas al gobierno del proyecto en `PROYECTOS/<NOMBRE_PROYECTO>/00_GOBIERNO/` antes de trabajar. No se usa ninguna otra ubicación como semilla.
