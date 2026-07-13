# CLAUDE BOOTSTRAP â€” JULCON v13.1 / PROYECTO NUEVO / GITHUB ONLY

**Estado:** PLANTILLA_CANONICA_GITHUB_ONLY / NO_EMITIBLE / USO_INTERNO

## 1. Mandato

Para proyecto nuevo, la fuente del sistema debe tomarse exclusivamente desde GitHub.

No usar memoria de chat como verdad operativa.
No usar archivos adjuntos como sustituto del sistema.
No pedir que el usuario suba los archivos de arranque al chat.
No pedir tokens pegados en conversaciÃ³n.
No leer documentos del cliente durante el arranque.

## 2. Fuente obligatoria

Repositorio fuente:

`jcdlmty1978-coder/JULCON-System`

Archivo de entrada:

`CLAUDE.md`

El agente debe buscar y leer, desde GitHub, en este orden:

1. `CLAUDE.md`
2. `00_RECOVERY_PACK/CURRENT.md`
3. `00_RECOVERY_PACK/JULCON_v13_1/MANIFEST.md`
4. `00_RECOVERY_PACK/JULCON_v13_1/REGLAS_BASE/README.md`
5. `PLANTILLAS/CLAUDE_BOOTSTRAP_JULCON_v13_1_PROYECTO_NUEVO.md`
6. Reglas R0, R2, R3, R4 y R5 indicadas por el manifest.

## 3. Si GitHub no estÃ¡ disponible

Si la sesiÃ³n no tiene conector, OAuth, GitHub App, GitHub CLI autenticado, clone local autenticado o acceso raw autorizado al repositorio, el agente debe detenerse.

Estado Ãºnico permitido:

`GITHUB_SOURCE_REQUIRED / GITHUB_NO_DISPONIBLE / BASELINE_NO_CARGADA / NO_EMITIBLE`

No ofrecer vÃ­a B manual como sustituto.
No pedir adjuntos.
No pedir Drive.
No pedir tokens pegados.
No fabricar estructura de proyecto.
No activar reglas no leÃ­das desde GitHub.

## 4. QuÃ© debe pedir en lugar de archivos

El agente debe pedir Ãºnicamente que se habilite una vÃ­a de acceso GitHub:

1. Conector GitHub / OAuth autorizado al repositorio.
2. GitHub App autorizada al repositorio.
3. GitHub CLI local autenticado con `gh auth login` y repo clonado.
4. Repo espejo pÃºblico de solo lectura para archivos base no sensibles.

## 5. ProhibiciÃ³n de documentos cliente

Durante el arranque queda prohibido leer, abrir, analizar, citar, comparar, resumir, despiezar o modificar propuestas, cotizaciones, PDFs tÃ©cnicos, anexos, catÃ¡logos, planos, hojas de costo o documentos del cliente.

Estado si se toca un documento del cliente antes de terminar arranque:

`VIOLACION_DE_ARRANQUE / CONTAMINACION_DOCUMENTAL / NO_EMITIBLE`

## 6. Estado exitoso esperado

Cuando GitHub sÃ­ estÃ© disponible, despuÃ©s de leer la fuente, el agente debe declarar:

`JULCON_v13.1_BASE_LEIDA_DESDE_GITHUB / GOBIERNO_BASE_ACTIVO / NO_EMITIBLE_HASTA_BOOTSTRAP_DE_PROYECTO`

Luego podrÃ¡ crear o verificar:

`PROYECTOS/<NOMBRE_PROYECTO>/00_GOBIERNO/`

sin tocar documentos tÃ©cnicos del cliente.
