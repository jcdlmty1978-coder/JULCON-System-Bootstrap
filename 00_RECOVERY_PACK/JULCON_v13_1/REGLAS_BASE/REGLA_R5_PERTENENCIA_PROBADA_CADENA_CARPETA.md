# REGLA_R5 â€” PERTENENCIA PROBADA POR CADENA DE CARPETA

**Sistema:** JULCON v13.1  
**Ãmbito:** REGLA_BASE_CANONICA  
**Estado:** JULCON v13.1 / REGLA_BASE_CANONICA / NO_EMITIBLE POR SÃ SOLA  
**Tipo:** Regla operativa obligatoria de prueba de pertenencia documental.

---

## 1. Causa raÃ­z

Durante un inventario se clasificÃ³ un archivo, `otro proyecto-MMF-IE-PL-0101 Diagrama Unifilar`, como **gap del proyecto** confiando en el tÃ­tulo/prefijo, sin probar su cadena de carpeta hasta una raÃ­z del proyecto.

El archivo era de otro origen. El prefijo `otro proyecto` ya habÃ­a contaminado antes mediante una memoria otro proyecto.

Este antecedente queda como caso de control: **falso gap es tan grave como falso hallazgo**.

---

## 2. Criterio rector

NingÃºn archivo se clasifica, cita, integra ni reporta, ni siquiera como gap del proyecto, hasta **PROBAR** que su carpeta padre asciende por cadena verificada hasta una raÃ­z autorizada del proyecto.

Las raÃ­ces autorizadas son las que se declaren para el proyecto activo en su bootstrap de gobierno. No se usa ninguna raÃ­z que no estÃ© declarada y verificada para el proyecto en curso.

La pertenencia no se infiere por tÃ­tulo, prefijo, nombre de subestaciÃ³n, disciplina aparente, similitud documental ni por sonar relacionado al proyecto.

---

## 3. Regla de prueba

1. La pertenencia se **PRUEBA** por cadena de `parentId` hasta una raÃ­z autorizada del proyecto.
2. La pertenencia nunca se infiere del tÃ­tulo, prefijo, nombre de SE o apariencia documental.
3. Toda bÃºsqueda global de repositorio se considera **CONTAMINADA POR DEFECTO**, porque mezcla proyectos, clientes, bibliotecas de norma y documentos de contexto.
4. Cada resultado de bÃºsqueda global nace como **FUENTE_NO_VERIFICADA** hasta probar su cadena de carpeta.
5. Sin cadena probada, el archivo no se usa para nada:
   - No se usa como fuente.
   - No se usa como faltante.
   - No se usa como referencia.
   - No se usa como evidencia.
   - No se reporta como gap.
6. Si la cadena de carpeta no puede probarse, por limitaciÃ³n de API o falta de confirmaciÃ³n de origen, el archivo permanece **FUENTE_NO_VERIFICADA**.
7. Un archivo debe excluirse si su cadena asciende a otro proyecto o cliente, por ejemplo otro proyecto, otro proyecto / fuente no perteneciente, otro proyecto, bibliotecas ajenas o normas de otro contexto no aplicable.

---

## 4. Prohibiciones

- Prohibido clasificar un archivo como del proyecto por su tÃ­tulo o prefijo.
- Prohibido clasificar un archivo como faltante del proyecto sin cadena de carpeta probada.
- Prohibido reportar un gap basado en un archivo cuya cadena de carpeta no se probÃ³.
- Prohibido tratar la bÃºsqueda global como inventario.
- El inventario se hace navegando la jerarquÃ­a desde las raÃ­ces autorizadas del proyecto hacia abajo.

---

## 5. MÃ©todo correcto de inventario

El inventario se ejecuta navegando desde las raÃ­ces autorizadas del proyecto hacia abajo:

1. Confirmar raÃ­z autorizada.
2. Enumerar carpetas hijas.
3. Enumerar subcarpetas.
4. Enumerar archivos.
5. Registrar cadena de carpeta / `parentId`.
6. Solo despuÃ©s clasificar frente, disciplina, rol y estado de lectura.

La bÃºsqueda por tÃ­tulo puede usarse solo como herramienta auxiliar de localizaciÃ³n, nunca como prueba de pertenencia ni como inventario.

---

## 6. RelaciÃ³n con reglas de cobertura

- **R2** = pertenencia: pregunta si la fuente pertenece al proyecto.
- **R5** = mÃ©todo de prueba: prueba por cadena de carpeta, no por tÃ­tulo.
- **R4** = universo al arranque: se enumera desde las raÃ­ces, no por bÃºsqueda.
- **R3** = barrido antes de cierre: verifica que todo el universo fue cubierto antes de declarar cierre.

SÃ­ntesis operativa:

- **R5 es el mÃ©todo de prueba que hace ejecutables a R2 y R4.**

---

## 7. Estado por defecto

Todo archivo sin cadena de carpeta probada queda por defecto:

**FUENTE_NO_VERIFICADA / NO_EMITIBLE.**

