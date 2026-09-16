# Adobe Stock AI Production OS

Sistema operativo **local-first y repo-first** para que un agente de IA pueda crear activos fotográficos comerciales para Adobe Stock con un proceso reproducible de: investigación → selección de concepto → generación → inspección → corrección → metadata → licencia → preflight → registro.

## LA REGLA DE ARRANQUE

Cuando este repositorio se entregue a un GPT/agent en un chat nuevo y el usuario diga únicamente:

> **Lee este repo.**

el agente debe tratar este repositorio como su **manual operativo principal** y continuar de forma autónoma. No debe limitarse a resumir archivos.

Debe leer en este orden:

1. `AGENT_BOOTSTRAP.md` — protocolo obligatorio de inicio.
2. `memory/CORE_MEMORY.md` — memoria persistente.
3. `prompts/MASTER_GPT_IMAGE_SYSTEM.md` — sistema maestro de producción.
4. `WORKFLOW.md` — flujo completo de principio a fin.
5. `skills/STOCK_DEMAND_RESEARCH.md` — cómo decidir qué imagen producir actualmente.
6. `skills/PRO_PHOTOGRAPHY.md` — dirección fotográfica profesional.
7. `skills/AI_ARTIFACT_QC.md` — inspección visual estricta.
8. `skills/LEGAL_IP_LICENSE.md` — propiedad intelectual, releases y licencias.
9. `skills/METADATA_AND_SUBMISSION.md` — metadata y portal.
10. `skills/PORTFOLIO_AND_SIMILARITY.md` — diferenciación y control de similitud.
11. `skills/CHAT_OUTPUT_PROTOCOL.md` — comportamiento del agente en chats nuevos.
12. `research/OFFICIAL_SOURCES.md` — fuentes oficiales y verificación.
13. `rules/ADOBE_RULES.md` — reglas consolidadas de Adobe.
14. `rules/REJECTION_GATES.md` — gates de bloqueo.
15. `rules/PLATFORM_MATRIX.md` — destinos de plataforma.
16. `templates/` — formatos de metadata y registro.

Si el agente tiene acceso web, debe **verificar las fuentes oficiales actuales antes de decidir demanda/tendencias o realizar un lote grande**. Este repositorio no debe congelar una afirmación como “la foto más vendida” sin evidencia actual.

## OBJETIVO

No perseguimos “una imagen bonita”. Producimos **stock profesional, útil, diferenciable y comercialmente reutilizable**, minimizando riesgos de:

- rechazo por calidad técnica;
- anomalías generativas;
- propiedad intelectual;
- metadata incorrecta;
- falta de releases;
- spam o contenido demasiado similar;
- licencias insuficientes del generador;
- elección de temas sin evidencia comercial o excesivamente saturados.

## PIPELINE CANÓNICO

`RESEARCH → DEMAND SCORE → CONCEPT GATE → CREATIVE BRIEF → GENERATION PROMPT → GENERATION → 100% QC → REGEN/FIX → TECHNICAL EXPORT → LEGAL/LICENSE QC → METADATA → PORTAL PREFLIGHT → READY_TO_UPLOAD`

## PRINCIPIOS NO NEGOCIABLES

1. **Nunca garantizar aprobación.** Adobe Stock toma la decisión final de moderación.
2. **Nunca confundir 4 MP con 4 MB.** Para fotos, la referencia actual es 4–100 MP y máximo 45 MB; JPEG sRGB.
3. **Nunca inventar demanda.** Las tendencias son señales; no equivalen automáticamente a ventas.
4. **Investigar antes de generar** cuando se dispone de web: tendencias oficiales, categorías destacadas, necesidades comerciales y saturación observable.
5. **Preferir conceptos diferenciados** sobre 20 variaciones casi iguales.
6. **Inspeccionar el archivo final**, no solamente la vista previa del generador.
7. **Ante una duda legal o de licencia: HOLD.** Nunca racionalizarla.
8. **Metadata basada en lo visible.** Sin keyword stuffing.
9. **Marcar IA generativa cuando corresponda.**
10. **Una imagen con un defecto material no pasa a READY_TO_UPLOAD.**

## ESTADO DE REFERENCIA

Reference date: 2026-09-17.

Las políticas de Adobe pueden cambiar. El agente debe priorizar la fuente oficial más reciente sobre cualquier texto histórico del repositorio.

## FUENTES

Las fuentes y URLs verificables están centralizadas en `research/OFFICIAL_SOURCES.md`.

## RESULTADO ESPERADO DE CADA EJECUCIÓN

El agente debe ser capaz de producir:

- concepto elegido y justificación basada en señales actuales;
- brief fotográfico profesional;
- prompt de generación listo para usar;
- negative constraints;
- checklist de inspección 100%;
- decisión `READY_TO_UPLOAD`, `REJECTED_NEEDS_FIX`, `HOLD_FOR_LEGAL_REVIEW` o `HOLD_FOR_LICENSE_REVIEW`;
- dimensiones y especificaciones técnicas;
- título en inglés;
- keywords relevantes y ordenadas;
- categoría;
- disclosure de IA;
- notas de releases/licencia;
- registro reproducible del asset.

## IMPORTANTE

Este repositorio **reduce riesgos y sistematiza el proceso**, pero no puede convertir un activo en una aprobación garantizada. El objetivo es que el agente entregue únicamente activos que, con la evidencia disponible, hayan superado todos los controles internos y estén razonablemente preparados para la revisión humana de Adobe.
