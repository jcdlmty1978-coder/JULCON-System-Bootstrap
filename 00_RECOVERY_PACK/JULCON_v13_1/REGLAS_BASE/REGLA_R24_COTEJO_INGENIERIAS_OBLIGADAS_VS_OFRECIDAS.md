# REGLA R24 — COTEJO DE INGENIERÍAS OBLIGADAS VS OFRECIDAS

**Sistema:** JULCON v13.1  
**Ámbito:** REGLA_GLOBAL / REGLA_BASE_CANONICA  
**Estado:** REGLA_PROTEGIDA / ACTIVA

## 1. Criterio rector

Antes de ratificar un Libro Maestro, despiece o paquete RFQ, se debe cotejar mediante checklist el conjunto de ingenierías, memorias y estudios obligados por el documento rector contra los ofrecidos en el entregable.

Toda ausencia debe integrarse como partida o entregable nuevo marcado `POR_AUDITORIA`, o registrarse como RFI. Nunca se ratifica un entregable con una ingeniería obligada ausente.

## 2. Checklist mínimo enunciativo

Según aplique, revisar:

- ingeniería de detalle electromecánica y civil;
- topografía, geotecnia, mecánica de suelos y resistividad;
- censo de instalaciones subterráneas;
- corto circuito;
- coordinación de protecciones;
- arco eléctrico;
- coordinación de aislamiento;
- sistema de pararrayos o blindaje atmosférico, distinto de apartarrayos;
- SAS, control supervisorio, SCL, matrices y base de datos;
- comunicaciones y ciberseguridad;
- sistema contra incendios;
- alumbrado y luxometría;
- drenaje y obras complementarias;
- lista de materiales multidisciplina y número de proveedores exigido;
- As-Built y formatos requeridos;
- Código de Red;
- validaciones, pruebas, telemetría y gestiones de organismos competentes.

La lista es enunciativa, no limitativa.

## 3. Método obligatorio

Por cada obligación registrar:

- obligación exacta;
- documento rector y ubicación;
- disciplina y frente;
- entregable ofrecido que la cubre;
- cobertura total, parcial o nula;
- acción requerida;
- estado de emitibilidad.

## 4. Prohibiciones

- Dar por cubierta una ingeniería por similitud de título.
- Suponer que una memoria genérica cubre todos los estudios especializados.
- Confundir blindaje atmosférico con apartarrayos.
- Omitir censo de subterráneas en trazados enterrados.
- Ratificar con obligaciones sin contraparte ofrecida.

## 5. Gate de cierre

Estados permitidos por obligación:

- `CUBIERTA_TOTALMENTE`
- `CUBIERTA_PARCIAL_CON_ACCION`
- `INTEGRADA_POR_AUDITORIA`
- `RFI_ABIERTA_BLOQUEANTE`
- `NO_APLICA_CON_FUNDAMENTO`

Una obligación sin registro mantiene:

`INGENIERIA_OBLIGADA_NO_COTEJADA / RATIFICACION_BLOQUEADA`

## 6. Estado operativo

`R24_ACTIVA / CHECKLIST_OBLIGADO_VS_OFRECIDO / AUSENCIA_BLOQUEANTE / INTEGRACION_POR_AUDITORIA_O_RFI`