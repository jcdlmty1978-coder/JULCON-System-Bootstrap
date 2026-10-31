# CLAUDE.md — ARRANQUE CANÓNICO JULCON v13.1

**Estado:** ARRANQUE_CANONICO / USO_INTERNO / NO_EMITIBLE

Este archivo es el punto de entrada para cualquier sesión que use el bootstrap público.

## 1. Mandato de arranque o resincronización

Antes de analizar, despiezar, comparar, emitir RFI, cerrar frentes o generar entregables, el agente debe:

1. Leer `CLAUDE.md` completo.
2. Leer `00_RECOVERY_PACK/CURRENT.md`.
3. Leer `00_RECOVERY_PACK/JULCON_v13_1/MANIFEST.md`.
4. Leer `00_RECOVERY_PACK/JULCON_v13_1/REGLAS_BASE/README.md`.
5. Leer `PLANTILLAS/CLAUDE_BOOTSTRAP_JULCON_v13_1_PROYECTO_NUEVO_GITHUB_ONLY.md`.
6. Leer todas las reglas presentes en `00_RECOVERY_PACK/JULCON_v13_1/REGLAS_BASE/`.
7. Reportar commit HEAD, rutas, estado de lectura y blob SHA cuando esté disponible.

No se permite usar memoria de chat como versión vigente de las reglas.

## 2. Reglas mínimas obligatorias

Deben quedar activas, como mínimo:

- R0, R2, R3, R4, R5 y R7;
- R20 — inicialización y fuente rectora por objeto de decisión;
- R21 — actualización en sitio preservando estética;
- R22 — homologación de distancia de fuga al valor más severo;
- R23 — auditoría de cantidades contra rector;
- R24 — cotejo de ingenierías obligadas vs ofrecidas;
- R25 — revisión obligatoria por especialista senior independiente.

El manifest y el índice gobiernan si aparecen reglas adicionales.

## 3. Proyecto nuevo

Después de cargar el sistema, crear o verificar:

`PROYECTOS/<NOMBRE_PROYECTO>/00_GOBIERNO/`

Ahí debe quedar el gobierno mínimo del proyecto: bootstrap, reglas aplicables, registro de reglas, raíces documentales y estado de arranque.

## 4. Proyecto o chat activo

Al resincronizar un chat ya iniciado:

- preservar contexto técnico, RFIs, inventarios, hallazgos y decisiones;
- releer HEAD vigente;
- actualizar únicamente el motor de reglas;
- continuar desde el punto previo con las reglas nuevas.

## 5. Gate R25

Cuando el trabajo sea crítico, separar expresamente:

- `ROL_CONSTRUCTOR`;
- `ROL_REVISOR_SENIOR_INDEPENDIENTE`.

El revisor senior debe consultar fuentes directamente, desafiar el trabajo y registrar hallazgos, discrepancias y estado. Una revisión por IA no sustituye firma profesional, autoridad competente ni ratificación del director EPC cuando corresponda.

Si R25 aplica y no se ejecuta:

`REVISION_SENIOR_NO_EJECUTADA / RATIFICACION_BLOQUEADA / NO_EMITIBLE`

## 6. Prohibición durante la carga del gobierno

Durante el arranque o resincronización no se deben abrir ni modificar documentos técnicos del cliente. Una vez terminada la carga del gobierno, el trabajo técnico puede continuar conforme al estado documental del proyecto.

## 7. Jerarquía

R0 gobierna a todas. R2, R5, R4 y R3 ordenan pertenencia, universo y cobertura. R7 gobierna referencias normativas. R20-R25 actúan como compuertas globales según la tarea.

## 8. Estados esperados

Proyecto nuevo:

`JULCON_v13.1_BASE_LEIDA_DESDE_GITHUB_PUBLICO / GOBIERNO_BASE_ACTIVO / R20_R25_ACTIVAS / NO_EMITIBLE_HASTA_BOOTSTRAP_DE_PROYECTO`

Proyecto activo:

`JULCON_v13.1_REGLAS_ACTUALIZADAS_DESDE_GITHUB / GOBIERNO_RESINCRONIZADO / R20_R25_ACTIVAS / PROYECTO_PRESERVADO / LISTO_PARA_CONTINUAR`

## 9. Perfil de centro de carga — visita preliminar (compatibilidad al 2026-10-30)

Para una nueva visita a centro de carga, después de cargar v13.1 y las reglas base, leer:
- `00_RECOVERY_PACK/ESTADO_COMPATIBILIDAD_v13_2_20261030.md`;
- `PLANTILLAS/CENTROS_DE_CARGA/ARRANQUE_PRELIMINAR_JULCON.md`;
- `PLANTILLAS/CENTROS_DE_CARGA/CHECKLIST_VISITA_CENTRO_CARGA.md`.
- Para visita del 4 de noviembre de 2026, consultar `PLANTILLAS/CENTROS_DE_CARGA/ARRANQUE_VISITA_20261104.md`.

**La versión canónica continúa siendo v13.1.** Estas plantillas NO promueven motores v13.2, no autorizan uso EPC real de componentes experimentales, ni sustituyen R25. Nunca colocar datos o documentos de cliente en este repositorio público. El estado de hitos está en el documento de compatibilidad.
