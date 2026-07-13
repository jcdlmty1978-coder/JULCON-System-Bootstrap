# REGLA_R0 â€” COBERTURA DOCUMENTAL EXHAUSTIVA [INVIOLABLE]

**Sistema:** JULCON v13.1  
**Ãmbito:** REGLA_BASE_CANONICA  
**Estado:** JULCON v13.1 / REGLA_BASE_CANONICA / INVIOLABLE / NO_EMITIBLE POR SÃ SOLA  
**Tipo:** Regla superior de cobertura documental exhaustiva, pertenencia, inventario, ausencia, faltante, cierre y validez de entregables.  
**Severidad:** MÃXIMA / INVIOLABLE / PRECEDENCIA ABSOLUTA.

---

## 1. BREAKING / Precedencia

**R0 tiene precedencia sobre velocidad, conveniencia, presiÃ³n de entrega, lectura dirigida y lÃ­mites tÃ©cnicos.**

R0 absorbe y eleva a severidad mÃ¡xima inviolable las reglas de cobertura:

- **R2** â€” pertenencia.
- **R5** â€” prueba por cadena de carpeta.
- **R4** â€” universo documental al arranque.
- **R3** â€” barrido completo antes de cierre.
- **R6** â€” recorrido descendente.

Ninguna regla subordinada puede interpretarse de forma que reduzca el mandato de cobertura exhaustiva de R0.

---

## 2. Mandato rector inviolable

Ninguna afirmaciÃ³n de cobertura, ausencia, cierre, faltante, gap, RFI cerrado, frente cerrado, despiece completo, catÃ¡logo completo o dictamen equivalente es vÃ¡lida sin recorrer fÃ­sicamente cada carpeta y subcarpeta del universo documental del proyecto, hasta las hojas, por navegaciÃ³n jerÃ¡rquica.

La navegaciÃ³n debe hacerse desde las raÃ­ces autorizadas del proyecto hacia abajo, no por bÃºsqueda de tÃ­tulos.

---

## 3. Principios inviolables

1. **BÃºsqueda sin resultado no prueba ausencia.**
2. La pertenencia de una fuente se prueba por cadena de carpeta / `parentId` hasta raÃ­z autorizada.
3. Ninguna limitaciÃ³n tÃ©cnica autoriza omitir un nodo del universo documental.
4. NingÃºn archivo se usa como fuente, faltante, referencia, gap o evidencia sin pertenencia probada.
5. NingÃºn cierre o declaraciÃ³n de cobertura es vÃ¡lido sin inventario de arranque y barrido registrado.
6. Todo entregable en violaciÃ³n de R0 queda **NULO**.

---

## 4. Ausencia no probada

Una bÃºsqueda sin resultado **NO prueba ausencia**.

La ausencia de una fuente, plano, norma, frente, carpeta, anexo, especificaciÃ³n, memoria, lista, plano civil, plano electromecÃ¡nico, PCyM, SCI, servicios propios, HVAC, planta de emergencia, LT, mediciÃ³n o documento equivalente solo puede afirmarse despuÃ©s de recorrer fÃ­sicamente todo el universo documental aplicable.

---

## 5. Pertenencia probada

Toda fuente usada, citada, clasificada, integrada, descartada o reportada debe tener pertenencia probada por cadena de carpeta hasta una raÃ­z autorizada del proyecto.

La pertenencia se prueba por cadena de `parentId`, no por:

- TÃ­tulo.
- Prefijo.
- Nombre de subestaciÃ³n.
- Nombre de disciplina.
- Similitud documental.
- Resultado de bÃºsqueda.
- Apariencia de pertenecer al proyecto.

Todo resultado de bÃºsqueda global nace como **FUENTE_NO_VERIFICADA** hasta probar su cadena de carpeta.

---

## 6. LÃ­mites tÃ©cnicos

Ninguna limitaciÃ³n tÃ©cnica autoriza omitir un nodo documental.

