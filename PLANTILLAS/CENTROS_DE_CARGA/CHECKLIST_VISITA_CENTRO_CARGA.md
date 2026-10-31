# Checklist técnico de campo — centro de carga
**JULCON v13.1 · uso inicial · INTERNO / NO EMITIBLE**. No realizar operaciones ni ensayos sin permisos y procedimiento. Todo campo sin evidencia queda **TBD**.

## 0. Antes de entrar: seguridad y alcance
- [ ] Confirmar autorización de acceso, responsable de sitio, anfitrión, permisos de fotos y restricciones de áreas.
- [ ] Revisar inducción, EPP, análisis de riesgos, proximidad a partes energizadas y limitaciones de observación; no abrir equipos energizados.
- [ ] Definir objetivo: reconocimiento, cambio de suministrador, incremento de demanda, mantenimiento, CR, medición u otro (marcar lo **declarado**, no asumir).
- [ ] Definir activos visitables, límites físicos, participantes y fuentes disponibles.
- [ ] Identificar qué datos son confidenciales y dónde se custodiarán (nunca Bootstrap público).

## 1. Identidad del centro de carga y frontera
- [ ] Nombre, razón social, ubicación, contactos técnicos autorizados, fecha y horario.
- [ ] RPU/identificador y contrato de servicio/suministro, si se entregan.
- [ ] Suministrador, operador responsable, estado contractual y regulatorio **por comprobar en fuente primaria**.
- [ ] Punto físico de suministro/conexión, titularidad de equipos, frontera mantenimiento/operación.
- [ ] Tipo de acometida: directa, TAP, línea dedicada, seccionamiento, bus, doble alimentación, transferencia (TBD si no existe plano).
- [ ] Unifilar vigente, revisiones, aprobaciones, diferencias visuales.

## 2. Capacidad y calidad eléctrica
- [ ] Tensión(es) nominales de alimentación y distribución; frecuencia y niveles MT/BT/AT.
- [ ] Potencia contratada/demanda máxima, curva 12 meses, consumo y factor de potencia (solo fuentes).
- [ ] Transformadores: cantidad, placa, kVA/MVA, tensiones, conexión, impedancia, enfriamiento, taps, año y estado observado.
- [ ] Barras, interruptores, cuchillas, fusibles, TC/TP: placas, capacidades, clase, relaciones y condición **sin intervenir**.
- [ ] Características de cargas relevantes, motores grandes, variadores, hornos, inversores, generación propia, BESS y expansiones.
- [ ] Registros de eventos, disturbios, calidad de energía, armónicos, flicker, tensión y PF; no declarar Código de Red cumplido sin estudio.
- [ ] Existencia de estudios de carga, cortocircuito, coordinación, arco eléctrico y puesta a tierra; fecha/revisión.

## 3. Protecciones, medición y comunicaciones
- [ ] Arquitectura de protecciones y control; identificación de relevadores, lógica de disparo y registros de pruebas.
- [ ] Medición fiscal: medidores, placa, TC/TP, sellos, gabinete, principal/respaldo y comunicaciones (sin retirar sellos).
- [ ] Comunicaciones hacia operador/suministrador, canales, FO/radio/módem, sincronismo horario, ciberseguridad y propiedad.
- [ ] SCADA, telemetría, alarmas y señales requeridas: existencia documental, no asumir interoperabilidad.
- [ ] Servicios auxiliares AC/DC, banco de baterías, cargadores y planos disponibles.

## 4. Obra civil, operación y mantenimiento
- [ ] Layout, accesos, distancias, cimentaciones, canalizaciones, drenaje, contención de aceite y espacio para expansión.
- [ ] Condiciones ambientales: contaminación industrial/salinidad, altitud, humedad y exposición; verificaciones posteriores de distancia de fuga.
- [ ] Estado visible de conexiones, aisladores, corrosión, fugas, etiquetas y barreras, sin diagnosticar con certeza por fotografía.
- [ ] Programa y reportes de mantenimiento, pruebas FAT/SAT/comisionamiento, inspecciones y no conformidades.
- [ ] Accesos a planimetría, catálogos, memorias, especificaciones técnicas y actas CFE/CENACE cuando correspondan.

## 5. Gestión documental y salidas
- [ ] Inventariar cada archivo visto con nombre, tipo, revisión, fuente, raíz, hash si hay copia autorizada y alcance de revisión.
- [ ] Distinguir `CONFIRMADO / INTERPRETACIÓN / SUPUESTO / TBD`; cada dato confirmado debe enlazar evidencia.
- [ ] Listar documentos no entregados y fuentes cuya inexistencia NO está comprobada.
- [ ] Dibujar un mapa preliminar de equipos y fronteras como hipótesis, sujeto a unifilar.
- [ ] Identificar riesgos de seguridad inmediatos para notificar al responsable del sitio, sin emitir dictamen pericial.
- [ ] Preparar minuta interna, matriz de levantamiento, acciones por responsable y RFI condicionados a inventario R0/R2/R5.

## Resultado
`OBSERVACION_DE_CAMPO` no es `ESTUDIO`, `CONFORMIDAD`, `READY`, `R25_PASS` ni autorización de un documento emitible.
