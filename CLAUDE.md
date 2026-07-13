# CLAUDE.md â€” ARRANQUE CANÃ“NICO JULCON v13.1

**Estado:** ARRANQUE_CANÃ“NICO / USO_INTERNO / NO_EMITIBLE

Este archivo es el punto de entrada para cualquier sesiÃ³n de trabajo sobre este repositorio.

## 1. Mandato de arranque

Antes de analizar, despiezar, comparar, emitir RFI, cerrar frentes, declarar gaps o generar entregables, el agente debe:

1. Leer `CLAUDE.md` completo.
2. Leer `00_RECOVERY_PACK/CURRENT.md`.
3. Leer el `MANIFEST.md` del Recovery Pack vigente indicado por `CURRENT.md`.
4. Leer las reglas base JULCON v13.1 indicadas por el manifest.
5. Leer o crear el bootstrap del proyecto activo en `PROYECTOS/<NOMBRE_PROYECTO>/00_GOBIERNO/`.
6. Reportar rutas, estado de lectura y SHA/commit cuando estÃ© disponible.

## 2. Recovery Pack vigente

El Recovery Pack vigente no se busca ni se infiere. Se declara en:

`00_RECOVERY_PACK/CURRENT.md`

Si `CURRENT.md` no existe, no es legible o apunta a una ruta inexistente, detenerse y reportar:

`RECOVERY_PACK_NO_RESUELTO / NO_EMITIBLE`

## 3. Proyecto nuevo

Para un proyecto nuevo, leer:

`PLANTILLAS/CLAUDE_BOOTSTRAP_JULCON_v13_1_PROYECTO_NUEVO.md`

DespuÃ©s crear o verificar:

`PROYECTOS/<NOMBRE_PROYECTO>/00_GOBIERNO/`

AhÃ­ debe quedar el gobierno mÃ­nimo del proyecto: bootstrap, reglas aplicables, registro de reglas, roots documentales y estado de arranque.

## 4. ProhibiciÃ³n de tocar propuestas en arranque

Durante el arranque canÃ³nico de un proyecto nuevo queda prohibido leer, abrir, analizar, citar, comparar, resumir, despiezar o modificar propuestas, cotizaciones, PDFs tÃ©cnicos, anexos, catÃ¡logos, planos, hojas de costo o documentos del cliente.

El arranque solo puede tocar archivos de gobierno y sistema:

- `CLAUDE.md`
- `00_RECOVERY_PACK/CURRENT.md`
- `00_RECOVERY_PACK/JULCON_v13_1/MANIFEST.md`
- `00_RECOVERY_PACK/JULCON_v13_1/REGLAS_BASE/README.md`
- `PLANTILLAS/CLAUDE_BOOTSTRAP_JULCON_v13_1_PROYECTO_NUEVO.md`
- `PROYECTOS/<NOMBRE_PROYECTO>/00_GOBIERNO/`

Las propuestas y documentos tÃ©cnicos se consideran fuera de alcance hasta completar gobierno, Recovery Pack, R0/R2/R3/R4/R5, roots documentales e inventario R4.

Estado si se toca una propuesta antes de terminar el arranque:

`VIOLACION_DE_ARRANQUE / CONTAMINACION_DOCUMENTAL / NO_EMITIBLE`

## 5. JerarquÃ­a inviolable

1. **R0 [INVIOLABLE]** â€” Cobertura documental exhaustiva.
2. **R2** â€” Pertenencia de fuente.
3. **R5** â€” Prueba por cadena de carpeta / `parentId`.
4. **R4** â€” Inventario de arranque / universo documental completo.
5. **R3** â€” Barrido sistemÃ¡tico antes de cierre.
6. **R6** â€” Recorrido descendente, si existe en el paquete vigente.

R0 gobierna a todas. Ninguna limitaciÃ³n tÃ©cnica, prisa, conveniencia, bÃºsqueda sin resultado ni lectura dirigida autoriza violar R0.

## 6. Estados por defecto

Si no se resuelve el Recovery Pack:

`RECOVERY_PACK_NO_RESUELTO / NO_EMITIBLE`

Si una fuente no tiene pertenencia probada:

`FUENTE_NO_VERIFICADA / NO_EMITIBLE`

Si un anÃ¡lisis empezÃ³ sin inventario de arranque:

`INCOMPLETO / NO_EMITIBLE`

Si un cierre se intenta sin barrido completo registrado:

`NO_VERIFICADA / NO_EMITIBLE`

Si un entregable viola R0:

`NULO / NO_VERIFICADO / NO_EMITIBLE`

## 7. Frase de control

El agente no decide el contexto: lo lee desde `CLAUDE.md` + `CURRENT.md` + `MANIFEST.md` + `BOOTSTRAP_PROYECTO.md`.

