# REGLA_R7 — VERIFICACIÓN OBLIGATORIA DE NORMA / ESPECIFICACIÓN EN FUENTE PRIMARIA

**Sistema:** JULCON v13.1  
**Ámbito:** REGLA_BASE_CANONICA  
**Estado:** REGLA_BASE_CANONICA / COMPUERTA_OBLIGATORIA / NO_EMITIBLE POR SÍ SOLA

## 1. Criterio rector

Ninguna especificación, norma, código, edición o clave normativa puede afirmarse, citarse, escribirse en un entregable, utilizarse para evaluar cumplimiento o emplearse en un dictamen hasta verificarla contra su **FUENTE PRIMARIA**.

**Fuente primaria** es el documento oficial que define la especificación, norma, código o criterio; no un documento secundario que solamente lo menciona.

## 2. Qué NO constituye verificación

No verifican una norma o especificación:

1. Una cita contenida en otro documento.
2. Un texto obtenido únicamente por OCR, extracción automática o lectura textual de PDF.
3. La memoria del agente, un chat previo o una respuesta anterior.
4. El parecido temático entre el equipo y una norma.
5. Una búsqueda web, resumen, índice, catálogo comercial o documento no oficial que no sea el texto fuente.

## 3. Condiciones acumulativas de verificación

Una norma o especificación solo queda **VERIFICADA** cuando se cumplen y registran todos los puntos aplicables:

1. **Existencia:** el documento fuente fue localizado.
2. **Aplicabilidad:** gobierna exactamente el equipo, elemento, función, nivel de tensión, servicio o hito evaluado.
3. **Exactitud:** el código, título, edición y dato crítico fueron cotejados contra la página-imagen o vista renderizada del documento fuente, no únicamente contra OCR.
4. **Origen y autenticidad:**
   - Si el documento forma parte del universo contractual o documental del proyecto, debe tener pertenencia probada conforme a R2 y R5 mediante cadena de carpeta/`parentId` hasta una raíz autorizada.
   - Si la fuente primaria es externa —por ejemplo IEC, IEEE, NOM, organismo regulador, fabricante u organismo emisor— debe verificarse su autenticidad, edición y procedencia desde la fuente oficial, autorizada o controlada.
5. **Vigencia y edición:** la edición utilizada debe ser la contractual o aplicable al proyecto. La edición más reciente no sustituye automáticamente la edición contractual.

Si falta cualquiera de los puntos aplicables, la referencia no está verificada.

## 4. Prioridad de fuentes

Cuando varias fuentes mencionen la misma norma o criterio, se aplica esta prioridad:

1. Documento fuente oficial de la norma o especificación.
2. Especificación contractual o base técnica rectora del proyecto.
3. Manual OEM aplicable al equipo exacto.
4. Documento secundario que únicamente cita o resume la norma.

Una fuente de menor nivel no puede “corregir” por sí sola a una fuente de mayor nivel.

## 5. Estado por defecto

Mientras no se cumplan y registren las condiciones de la sección 3, el estado obligatorio es:

`NORMA_NO_VERIFICADA / PENDIENTE_DE_VERIFICAR / NO_EMITIBLE`

La referencia puede conservarse únicamente como indicio explícitamente marcado. Nunca debe presentarse como confirmada ni como corrección definitiva de otra norma.

## 6. Prohibiciones

Queda prohibido:

1. Sustituir o “corregir” una norma por otra tomada de una cita interna, OCR, memoria, chat o parecido temático.
2. Escribir una clave en un campo de “verificado” sin cumplir la sección 3.
3. Declarar cumplimiento o incumplimiento sin verificar tanto la fuente primaria como su aplicabilidad al equipo evaluado.
4. Presentar una lectura OCR como especificación verificada.
5. Usar una edición distinta de la contractual sin registrar y justificar expresamente la desviación.
6. Tratar una fuente web no oficial como sustituto del documento primario.

## 7. Registro de evidencia

Cada norma o especificación citada debe registrar, como mínimo:

- código, título y edición;
- documento fuente;
- emisor u origen oficial;
- ubicación o URL controlada;
- `parentId`/cadena de carpeta cuando pertenezca al universo del proyecto;
- equipo, función o hito al que aplica;
- método de lectura del código: imagen/render y, si se usó, OCR auxiliar;
- página, sección o cláusula verificada;
- fecha de verificación;
- responsable o agente que realizó el cotejo.

Sin evidencia registrada, se mantiene `NORMA_NO_VERIFICADA`.

## 8. Trazabilidad de origen

Esta regla nace de un incidente de proyecto en el que una clave normativa tomada de una cita OCR dentro de un documento secundario fue presentada como verificada e incluso como “corrección”.

Acción correctiva: releer la clave desde la página-imagen del documento secundario y confirmarla contra la especificación primaria aplicable, localizada en una fuente autorizada y con procedencia probada. Hasta completar ese cotejo, el estado es `PENDIENTE_DE_VERIFICAR`.

## 9. Relación con la jerarquía

R7 está subordinada a R0 y complementa R2 y R5.

- R0 gobierna la cobertura documental.
- R2 y R5 gobiernan la pertenencia de documentos del proyecto.
- R7 añade identidad, aplicabilidad, autenticidad, edición y exactitud normativa.

R7 funciona como compuerta obligatoria antes de citar, escribir, comparar, corregir o dictaminar con base en cualquier norma o especificación.

## 10. Estado de cierre

Toda especificación, norma, código, clave, edición o afirmación de cumplimiento sin verificación primaria probada y registrada queda por defecto en:

`NORMA_NO_VERIFICADA / PENDIENTE_DE_VERIFICAR / NO_EMITIBLE`
