# REGLAS_BASE — JULCON v13.1

**Estado:** INDICE_BASE / USO_INTERNO / NO_EMITIBLE

Esta carpeta concentra las reglas base que debe activar todo proyecto nuevo o resincronizar todo proyecto activo.

Reglas base canónicas (`REGLA_BASE_CANONICA`) presentes en esta carpeta:

- `REGLA_R0_COBERTURA_DOCUMENTAL_EXHAUSTIVA_INVIOLABLE.md` — Cobertura documental exhaustiva [INVIOLABLE].
- `REGLA_R2_PERTENENCIA_FUENTE.md` — Pertenencia de fuente.
- `REGLA_R3_BARRIDO_SISTEMATICO_FUENTES.md` — Barrido sistemático de fuentes.
- `REGLA_R4_INVENTARIO_ARRANQUE_OBLIGATORIO.md` — Inventario de arranque obligatorio.
- `REGLA_R5_PERTENENCIA_PROBADA_CADENA_CARPETA.md` — Pertenencia probada por cadena de carpeta.
- `REGLA_R7_VERIFICACION_OBLIGATORIA_NORMA_ESPECIFICACION_FUENTE_PRIMARIA.md` — Verificación obligatoria de norma/especificación en fuente primaria.
- `REGLA_R20_INICIALIZACION_AGENTES_MOTORES_Y_FUENTE_RECTORA.md` — Inicialización multifuentente y fuente rectora por objeto de decisión.
- `REGLA_R21_ACTUALIZACION_EN_SITIO_PRESERVANDO_ESTETICA.md` — Actualización quirúrgica en sitio, preservando estética y medios.
- `REGLA_R22_HOMOLOGACION_FUGA_VALOR_MAS_SEVERO.md` — Homologación de distancia de fuga hacia el valor más severo.
- `REGLA_R23_AUDITORIA_CANTIDADES_CONTRA_RECTOR.md` — Auditoría de cantidades, unidades cotizables y doble conteo.
- `REGLA_R24_COTEJO_INGENIERIAS_OBLIGADAS_VS_OFRECIDAS.md` — Checklist de ingenierías obligadas contra ofrecidas.
- `REGLA_R25_REVISION_OBLIGATORIA_AGENTE_ESPECIALISTA_SENIOR_INDEPENDIENTE.md` — Segunda revisión técnica independiente por especialista senior antes de ratificación.

La numeración R20 ya estaba ocupada antes de la integración de R21-R24; se preservó la regla existente y se continuó la secuencia hasta R25.

Esta carpeta es la fuente rectora base. Para un proyecto nuevo, el agente copia o adapta estas reglas al gobierno del proyecto. Para un proyecto activo, relee HEAD y resincroniza reglas sin borrar el contexto técnico.