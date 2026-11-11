# GATE-EPC-QA-001 — Calidad técnica por concepto y emisión controlada de entregables EPC

**Estado:** PROPUESTA_P0 / NO_CANONICA / NO_FUSIONAR_SIN_REVISION_INDEPENDIENTE / NO_EMITIBLE.
**Origen:** NC-otro centro de carga-2026-11-04; catálogo preliminar 115/13.8 kV de otro centro de carga presentado como terminado con descripciones insuficientes para cotización.
**Aplicabilidad propuesta:** catálogos EPC, despieces, RFQ, memorias, listas de equipos, RFI técnicos y entregables multidisciplinarios de JULCON.
**Jerarquía:** complemento operativo y verificable de R0, R7, R14, R19, R20, R21, R23, R24 y R25. No sustituye ni modifica reglas protegidas existentes.

## 1. Falla que debe bloquearse

Un documento puede tener muchas partidas, formato correcto, nombres de hojas, fórmulas y un enlace descargable y seguir siendo técnicamente incompleto. El número de conceptos, de páginas, de hojas o de palabras **no** acredita calidad, cotizabilidad ni cobertura.

**Invariante:** `ENTREGABLE_GENERADO != ENTREGABLE_TECNICAMENTE_ENRIQUECIDO != ENTREGABLE_AUDITADO != ENTREGABLE_APROBADO != ENTREGABLE_EMITIBLE`.

El constructor no puede declarar APTO_PARA_RFQ por obtener un Excel que abre y parece profesional. La imposibilidad de activar un motor o un segundo agente se registra explícitamente, sin simular su ejecución.

## 2. Preflight previo a generar

1. Identificar objetivo, destinatario, nivel de madurez: BORRADOR_INTERNO / PRELIMINAR_INDICATIVO / CANDIDATO_RFQ / RFQ_APROBADO.
2. Leer reglas y puntero canónico **actuales** desde GitHub; registrar referencia, commit y diferencias con la versión reclamada. Si `CURRENT.md` apunta a v13.1, no afirmar que v13.2 es canónica.
3. Inventariar fuentes y delimitar qué se leyó, cotejó, interpretó o no se pudo revisar. HULKON indexado ≠ fuente primaria abierta ni norma verificada.
4. Construir mapa de disciplinas, interfaces, sistemas, entregables, exclusiones y RFIs.
5. Designar por separado constructor y revisor senior; si no hay ejecución efectiva, estado `R25_NO_EJECUTADA`.

## 3. Contrato de calidad para CADA concepto de catálogo EPC

Validación exhaustiva al **100 % de los IDs**, no sólo una muestra. Cada ID debe contener o vincular expresamente:

| Campo | Condición semántica obligatoria |
|---|---|
| ID / sistema / especialidad | Único, estable; paquete e integrador responsable identificados |
| Concepto | Objeto técnico inequívoco que permite diferenciarlo de otros |
| Descripción de alcance | Función, suministro/trabajo, componentes, accesorios, montaje/instalación y fronteras; especificación física y eléctrica pertinente |
| Parámetros | Nivel de tensión, corriente, relación, exactitud, burden, aislamiento, ambiente, protocolo, material, dimensión, etc., **solo según aplique y fuente** |
| Unidad/cantidad | Unidad cotizable y cantidad con fuente, cálculo o estado TBD, nunca cifra decorativa |
| Normativa | Clave, edición, cláusula **verificada bajo R7** cuando se cite como exigencia; si no, referencia candidata marcada `NORMA_NO_VERIFICADA` sin aparentar mandato |
| Interfaces | Conexión con otros sistemas, obra preexistente, titular único de suministro/trabajo, exclusiones y dependencia |
| Pruebas/aceptación | Evidencia de aceptación observable: FAT, SAT, pruebas de campo, documentos, criterio de recepción aplicable |
| Dependencia/RFI | RFI preciso y efecto en alcance, costo, plazo o emitibilidad, si corresponde |
| Madurez | CONFIRMADO / INTERPRETACIÓN / SUPUESTO / TBD, fuente e impacto de la reserva |
| Comprabilidad | El licitante puede identificar qué suministrar, instalar, probar y documentar, y qué NO está incluido |

**Excepciones legítimas:** para una tarea sencilla, campo no aplicable `N/A_CON_JUSTIFICACION`; para un dato no disponible `TBD_CON_RFI_IMPACTO`. Nunca completar un campo con texto genérico para aparentar cobertura.

**Prohibiciones de texto vacío de ingeniería:** `conforme a normas aplicables`, `incluye todo lo necesario`, `equipo completo`, `según especificación`, `a satisfacción del cliente` si no se desarrolla el alcance verificable. Su presencia no falla automáticamente cuando hay contexto, pero dispara revisión semántica.

## 4. GATE por capas y barreras de emisión

**G0 Inventario y contexto:** fuente, universo, documento maestro, proyecto, alcance, versión, fecha y destinación; FAIL si se parte de resumen como única fuente.

**G1 Cobertura:** R0/R19/R24, cruce de especialidades, intangibles, pruebas y gestiones; FAIL si faltan categorías obligadas o no se explica exclusión.

