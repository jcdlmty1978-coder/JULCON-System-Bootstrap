# REGLA_R4 â€” INVENTARIO DE ARRANQUE OBLIGATORIO

**Sistema:** JULCON v13.1  
**Ãmbito:** REGLA_BASE_CANONICA  
**Estado:** JULCON v13.1 / REGLA_BASE_CANONICA / NO_EMITIBLE POR SÃ SOLA  
**Tipo:** Regla operativa obligatoria de arranque, inventario documental y definiciÃ³n de universo de fuentes.

---

## 1. Criterio rector

Antes de producir **CUALQUIER** anÃ¡lisis, despiece, RFI o entregable de un proyecto, se debe establecer y registrar el **UNIVERSO DOCUMENTAL COMPLETO** del proyecto.

El universo documental se descubre por enumeraciÃ³n. No se infiere desde archivos cargados por el usuario ni desde una sola carpeta conocida.

---

## 2. Procedimiento obligatorio de arranque

Antes de trabajar sobre cualquier documento individual se debe:

1. Enumerar la estructura completa de carpetas del repositorio del proyecto:
   - Todas las raÃ­ces verificadas por **REGLA_R2**.
   - Toda su jerarquÃ­a recursiva.
   - Todas las subcarpetas y archivos detectados.

2. No asumir que los archivos cargados por el usuario, ni una sola carpeta conocida, constituyen el universo total del proyecto.

3. Registrar el inventario como lÃ­nea base, incluyendo lista de carpetas y su disciplina/frente, por ejemplo:
   - Civil.
   - ElectromecÃ¡nico.
   - PCyM.
   - SCI.
   - Servicios propios.
   - HVAC.
   - Planta de emergencia.
   - LT.
   - MediciÃ³n.
   - Especificaciones.
   - VolÃºmenes.
   - Otros frentes o disciplinas que aparezcan en el repositorio.

4. Solo despuÃ©s de tener el inventario de arranque se comienza a leer, despiezar, comparar, emitir RFIs o preparar entregables.

---

## 3. Prohibiciones

- Prohibido iniciar despiece, RFI, CAPEX, catÃ¡logo o anÃ¡lisis trabajando de adentro hacia afuera, es decir, desde los archivos a la mano, sin haber inventariado el repositorio completo.
- Prohibido tratar los archivos cargados por el usuario como alcance total del proyecto. Los archivos cargados son una muestra, no el universo documental.
- Si aparece una carpeta o frente no inventariado a mitad del trabajo, se detiene la actividad, se re-inventarÃ­a el proyecto y se reevalÃºa quÃ© entregables previos quedaron incompletos.

---

## 4. Antecedente operativo

Se despiezaron frentes durante mÃºltiples sesiones sin haber inventariado el repositorio. ExistÃ­an carpetas disciplinarias completas no abiertas, incluyendo, entre otras:

- 07 Servicios Propios.
- 08 SCI.
- 09 HVAC.
- 10 Planta Emergencia.
- IngenierÃ­a ElectromecÃ¡nica.
- IngenierÃ­a BÃ¡sica PCyM.

El despiece quedÃ³ estructuralmente incompleto sin que se detectara, por trabajar desde lo cargado en lugar de trabajar desde el universo documental completo.

---

## 5. RelaciÃ³n con otras reglas

- **R2** valida que una fuente pertenece al proyecto.
- **R4** establece el universo completo de fuentes al arranque.
- **R3** verifica que todo ese universo fue barrido antes de declarar cierre.

SÃ­ntesis operativa:

- **R4 = antes de empezar.**
- **R3 = antes de cerrar.**

---

## 6. Estado por defecto

Todo despiece, RFI, CAPEX, catÃ¡logo, comparativo, anÃ¡lisis o entregable iniciado sin inventario de arranque queda por defecto:

**INCOMPLETO / NO_EMITIBLE.**