Si una API, conector, visor, extractor, buscador, OCR, Ã­ndice, ZIP, Drive, GitHub, herramienta o plataforma impide ascender, listar, abrir, descargar, ver o recorrer un nodo, el nodo queda bloqueante hasta resolverse o declararse explÃ­citamente como no verificable.

Un nodo no recorrido no puede tratarse como ausente, irrelevante, cerrado ni cubierto.

---

## 7. Casos que originan R0

R0 nace de fallas operativas documentales donde la lectura dirigida generÃ³ falsos huecos, falsos faltantes o cierres prematuros:

- **CFE/LTS-DRE/170298** fue declarada faltante estando en carpeta LTS no abierta.
- Se produjo un falso hueco de frentes que correspondÃ­a a otro proyecto.
- **RFI-FOSA-FC** casi se cerrÃ³ sin leer **DCDLTS01**.

Estos casos quedan como antecedentes de control para impedir cobertura declarada sin recorrido exhaustivo.

---

## 8. JerarquÃ­a de cobertura

R0 gobierna la jerarquÃ­a documental de cobertura:

1. **R0 [INVIOLABLE]** â€” Cobertura documental exhaustiva.
2. **R2** â€” Pertenencia: pregunta si la fuente pertenece al proyecto.
3. **R5** â€” Cadena: prueba la pertenencia por cadena de carpeta / `parentId`.
4. **R4** â€” Universo: establece el universo documental completo al arranque.
5. **R3** â€” Barrido: verifica todo el universo antes de declarar cierre.
6. **R6** â€” Recorrido descendente: ejecuciÃ³n jerÃ¡rquica desde raÃ­z hacia hojas.

R0 gobierna R2, R5, R4, R3 y R6.

---

## 9. Prohibiciones

- Prohibido declarar cobertura completa sin recorrer cada carpeta y subcarpeta hasta las hojas.
- Prohibido declarar ausencia por bÃºsqueda sin resultado.
- Prohibido declarar cierre por lectura a demanda.
- Prohibido usar una fuente sin pertenencia probada por cadena de carpeta.
- Prohibido omitir carpetas o nodos por lÃ­mites tÃ©cnicos, prisa, conveniencia o aparente baja relevancia.
- Prohibido emitir entregables que violen R0.

---

## 10. Procedimiento mÃ­nimo obligatorio bajo R0

Antes de afirmar cobertura, ausencia, faltante o cierre se debe demostrar:

1. RaÃ­ces autorizadas identificadas.
2. Cadena de carpeta probada para cada fuente usada.
3. Ãrbol completo de carpetas recorrido desde raÃ­ces hacia hojas.
4. Archivos enumerados por carpeta.
5. Estado de lectura por archivo.
6. Rol documental por archivo.
7. Documentos rectores abiertos y leÃ­dos en fuente primaria.
8. Nodos bloqueados o no verificables declarados como bloqueantes.
9. Ãndice de cobertura vivo actualizado.
10. DeclaraciÃ³n explÃ­cita de que no hay documentos rectores **NO_LEÃDOS** dentro del alcance que se pretende cerrar.

---

## 11. Nulidad de entregables

Todo entregable, anÃ¡lisis, despiece, catÃ¡logo, RFI, comparativo, dictamen, reporte de gaps o afirmaciÃ³n de cobertura emitido en violaciÃ³n de R0 queda:

**NULO / NO_VERIFICADO / NO_EMITIBLE.**

La nulidad aplica aunque el resultado sea Ãºtil, parcial o aparentemente correcto.

---

## 12. Estado por defecto

Toda afirmaciÃ³n de cobertura, ausencia, cierre, faltante, gap, RFI, despiece, catÃ¡logo o entregable que no demuestre cumplimiento de R0 queda por defecto:

**NO_VERIFICADA / NO_EMITIBLE / NULA PARA CIERRE.**

