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
- R24 — cotejo de ingenierías obligadas vs ofrecidas.

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

## 5. Prohibición durante la carga del gobierno

Durante el arranque o resincronización no se deben abrir ni modificar documentos técnicos del cliente. Una vez terminada la carga del gobierno, el trabajo técnico puede continuar conforme al estado documental del proyecto.

Estado de violación:

`VIOLACION_DE_ARRANQUE / CONTAMINACION_DOCUMENTAL / NO_EMITIBLE`

## 6. Jerarquía

R0 gobierna a todas. R2, R5, R4 y R3 ordenan pertenencia, universo y cobertura. R7 gobierna referencias normativas. R20-R24 actúan como compuertas globales según la tarea.

## 7. Estados esperados

Proyecto nuevo:

`JULCON_v13.1_BASE_LEIDA_DESDE_GITHUB_PUBLICO / GOBIERNO_BASE_ACTIVO / R20_R24_ACTIVAS / NO_EMITIBLE_HASTA_BOOTSTRAP_DE_PROYECTO`

Proyecto activo:

`JULCON_v13.1_REGLAS_ACTUALIZADAS_DESDE_GITHUB / GOBIERNO_RESINCRONIZADO / R20_R24_ACTIVAS / PROYECTO_PRESERVADO / LISTO_PARA_CONTINUAR`