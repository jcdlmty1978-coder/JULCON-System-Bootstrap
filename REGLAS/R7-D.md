<!-- TRAZABILIDAD DE ORIGEN; fuente: expediente interno de origen/00_GOBIERNO/REGLA_R7_RFI_DOCUMENTO_FALTANTE_VS_ENTREGABLE_CONTRATISTA.md @blob:94efffc662431d3b60cb0cc97f5ddcf749a1f52f; R7-N/R7-D son identidades distintas. -->

# REGLA R7-D — RFI DOCUMENTO FALTANTE VS ENTREGABLE DEL CONTRATISTA

**Ámbito:** Todos los proyectos donde se determine la responsabilidad contractual de documentos y RFI; origen trazado en fuente privada.
**Sistema:** JULCON / Gobierno técnico interno  
**Estado:** ACTIVA / PROTEGIDA / INVIOLABLE  
**Fecha de alta:** 2026-07-07  
**Relación:** Complementa R2, R3, R4, R5, R6 y R6.1.  
**Uso cliente:** JULCON invisible; no mencionar esta regla en entregables externos.

---

## 1. Nombre corto

`R7-D_NO_RFI_DOCUMENTO_FALTANTE_SIN_REVISAR_ENTREGABLE_CONTRATISTA`

---

## 2. Motivo

Esta regla corrige una falla de clasificación detectada en la revisión de RFIs: se marcó como RFI vivo una lista/documento que en realidad correspondía a un **entregable de ingeniería del Contratista**, no a un faltante documental del paquete base.

A partir de esta regla, queda prohibido declarar RFI por documento faltante sin revisar primero si ese documento:

- es parte de la ingeniería a desarrollar por el Contratista;
- se entrega después de aceptación de ingeniería previa;
- forma parte de valores de obra / ingeniería reconocible;
- corresponde a documento as-built, de fabricación, pruebas, puesta en servicio o libro final;
- depende de ingeniería de detalle posterior.

---

## 3. Principios inviolables

> **DOCUMENTO NO LOCALIZADO ≠ RFI AUTOMÁTICO**  
> **LISTA NO EXISTENTE EN BASE ≠ FALTANTE DEL CLIENTE**  
> **LISTA DE CABLES ≠ INSUMO BASE OBLIGATORIO SI EL RECTOR LA DEFINE COMO ENTREGABLE DEL CONTRATISTA**  
> **RFI DOCUMENTAL ≠ SUSTITUTO DE MATRIZ DE ENTREGABLES**  
> **ANTES DE RFI, REVISAR QUIÉN DEBE ELABORAR EL DOCUMENTO Y CUÁNDO**

---

## 4. Regla central

Antes de clasificar cualquier partida, lista, plano, cálculo, tabla, memoria, cédula, matriz, reporte o documento como:

- `RFI_DOCUMENTAL`,
- `FALTANTE`,
- `NO_LOCALIZADO`,
- `NO_CERRABLE`,
- `PENDIENTE_POR_DOCUMENTO`,
- `NO_EMITIBLE_POR_LISTA`,

se debe revisar de forma obligatoria la **matriz contractual/técnica de entregables de ingeniería**.

Si el documento está definido como entregable del Contratista, el estado correcto será:

`CERRADO_COMO_ENTREGABLE_CONTRATISTA / NO_RFI / CONTROLAR_COMO_ALCANCE`

---

## 5. Revisión mínima obligatoria antes de declarar RFI documental

Para cualquier supuesto documento faltante se debe revisar, como mínimo:

1. Características Particulares del frente o disciplina.
2. Características Generales aplicables.
3. Lineamientos de determinación de valores de obra.
4. Características Particulares de Ingeniería Electromecánica y Civil.
5. Pliego de Requisitos / Volumen I / Volumen II aplicable.
6. Tabla de actividades de ingeniería.
7. Tabla de entregables por etapa: entrega, aceptación, fabricación, obra, pruebas, puesta en servicio, libro final.
8. Dependencia documental: si el documento se genera después de aceptar otro paquete de ingeniería.
9. Responsabilidad de elaboración: Contratista, CFE, fabricante, cliente, tercero o integrador.
10. Momento de entrega: licitación, ingeniería de detalle, fabricación, obra, FAT, SAT, PES, as-built o libro final.

---

## 6. Clasificación obligatoria

Todo documento no localizado debe clasificarse en una de estas categorías antes de abrir RFI:

