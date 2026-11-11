# CLAUDE BOOTSTRAP — JULCON v13.2 / PROYECTO NUEVO / GITHUB ONLY

**Estado:** PLANTILLA_CANONICA_GITHUB_ONLY / NO_EMITIBLE / USO_INTERNO

## 1. Mandato

Para proyecto nuevo, la fuente del sistema debe tomarse exclusivamente desde GitHub.

No usar memoria de chat como verdad operativa.
No usar archivos adjuntos como sustituto del sistema.
No pedir que el usuario suba los archivos de arranque al chat.
No pedir tokens pegados en conversación.
No leer documentos del cliente durante el arranque.

## 2. Fuente obligatoria

Repositorio fuente:

`JULCON-ENTERPRISES/plataforma JULCON`

Archivo de entrada:

`CLAUDE.md`

El agente debe buscar y leer, desde GitHub, en este orden:

1. `CLAUDE.md`
2. `ARRANQUE.md`
3. `00_RECOVERY_PACK/CURRENT.md`
4. El índice `REGLAS.yaml` y los textos completos de las reglas vigentes conforme a `CURRENT.md` y `ARRANQUE.md`.
5. `REGLAS.yaml` y textos íntegros aplicables, incluyendo R0, R2, R3, R4, R5, R7-N, R20–R25 y RD-001 en la versión ratificada.
6. `PLANTILLAS/CLAUDE_BOOTSTRAP_JULCON_PROYECTO_NUEVO.md`.

## 3. Si GitHub no está disponible

Si la sesión no tiene conector, OAuth, GitHub App, GitHub CLI autenticado, clone local autenticado o acceso raw autorizado al repositorio, el agente debe detenerse.

Estado único permitido:

`GOBIERNO_NO_CARGADO / NO_EMITIBLE`

Motivo técnico de bloqueo, si corresponde: `GITHUB_SOURCE_REQUIRED / GITHUB_NO_DISPONIBLE / BASELINE_NO_CARGADA`.

No ofrecer vía B manual como sustituto.
No pedir adjuntos.
No pedir Drive.
No pedir tokens pegados.
No fabricar estructura de proyecto.
No activar reglas no leídas desde GitHub.

## 4. Qué debe pedir en lugar de archivos

El agente debe pedir únicamente que se habilite una vía de acceso GitHub:

1. Conector GitHub / OAuth autorizado al repositorio.
2. GitHub App autorizada al repositorio.
3. GitHub CLI local autenticado con `gh auth login` y repo clonado.
4. Repo espejo público de solo lectura para archivos base no sensibles.

## 5. Prohibición de documentos cliente

Durante el arranque queda prohibido leer, abrir, analizar, citar, comparar, resumir, despiezar o modificar propuestas, cotizaciones, PDFs técnicos, anexos, catálogos, planos, hojas de costo o documentos del cliente.

Estado si se toca un documento del cliente antes de terminar arranque:

`VIOLACION_DE_ARRANQUE / CONTAMINACION_DOCUMENTAL / NO_EMITIBLE`

## 6. Estado exitoso esperado

Cuando GitHub sí esté disponible, después de leer la fuente, el agente debe declarar:

`JULCON_v13.2_NUEVO / GOBIERNO_LEIDO / NO_EMITIBLE_HASTA_INVENTARIO_Y_COBERTURA`

Luego podrá crear o verificar:

`PROYECTOS/<NOMBRE_PROYECTO>/00_GOBIERNO/`

sin tocar documentos técnicos del cliente.
## Estado de proyecto activo

Cuando se retoma un proyecto, usar el único estado de proyecto activo definido en `ARRANQUE.md` y la evidencia real de recuperación; no tratar la plantilla como orden de cambiar `CURRENT.md`.
