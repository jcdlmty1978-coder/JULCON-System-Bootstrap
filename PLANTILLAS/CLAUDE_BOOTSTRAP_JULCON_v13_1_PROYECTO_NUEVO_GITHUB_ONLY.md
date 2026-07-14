# CLAUDE BOOTSTRAP — JULCON v13.1 / PROYECTO NUEVO / GITHUB ONLY

**Estado:** PLANTILLA_CANONICA_GITHUB_ONLY / NO_EMITIBLE / USO_INTERNO

## 1. Mandato

Para proyecto nuevo, la fuente del sistema debe tomarse exclusivamente desde GitHub público.

No usar memoria de chat como verdad operativa.  
No usar archivos adjuntos como sustituto del sistema.  
No pedir que el usuario suba los archivos de arranque al chat.  
No pedir tokens pegados en conversación.  
No leer documentos del cliente durante el arranque.

## 2. Fuente obligatoria

Repositorio fuente público:

`jcdlmty1978-coder/JULCON-System-Bootstrap`

Archivo de entrada:

`CLAUDE.md`

El agente debe releer `HEAD` vigente al inicio de cada proyecto o chat nuevo y buscar/leer, desde GitHub, en este orden:

1. `CLAUDE.md`
2. `00_RECOVERY_PACK/CURRENT.md`
3. `00_RECOVERY_PACK/JULCON_v13_1/MANIFEST.md`
4. `00_RECOVERY_PACK/JULCON_v13_1/REGLAS_BASE/README.md`
5. `PLANTILLAS/CLAUDE_BOOTSTRAP_JULCON_v13_1_PROYECTO_NUEVO_GITHUB_ONLY.md`
6. Todas las reglas base canónicas listadas en el manifest y presentes en `REGLAS_BASE/`, incluyendo R0, R2, R3, R4, R5 y R7.

No debe reutilizar como vigentes reglas leídas en otro chat sin volver a consultar `HEAD`.

## 3. Si GitHub no está disponible

Si la sesión no tiene acceso público raw/clone al repositorio, el agente debe detenerse.

Estado único permitido:

`BOOTSTRAP_PUBLICO_NO_ACCESIBLE / BASELINE_NO_CARGADA / NO_EMITIBLE`

No ofrecer vía B manual como sustituto.  
No pedir adjuntos.  
No pedir Drive.  
No pedir tokens pegados.  
No fabricar estructura de proyecto.  
No activar reglas no leídas desde GitHub.

## 4. Reporte de actualización en cada arranque

El agente debe reportar:

- commit `HEAD` leído;
- ruta y estado de cada archivo requerido;
- `blob SHA` cuando esté disponible;
- reglas base localizadas;
- confirmación de que no se tocaron documentos del cliente.

Si un proyecto activo fue iniciado con un commit anterior, debe declarar:

`REGLAS_BASE_ACTUALIZADAS_DISPONIBLES / RELECTURA_REQUERIDA`

y releer las reglas vigentes antes de continuar. La adaptación del gobierno local del proyecto debe quedar trazada.

## 5. Prohibición de documentos cliente

Durante el arranque queda prohibido leer, abrir, analizar, citar, comparar, resumir, despiezar o modificar propuestas, cotizaciones, PDFs técnicos, anexos, catálogos, planos, hojas de costo o documentos del cliente.

Estado si se toca un documento del cliente antes de terminar arranque:

`VIOLACION_DE_ARRANQUE / CONTAMINACION_DOCUMENTAL / NO_EMITIBLE`

## 6. Estado exitoso esperado

Cuando GitHub esté disponible, después de leer la fuente y todas las reglas base vigentes, el agente debe declarar:

`JULCON_v13.1_BASE_LEIDA_DESDE_GITHUB_PUBLICO / GOBIERNO_BASE_ACTIVO / NO_EMITIBLE_HASTA_BOOTSTRAP_DE_PROYECTO`

Luego podrá crear o verificar:

`PROYECTOS/<NOMBRE_PROYECTO>/00_GOBIERNO/`

sin tocar documentos técnicos del cliente hasta cerrar el bootstrap correspondiente.