**G2 Calidad por partida:** chequeo de 100% ID; FAIL si existen descripciones no cotizables, normativas falsas, aceptaciones circulares, interfaces ambiguas o duplicados. Un concepto `TBD_CON_RFI_IMPACTO` puede permanecer en BORRADOR_INDICATIVO, pero jamás disfrazarse de RFQ cerrado.

**G3 Integridad comercial:** R23, unidades medibles, conteos, cantidades, fórmulas y ausencia de doble conteo. FAIL para RFQ/CAPEX ante inconsistencias materiales.

**G4 Evidencia normativa:** R7, emisor, documento fuente, edición, cláusula, aplicabilidad y prueba de lectura de fuente primaria; obligación no verificada impide presentarla como exigencia.

**G5 Independencia:** R25, revisión real separada de construcción, hallazgos y correcciones; no equivale a autoaprobación.

**G6 Entrega funcional:** comprobar existencia física del archivo, apertura válida, integridad ZIP/XLSX, 100% hojas esperadas, fórmulas, formatos, enlaces reales, inventario y SHA-256. Prohibido publicar un enlace sin comprobar el archivo en la sesión.

**G7 Ratificación:** responsabilidad expresa del Director EPC para emisión externa; la aprobación IA no sustituye al humano.

### Estados autorizados

- `BORRADOR_INTERNO_CONTROLADO`: puede revisarse internamente con reservas explícitas, sin anunciar aptitud de RFQ.
- `PRELIMINAR_INDICATIVO_CON_RFI`: descripciones sustantivas por partida, cantidades/riesgos etiquetados y pendientes visibles; no emitible comercialmente.
- `CORRECCION_REQUERIDA_NO_EMITIBLE`: descripción genérica, fuente inventada, doble conteo, prueba insuficiente o R25 no ejecutada.
- `CANDIDATO_RFQ_R25_APROBADO`: gates G0-G6 satisfechos; todavía sujeto a ratificación humana.
- `RFQ_RATIFICADO_POR_DIRECTOR_EPC`: autorización expresa de emisión; no implica VoBo CFE/CENACE.

**Ningún estado se otorga por defecto.** Si no hay evidencia de una compuerta, su valor es `NO_EJECUTADA` y su resultado se considera FAIL para ratificación.

## 5. Responsabilidad de agentes y motores

- Gobernador: comprueba arranque, versión, fuentes y gatillos; no suplanta al constructor.
- Constructor EPC: amplía cada concepto con especificaciones y traza la evidencia.
- Especialista normativo: confronta cada fundamento con la fuente primaria y vigencia; no infiere por analogía.
- Auditor de cantidades: revisa unidades, cálculos, dobles conteos y fronteras.
- Revisor independiente: ataca supuestos y evalúa partes críticas de todo el universo, con cobertura 100% de filas para criterios mínimos.
- Director EPC: ratifica decisiones de diseño, reservas y emisión externa.

**Motores:** gobierno, source traceability, grafo EPC, compliance assist, RFQ/CAPEX relevance, readiness/gate. Para cada uno registrar `ACTIVO_CON_EVIDENCIA`, `NO_DISPONIBLE`, `NO_EJECUTADO` o `EJECUCION_FALLIDA`; nunca afirmar activación sin ejecución comprobada.

## 6. Evidencia mínima para un catálogo

Acompañar el artefacto con matriz `ID → campos críticos (F/K/M/I/L o equivalentes) → evidencia → RFI → estado → revisor`; informe con número total, completos, con reserva, bloqueados, duplicados; diff de cambios en celdas; inventario/hash de entradas y salidas; R14 y R25 ejecutados o marcados como pendientes.

## 7. Aceptación del cambio en JULCON

**No se considera implementada esta regla** hasta:
1. Aprobación editorial del texto por gobernanza.
2. Implementación del preflight automatizado y validaciones estructurales sobre XLSX/CSV (identidad, campos, fórmulas, unidades, cantidades, enlaces).
3. Revisión semántica senior aparte: la longitud del texto o una regex no garantizan calidad.
4. Pruebas adversariales y regresión Linux/Windows según política vigente, sin excepciones autoaprobadas.
5. Integración a manifest/arranque vigente, con trazabilidad de versión, sin modificar `main` hasta NO-GO levantado.

**Caso de prueba P0:** CSV/XLSX con 171 IDs sintácticamente válidos pero descripciones genéricas debe obtener `CORRECCION_REQUERIDA_NO_EMITIBLE`, incluso si abre correctamente y sus fórmulas calculan. El catálogo enriquecido no obtiene APTO automáticamente; exige fuentes, evidencias, R25 y ratificación.

## 8. Estado del incidente otro centro de carga

El catálogo Rev.0.1 **no debe etiquetarse como RFQ listo** ni como prueba de funcionamiento de motores. Se permite usar como índice preliminar interno; exige enriquecimiento y auditoría exhaustiva. La existencia de un permiso histórico de generación es RFI, no evidencia de generación operativa; se mantiene excluida del alcance base hasta confirmación.

---
**Revisión requerida:** mantener como propuesta en rama aislada / PR DRAFT; no sobrescribir R14, R20, R25 ni declararla canónica antes del cierre de auditoría independiente y WP10.
