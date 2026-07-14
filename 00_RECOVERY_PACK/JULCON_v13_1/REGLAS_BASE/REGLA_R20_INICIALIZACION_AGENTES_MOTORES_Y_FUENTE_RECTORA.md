# REGLA R20 — INICIALIZACIÓN DE AGENTES Y MOTORES; FUENTE RECTORA POR OBJETO DE DECISIÓN

**Sistema:** JULCON v13.1  
**Ámbito:** REGLA_GLOBAL / REGLA_BASE_CANONICA  
**Estado:** ACTIVA / PROTEGIDA / INVIOLABLE / GLOBAL

## 1. Principio rector

Ningún análisis, RFI, despiece, RFQ, CAPEX, dictamen o entregable inicia sin:

1. activar los agentes y motores aplicables;
2. cargar las reglas vigentes desde GitHub;
3. consultar la biblioteca técnica autorizada del proyecto;
4. identificar el objeto exacto de la decisión; y
5. definir la fuente rectora correspondiente.

Ninguna norma, manual o especificación gobierna por sí sola un alcance completo. La fuente rectora se elige según la naturaleza de la decisión: diseño, construcción, pruebas, protecciones, SAS, medición, TIC, operación, aceptación o equipo.

## 2. Paso 0 obligatorio

Antes de leer, preguntar, calcular, redactar o emitir, el agente debe:

- identificar el tipo de tarea;
- activar gobierno, cobertura documental, pertenencia, ingeniería, normativa, RFI, RFQ/CAPEX, pruebas y gate pre-emisión, cuando correspondan;
- releer `HEAD` vigente de `JULCON-System-Bootstrap`;
- consultar primero las fuentes internas autorizadas, HULKON/JULCON o equivalentes disponibles;
- consultar web oficial cuando falte fuente, pueda haber cambio de vigencia o se requiera confirmar edición, publicación, fabricante u organismo emisor;
- construir trazabilidad documental antes de cerrar criterios o RFIs.

Si este paso no se ejecuta, el análisis queda:

`NO_INICIADO_FORMALMENTE / NO_EMITIBLE`

## 3. Fuente rectora por objeto de decisión

### 3.1 SAS / automatización

Gobiernan la ingeniería SAS del proyecto, especificación particular, arquitectura IEC 61850, archivos SCL, matrices de señales, filosofía de operación y manuales OEM aplicables.

### 3.2 Construcción, montaje y canalizaciones

Gobiernan las especificaciones constructivas, planos aprobados, normas de instalación y manuales OEM de instalación física.

### 3.3 Protecciones y control

Gobiernan la filosofía de protecciones, diagramas funcionales, especificaciones PCyM, estudios de corto circuito y coordinación, manuales OEM y normas aplicables.

### 3.4 Medición fiscal

Gobiernan el marco de medición aplicable, especificaciones de medidores y transformadores de instrumento, ingeniería aprobada y criterios del agente competente.

### 3.5 TIC / telemetría

Gobiernan el estudio de instalaciones, manual TIC vigente, requerimientos del transportista u operador, lista de señales aprobada y arquitectura de comunicaciones/ciberseguridad.

### 3.6 Equipo primario o secundario

Gobiernan la especificación particular, manual OEM, IEC/IEEE/CFE aplicable al nivel de tensión y función, e ingeniería aprobada.

### 3.7 Pruebas y aceptación

Gobiernan el procedimiento de prueba aplicable, manual OEM, especificación del equipo, norma correspondiente y criterio contractual de aceptación.

## 4. Cadena obligatoria de decisión

`OBJETO_DE_DECISION → AGENTES/MOTORES_ACTIVOS → FUENTE_RECTORA → FUENTES_COMPLEMENTARIAS → EVIDENCIA_DEL_PROYECTO → ESTADO_DE_CERTEZA`

Estados permitidos:

- `CONFIRMADO_EN_FUENTE_PRIMARIA`
- `CONFIRMADO_EN_INGENIERIA_DEL_PROYECTO`
- `COTEJABLE_PENDIENTE`
- `INDICATIVO`
- `RFI_REQUERIDA`
- `NO_APLICA`

## 5. HULKON / Drive / conocimiento de proyecto / web

- GitHub gobierna reglas y método.
- El conocimiento del proyecto y los documentos cargados son insumos autorizados, sujetos a pertenencia y trazabilidad.
- Drive/HULKON o la raíz documental autorizada constituyen el universo técnico interno a inventariar y analizar.
- La web oficial se consulta para vigencia, edición, fabricante, regulación o fuente primaria externa.
- Una fuente web no contractual no sustituye el documento contractual del proyecto.

## 6. Prohibiciones

- Iniciar análisis sin cargar reglas vigentes.
- Construir una RFI desde una sola norma sin mapear el objeto de decisión.
- Preguntar al cliente algo ya disponible en fuentes autorizadas.
- Omitir web oficial cuando la vigencia pueda haber cambiado.
- Usar blogs o resúmenes como fuente rectora cuando exista fuente primaria.
- Mencionar nombres internos del sistema en entregables externos.

## 7. Estado operativo

`R20_ACTIVA / INICIALIZACION_OBLIGATORIA / IA_TECNICA_MULTIFUENTE / FUENTE_RECTORA_POR_OBJETO_DE_DECISION`