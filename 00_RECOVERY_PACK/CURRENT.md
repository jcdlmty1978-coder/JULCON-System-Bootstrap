# CURRENT — JULCON
**Estado:** PUNTERO DE GOBIERNO / USO INTERNO / NO EMITIBLE POR SÍ SOLO

## Pack activo propuesto para integración PR-1

- `PACK_ACTIVO`: `JULCON_v13_2`
- `RUTA`: `ARRANQUE.md`
- `ENTRADA`: `ARRANQUE.md`
- `INDICE`: `REGLAS.yaml`
- `REGLAS`: `REGLAS/`
- `ESTADO`: `VIGENTE` **únicamente cuando este commit sea integrado a main y ratificado por Dirección**

## Orden obligatorio de lectura
1. Verificar `main@SHA` y la ratificación formal (una rama PR no es gobierno canónico).
2. Leer `CLAUDE.md`, `ARRANQUE.md` y este `CURRENT.md`.
3. Leer `SEGURIDAD.md`, `CAPACIDADES.md`, `REGLAS.yaml` y los textos íntegros de `REGLAS/` aplicables.
4. Ejecutar la plantilla `PLANTILLAS/CLAUDE_BOOTSTRAP_JULCON_PROYECTO_NUEVO_GITHUB_ONLY.md` o la plantilla de continuidad que corresponda, sin abrir documentos del cliente durante la carga de gobierno.
5. Inventario R4, fuentes y controles humanos antes de emitir.

## Histórico congelado
- Pack JULCON v13.1 íntegro: `99_OBSOLETO/JULCON_v13_1/`.
- Etiqueta histórica inmutable de consulta: `v13.1-final` → `4de49d6b58dab0309442bbe227a28e76575378da`.
- No se deben usar rutas antiguas del pack como rutas operativas.

**Límite de integración:** Mientras el PR-1 no se fusione y ratifique, el gobierno activo de GitHub sigue siendo `main` y este archivo es contenido candidato de la rama. El estado `VIGENTE` aquí no autoriza a un agente a anticipar el merge, crear la etiqueta `v13.2.0`, activar motores ni emitir ingeniería.
