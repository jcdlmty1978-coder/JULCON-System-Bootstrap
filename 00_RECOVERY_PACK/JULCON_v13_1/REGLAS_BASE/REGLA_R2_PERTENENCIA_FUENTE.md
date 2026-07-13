# REGLA_R2 â€” VERIFICACIÃ“N OBLIGATORIA DE PERTENENCIA DE FUENTE

**Sistema:** JULCON v13.1  
**Ãmbito:** REGLA_BASE_CANONICA  
**Estado:** JULCON v13.1 / REGLA_BASE_CANONICA / NO_EMITIBLE POR SÃ SOLA  
**Tipo:** Regla operativa obligatoria de pertenencia documental, lectura, integraciÃ³n, cita y dictamen.

---

## 1. Criterio rector

Antes de leer, integrar, citar, clasificar, usar para despiece, usar para RFI, usar para catÃ¡logo o usar para dictamen cualquier fuente, se debe verificar que pertenece simultÃ¡neamente a:

1. **Root del proyecto activo:** la raÃ­z autorizada declarada para el proyecto en curso en su bootstrap de gobierno.
2. **SE / frente / disciplina analizada:** por ejemplo civil, elÃ©ctrica, PCyM, control, comunicaciones, HSE, mediciÃ³n, servicios propios, SCI, HVAC, planta de emergencia, LT o normativa aplicable.

---

## 2. Tratamiento de fuentes sin pertenencia confirmada

Toda fuente sin pertenencia confirmada queda clasificada como:

**FUENTE_NO_VERIFICADA / NO_EMITIBLE.**

Una fuente en este estado:

- No se usa para cumplimiento.
- No se usa para cantidades definitivas.
- No se usa para dictamen.
- No se usa para cerrar RFI.
- No se usa para declarar faltante/gap.
- Solo puede usarse como indicio explÃ­citamente marcado y pendiente de validaciÃ³n.

---

## 3. AplicaciÃ³n prÃ¡ctica

- Un resultado de bÃºsqueda en Drive no basta para usar una fuente.
- Un PDF abierto no basta para usar una fuente.
- Una norma localizada no basta para declarar aplicabilidad.
- Un archivo cargado por el usuario no basta para asumir pertenencia al universo completo.
- Un nombre de subestaciÃ³n, prefijo o tÃ­tulo no prueba pertenencia.
- Una carpeta con nombre similar no prueba pertenencia si no se valida contra raÃ­z autorizada.

---

## 4. RelaciÃ³n con R5

R2 formula la pregunta de pertenencia:

**Â¿Esta fuente pertenece al proyecto, frente y disciplina que estoy analizando?**

R5 define el mÃ©todo de prueba:

**La pertenencia se prueba por cadena de carpeta / `parentId` hasta raÃ­z autorizada, no por tÃ­tulo ni prefijo.**

Por tanto, R2 no queda satisfecha hasta que R5 se cumpla.

---

## 5. RelaciÃ³n con reglas de cobertura

- **R0** gobierna la cobertura documental exhaustiva y hace inviolable la jerarquÃ­a de reglas.
- **R2** valida pertenencia de fuente.
- **R5** prueba pertenencia por cadena de carpeta.
- **R4** establece el universo documental completo al arranque.
- **R3** verifica el barrido completo antes de cierre.
- **R6** ejecuta el recorrido descendente desde raÃ­z hacia hojas, si aplica.

---

## 6. Estado por defecto

Todo documento, plano, CP, especificaciÃ³n, norma, tabla, captura, archivo local, bÃºsqueda Drive, resultado HULKON, ZIP, anexo o insumo de comparaciÃ³n cuya pertenencia no estÃ© confirmada queda por defecto:

**FUENTE_NO_VERIFICADA / NO_EMITIBLE.**

