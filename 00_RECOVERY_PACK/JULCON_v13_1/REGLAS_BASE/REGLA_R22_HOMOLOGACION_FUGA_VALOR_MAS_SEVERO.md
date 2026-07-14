# REGLA R22 — HOMOLOGACIÓN DE DISTANCIA DE FUGA AL VALOR MÁS SEVERO

**Sistema:** JULCON v13.1  
**Ámbito:** REGLA_GLOBAL / REGLA_BASE_CANONICA (diseño AT)  
**Estado:** REGLA_PROTEGIDA / ACTIVA

## 1. Criterio rector

En proyectos de subestaciones o líneas de alta tensión, cuando el ambiente sea de contaminación pesada y/o coexistan en el mismo sitio equipos con distintas clases de distancia de fuga, el agente debe levantar proactivamente la homologación de todo el equipo del sitio al **valor más severo aplicable**, en lugar de quedarse con el mínimo aislado de un documento rector.

## 2. Cláusulas obligatorias

1. No deben coexistir clases de fuga distintas sin justificación técnica expresa. La propuesta se formula hacia arriba.
2. Especificar por encima del mínimo puede ser válido y más robusto; se registra como criterio de diseño `DF-<TENSION>-<PROYECTO>-NN`.
3. La homologación debe ser ratificada por el director EPC y documentada en la memoria de coordinación de aislamiento.
4. El agente propone y traza; nunca degrada una distancia de fuga ya especificada.
5. La base debe indicar `Um`, criterio en mm/kV, valor total requerido, ambiente y fuentes.
6. Toda cifra fina queda sujeta a R7 y verificación en fuente primaria o documento contractual.

## 3. Salida obligatoria

- equipos afectados;
- valores detectados;
- fuente de cada valor;
- ambiente del sitio;
- propuesta de homologación;
- decisión pendiente o ratificada;
- impacto en RFQ, compra, ingeniería y pruebas.

## 4. Estado operativo

`R22_ACTIVA / HOMOLOGACION_FUGA_HACIA_ARRIBA / RATIFICACION_DIRECTOR_EPC_REQUERIDA / COORDINACION_AISLAMIENTO_OBLIGATORIA`