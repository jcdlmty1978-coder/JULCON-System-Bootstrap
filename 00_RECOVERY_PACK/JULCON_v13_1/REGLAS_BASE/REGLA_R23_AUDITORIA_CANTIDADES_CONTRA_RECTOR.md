# REGLA R23 — AUDITORÍA DE CANTIDADES CONTRA DOCUMENTO RECTOR

**Sistema:** JULCON v13.1  
**Ámbito:** REGLA_GLOBAL / REGLA_BASE_CANONICA  
**Estado:** REGLA_PROTEGIDA / ACTIVA

## 1. Criterio rector

Todo catálogo, Libro Maestro o despiece generado con cobertura documental parcial debe re-auditarse **partida por partida contra los documentos rectores** cuando la cobertura se complete, antes de ratificarse o utilizarse para RFQ o CAPEX.

## 2. Cláusulas obligatorias

1. Toda obligación expresada como razón —“por cada X”— debe expandirse contando las instancias reales de `X`. La cantidad resultante se escribe explícitamente y conserva memoria de cálculo.
2. La unidad debe ser cotizable. `LOTE` o `PZA` usados indebidamente para cables, conductores o materiales lineales deben convertirse a m, kg o pzas. Los juegos se expresan como `1 lote (N pzas)`.
3. Toda obra o suministro presente en dos frentes exige frontera declarada con titular único. El frente no titular se registra como interfaz. El doble conteo bloquea RFQ.
4. Los errores detectados se informan antes de generar el entregable corregido, identificando frente, partida, celda y fuente.
5. No se ratifican cantidades heredadas por plantilla, analogía o catálogo previo sin cotejo con el proyecto actual.
6. Toda cantidad conserva procedencia y estado: confirmada, calculada, estimada, pendiente de RFI o no aplicable.

## 3. Gate previo a RFQ / CAPEX

Se debe confirmar:

- cobertura o brechas declaradas;
- cantidades expandidas;
- unidades cotizables;
- memoria de cálculo;
- fronteras de alcance;
- ausencia de doble conteo;
- trazabilidad a fuente rectora.

Si falta alguno:

`AUDITORIA_CANTIDADES_PENDIENTE / RFQ_BLOQUEADO / CAPEX_NO_RATIFICADO`

## 4. Estado operativo

`R23_ACTIVA / AUDITORIA_PARTIDA_POR_PARTIDA / UNIDAD_COTIZABLE_OBLIGATORIA / DOBLE_CONTEO_BLOQUEANTE`