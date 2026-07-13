# REGLA_R3 â€” BARRIDO SISTEMÃTICO Y COMPLETO DE FUENTES

**Sistema:** JULCON v13.1  
**Ãmbito:** REGLA_BASE_CANONICA  
**Estado:** JULCON v13.1 / REGLA_BASE_CANONICA / NO_EMITIBLE POR SÃ SOLA  
**Tipo:** Regla operativa obligatoria de cobertura documental, cierre de frente, RFI, despiece y catÃ¡logo.

---

## 1. Criterio rector

Antes de declarar cerrado un frente, un RFI, un despiece o el catÃ¡logo, y antes de afirmar cobertura documental, se debe ejecutar un **BARRIDO SISTEMÃTICO Y COMPLETO** del repositorio del proyecto.

Este barrido debe ser de repositorio y paquete documental, no lectura a demanda.

---

## 2. Alcance del barrido

El barrido debe incluir:

1. Enumerar recursivamente **TODAS** las carpetas del proyecto:
   - Root del proyecto activo.
   - Carpetas de licitaciÃ³n verificadas por **REGLA_R2**.
   - Cada subcarpeta y archivo contenido.

2. Clasificar **CADA archivo** con estado explÃ­cito:
   - **LEÃDO_PRIMARIA**.
   - **LEÃDO_PARCIAL**.
   - **SOLO_CAJETÃN**.
   - **NO_LEÃDO**.

3. Clasificar **CADA archivo** por rol:
   - **RECTOR**.
   - **AUXILIAR**.
   - **BENCHMARK**.
   - **NO_APLICA**.

4. NingÃºn frente, RFI, despiece o catÃ¡logo se declara cerrado si un documento que lo gobierna estÃ¡ **NO_LEÃDO**.

5. Si el documento rector no se ha abierto, el Ã­tem queda **ABIERTO**. No se infiere como cerrado.

---

## 3. Prohibiciones

- Prohibido afirmar **analicÃ© todo** o **cobertura completa** sin barrido ejecutado y registrado.
- Prohibido cerrar un RFI por ausencia de evidencia cuando existan documentos **NO_LEÃDOS** que puedan contenerla.
- Prohibida la lectura a demanda como sustituto del barrido cuando se va a declarar cierre o cobertura.

---

## 4. Procedimiento de cierre

Debe mantenerse un **ÃNDICE DE COBERTURA vivo** con, como mÃ­nimo:

- Archivo.
- Carpeta/ruta.
- Estado de lectura.
- Rol documental.
- Frente/disciplina al que aplica.
- Porcentaje real de documentos leÃ­dos contra documentos totales.

Antes de cualquier declaraciÃ³n de cierre global, los documentos **RECTORES** del alcance deberÃ¡n estar en estado **LEÃDO_PRIMARIA**.

---

## 5. Antecedente operativo

**RFI-FOSA-FC:** casi se cierra como sin sustento cuando el dato de resistencia de concreto residÃ­a en el civil de Linde no barrido. La lectura dirigida ocultÃ³ el hueco.

Este antecedente queda como caso de control para impedir cierres sin barrido.

---

## 6. Estado por defecto

Toda cobertura, cierre, RFI, despiece o catÃ¡logo sin barrido registrado queda por defecto:

**NO_VERIFICADA / NO_EMITIBLE.**