| Estado | Uso |
|---|---|
| `INSUMO_BASE_CLIENTE` | Debe existir en el paquete base. Si no está, puede ser RFI. |
| `ENTREGABLE_CONTRATISTA` | Lo elabora el Contratista; no es RFI de faltante base. |
| `ENTREGABLE_FABRICANTE` | Lo entrega el OEM/fabricante; controlar como submittal. |
| `ENTREGABLE_POSTERIOR` | Se genera después de aceptación, fabricación, pruebas o campo. |
| `DOCUMENTO_AS_BUILT` | Se entrega al cierre/libro final; no bloquea despiece base salvo que sea requerido para alcance. |
| `DOCUMENTO_DE_PRUEBAS` | Se genera en FAT/SAT/PES; controlar en pruebas. |
| `DOCUMENTO_NO_APLICA` | No aplica al frente/equipo por alcance. |
| `RFI_DOCUMENTAL_POST_REVISION` | Sólo después de revisar matriz de entregables. |

---

## 7. Caso explícito: listas de cables

Para listas de cables de protección, control, medición, fuerza, servicios propios, fibra óptica o comunicaciones:

1. No deben marcarse automáticamente como RFI si no aparecen como lista final en el paquete base.
2. Debe revisarse si las listas son entregables de ingeniería del Contratista.
3. Debe revisarse si se entregan después de aceptación de ingeniería de tableros, PCyM, control supervisorio, comunicaciones o equipo primario.
4. Si el rector indica que son entregables del Contratista, se reclasifican como:

`ENTREGABLE_CONTRATISTA / CONTROLAR_EN_ALCANCE / NO_RFI`

5. El despiece debe incluir alcance de ingeniería, suministro, tendido, conexión, pruebas e integración, pero no inventar cédulas finales de cable.

---

## 8. Prohibiciones R7-D

Queda prohibido:

1. Abrir RFI por lista de cables sin revisar lineamientos de entregables de ingeniería.
2. Abrir RFI por memoria, lista, cálculo o plano no localizado sin determinar si lo elabora el Contratista.
3. Tratar como faltante del cliente un documento definido como entregable del Contratista.
4. Bloquear despiece base por un documento que contractualmente se desarrolla en ingeniería de detalle.
5. Inventar cantidades finales cuando el rector establece que se determinarán en ingeniería del Contratista.
6. Confundir `no localizado` con `no existe`.
7. Confundir `no existe en base` con `lo debe proporcionar el cliente`.
8. Confundir `entregable posterior` con `RFI técnico`.
9. Mezclar documentos de otro proyecto o fuentes no R5 para cerrar o abrir RFIs.

---

## 9. Efecto operativo en RFIs

Todo RFI documental deberá traer dos campos obligatorios:

| Campo | Pregunta |
|---|---|
| `RESPONSABLE_DOCUMENTO` | ¿Quién debe elaborar/proporcionar el documento? |
| `MOMENTO_ENTREGA` | ¿En qué etapa debe existir el documento? |

Si esos campos no están resueltos, el RFI queda inválido como RFI final y debe marcarse:

`RFI_PREMATURO / PENDIENTE_REVISION_R7-D`

---

## 10. Integración con reglas anteriores

- R2: define si la fuente pertenece al proyecto.
- R3: exige barrido antes de cierre.
- R4: fija universo documental desde root autorizado.
- R5: prueba cadena de carpeta/fuente.
- R6: exige extracción fina antes de RFI o cierre.
- R6.1: pone en cuarentena silenciosa todo resultado no R5.
- **R7-D: exige revisar matriz de entregables, responsable y etapa antes de abrir RFI documental.**

---

## 11. Aplicación inmediata

R7-D aplica de forma inmediata y retroactiva a todos los RFIs documentales del proyecto, incluyendo:

- listas de cables;
- listas de materiales;
- memorias de cálculo;
- planos de detalle;
- planos de fabricación;
- planos de pruebas;
- reportes FAT/SAT/PES;
- documentos as-built;
- libro final;
- software/configuración/base de datos;
- ingeniería de protección, control, medición, fuerza, comunicaciones y control supervisorio.

---

## 12. Estado operativo

`ACTIVA / PROTEGIDA / INVIOLABLE / APLICACION_INMEDIATA / NO_RFI_DOCUMENTAL_SIN_MATRIZ_ENTREGABLES`

---

## 13. Nota de control

Esta regla nace del caso de listas de cables de PCyM/control/fuerza/comunicaciones: antes de abrir RFI por ausencia de lista final, debe revisarse si el documento rector establece que dichas listas son entregables de ingeniería del Contratista y si dependen de aceptación previa de tableros/equipo primario.

El estándar queda corregido: primero se determina responsable y etapa del documento; sólo después se decide si existe RFI real.
