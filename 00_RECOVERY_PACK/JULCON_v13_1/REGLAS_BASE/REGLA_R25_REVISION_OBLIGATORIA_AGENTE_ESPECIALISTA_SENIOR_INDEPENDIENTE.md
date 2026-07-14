# REGLA R25 — REVISIÓN OBLIGATORIA POR AGENTE ESPECIALISTA SENIOR INDEPENDIENTE

**Sistema:** JULCON v13.1  
**Ámbito:** REGLA_GLOBAL / REGLA_BASE_CANONICA  
**Estado:** REGLA_PROTEGIDA / ACTIVA / INVIOLABLE

## 1. Principio rector

El agente que construye no puede ser el único que aprueba. Todo proyecto, Libro Maestro, despiece, RFQ, CAPEX, RFI técnico, memoria, estudio, dictamen o entregable crítico debe pasar por una segunda revisión independiente, ejecutada por uno o más agentes especialistas senior de las disciplinas que afecten el alcance.

Checklist cumplido no equivale a validación técnica senior. La revisión senior complementa el gate documental y no sustituye la ratificación del director EPC ni las aprobaciones profesionales, contractuales o regulatorias aplicables.

## 2. Independencia obligatoria

1. Separar explícitamente `ROL_CONSTRUCTOR` y `ROL_REVISOR_SENIOR_INDEPENDIENTE`.
2. El revisor debe desafiar el trabajo, detectar omisiones, contradicciones, supuestos no declarados, doble conteo y fuentes mal aplicadas.
3. Si la misma plataforma ejecuta ambos roles, debe registrar entradas revisadas, hallazgos propios y discrepancias.
4. La revisión por IA no se presenta como firma profesional ni validación humana.

## 3. Activación

R25 se activa antes de ratificar LM, catálogo, despiece, RFQ, CAPEX, RFI técnico, cálculos, memorias, criterios de diseño, estudios, fronteras de alcance o entregables que afecten seguridad, cumplimiento, costo, plazo, construcción, pruebas u operación.

## 4. Selección del especialista

El perfil senior se selecciona por objeto de decisión conforme a R20. Un entregable multidisciplinario exige revisión senior multidisciplinaria. Ningún perfil aprueba materias fuera de su competencia declarada.

## 5. Revisión mínima

El revisor senior debe comprobar, según aplique:

- objeto y alcance;
- cobertura y pertenencia documental;
- fuente rectora y verificación normativa;
- cálculos, hipótesis, cantidades y unidades;
- ingenierías obligadas vs ofrecidas;
- interfaces multidisciplinarias;
- constructibilidad, mantenibilidad y pruebas;
- criterios de aceptación;
- riesgos técnicos, de seguridad, costo y plazo;
- consistencia entre planos, LM, catálogo, memorias, especificaciones y RFIs;
- emitibilidad y reservas.

Debe consultar fuentes directamente y ejecutar recálculo o cotejo independiente cuando existan fórmulas, cantidades o decisiones de diseño.

## 6. Estados permitidos

- `APROBADO_POR_REVISION_SENIOR`
- `APROBADO_CON_RESERVAS_SENIOR`
- `CORRECCION_REQUERIDA`
- `RFI_REQUERIDA`
- `RECHAZADO_POR_REVISION_SENIOR`
- `R25_NO_APLICA_CON_FUNDAMENTO`

## 7. Escalamiento

Las discrepancias quedan registradas. Las decisiones de diseño, homologación, excepción o aceptación de riesgo se escalan al director EPC. Si falta fuente primaria, dato de campo o definición contractual, se abre RFI y no se fuerza una conclusión.

## 8. Gate

Si R25 aplica y no existe evidencia de revisión senior independiente:

`REVISION_SENIOR_NO_EJECUTADA / RATIFICACION_BLOQUEADA / NO_EMITIBLE`

Si existen hallazgos críticos abiertos:

`HALLAZGO_SENIOR_CRITICO_ABIERTO / NO_EMITIBLE`

## 9. Estado operativo

`R25_ACTIVA / REVISION_SENIOR_INDEPENDIENTE_OBLIGATORIA / CONSTRUCTOR_DISTINTO_DE_REVISOR / SEGUNDA_LINEA_DE_DEFENSA / GATE_PRE_RATIFICACION`