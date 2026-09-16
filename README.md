# Adobe Stock AI Production OS

Sistema operativo **repo-first** para que un agente de IA produzca activos fotográficos comerciales para Adobe Stock mediante un proceso reproducible de investigación → estrategia → dirección fotográfica → generación → inspección → corrección → metadata → licencia → preflight → registro.

## LA REGLA DE ARRANQUE

Cuando este repositorio se entregue a un GPT/agent en un chat nuevo y el usuario diga únicamente:

> **Lee este repo.**

el agente debe tratarlo como su **manual operativo principal** y continuar de forma autónoma. No debe limitarse a resumir archivos ni pedir al usuario que repita las reglas.

### Lectura obligatoria

1. `AGENT_BOOTSTRAP.md` — protocolo de inicio autónomo.
2. `memory/CORE_MEMORY.md` — memoria persistente.
3. `prompts/MASTER_GPT_IMAGE_SYSTEM.md` — sistema maestro.
4. `WORKFLOW.md` — pipeline completo.
5. `skills/STOCK_DEMAND_RESEARCH.md` — inteligencia de demanda.
6. `skills/BUYER_INTENT_AND_COMMERCIAL_VALUE.md` — necesidades de compradores.
7. `skills/COMPETITIVE_DIFFERENTIATION.md` — estrategia de diferenciación.
8. `skills/PRO_PHOTOGRAPHY.md` — dirección fotográfica.
9. `skills/IMAGE_GENERATION_ENGINEERING.md` — ingeniería de generación.
10. `skills/AI_ARTIFACT_QC.md` — control visual al 100%.
11. `skills/LEGAL_IP_LICENSE.md` — derechos, IP, releases y licencia.
12. `skills/METADATA_AND_SUBMISSION.md` — metadata y portal.
13. `skills/PORTFOLIO_AND_SIMILARITY.md` — similitud y portfolio.
14. `skills/EXPERIMENT_AND_LEARNING_LOOP.md` — aprendizaje basado en evidencia.
15. `skills/CHAT_OUTPUT_PROTOCOL.md` — formato de ejecución.
16. `research/OFFICIAL_SOURCES.md` — fuentes de verificación.
17. `research/DEMAND_SNAPSHOT_2026-09-17.md` — snapshot histórico de señales actuales.
18. `rules/ADOBE_RULES.md`, `rules/REJECTION_GATES.md`, `rules/SAFETY_BARRIER_MATRIX.md`, `rules/OUTPUT_DELIVERY_GATE.md`.
19. `templates/` — metadata y submission record.

## OBJETIVO

No perseguimos “una imagen bonita” ni volumen indiscriminado. Producimos **stock profesional, útil, diferenciado y comercialmente reutilizable**, maximizando el valor para compradores y minimizando riesgos de rechazo.

El agente debe distinguir siempre entre:

- **evidencia de plataforma**;
- **evidencia del propio portfolio/cuenta**;
- **hipótesis de mercado**.

No inventará ventas, rankings ni probabilidades de aprobación.

## INTELIGENCIA DE MERCADO

Cuando hay acceso web, el agente debe volver a comprobar antes de cada nueva dirección de producción:

- tendencias oficiales de Adobe Stock;
- colecciones destacadas;
- guías de Premium Collection;
- misiones/briefs disponibles;
- cambios de políticas;
- prácticas actuales de metadata;
- rechazo/similitud y restricciones vigentes;
- señales contemporáneas de necesidades de compradores.

Las tendencias de Adobe son señales editoriales/curatoriales, no un ranking público de ventas. Una afirmación como “esta es la foto más pedida” requiere evidencia directa y actual.

## PIPELINE CANÓNICO

`LIVE RESEARCH → SIGNAL EXTRACTION → BUYER INTENT → 3+ CANDIDATES → DIFFERENTIATION GAP → CONCEPT GATE → PHOTO BRIEF → GENERATION ENGINEERING → GENERATE → UPSCALE/EXPORT → OUTPUT DELIVERY GATE → 100% QC → FIX/REGENERATE → TECHNICAL EXPORT → LEGAL/LICENSE QC → METADATA SEO → PORTAL PREFLIGHT → PORTFOLIO CHECK → READY_TO_UPLOAD`

## ESTRATEGIA DE COMPETENCIA

La ventaja no se obtiene copiando a otros colaboradores ni generando 100 variantes. Se busca ventaja mediante:

- art direction precisa;
- realismo y física creíbles;
- composición útil para diseño;
- contexto contemporáneo y específico;
- concepto distinto de los clichés genéricos;
- copy space intencional;
- materiales y superficies convincentes;
- selección estricta de outputs;
- metadata limpia y orientada a búsqueda;
- portfolio con huecos cubiertos y poca redundancia.

Adobe recomienda diversificar conceptos, curar outputs y evitar variaciones casi idénticas porque la similitud puede provocar rechazo y reducir la visibilidad.

## PRINCIPIOS NO NEGOCIABLES

1. **Nunca garantizar aprobación o ventas.** Adobe decide la moderación y el mercado decide las compras.
2. **4 MP no es 4 MB.** Para fotos, usar la especificación vigente almacenada en las reglas y comprobarla en Adobe antes de trabajo masivo.
3. **No inventar demanda.** Diferenciar señal, hipótesis y dato real.
4. **Investigar antes de generar** cuando existe web.
5. **No competir mediante spam.** Cada envío debe aportar valor distintivo.
6. **Inspeccionar el archivo final al 100%.**
7. **El archivo descargable debe pasar `OUTPUT_DELIVERY_GATE`.** Una preview de baja resolución nunca se considera el asset final.
8. **Ante dudas legales o de licencia: HOLD.**
9. **Metadata basada estrictamente en lo visible y buscable.**
10. **Etiquetar IA generativa cuando corresponda.**
11. **Cualquier defecto material bloquea READY_TO_UPLOAD.**
12. **Registrar resultados** para que la estrategia mejore con evidencia real.
13. **Nunca imitar portfolios, campañas, artistas, marcas, personajes o trabajos protegidos.**

## ESTADO DE REFERENCIA

Reference date: 2026-09-17.

Las políticas y tendencias son volátiles. El agente debe priorizar siempre las fuentes oficiales actuales sobre snapshots históricos del repositorio.

## FUENTES

Las URLs oficiales están centralizadas en `research/OFFICIAL_SOURCES.md`.

## RESULTADO ESPERADO

Cada ejecución debe poder producir, según el estado:

- señales actuales y fuentes;
- candidatos comparados;
- concepto elegido;
- buyer/use-case rationale;
- gap competitivo;
- brief fotográfico profesional;
- prompt de generación;
- negative constraints;
- archivo final validado por resolución y exportación;
- QC 100%;
- especificaciones técnicas;
- title/keywords/category;
- AI disclosure;
- license/release notes;
- portfolio/similarity decision;
- final status;
- audit trail.

## LIMITACIÓN DEL SISTEMA

Este repositorio **reduce riesgos y sistematiza el proceso**, pero no puede convertir la moderación ni las ventas en algo determinista. Su función es elevar sistemáticamente la calidad, relevancia, diferenciación, discoverability y preparación comercial de cada asset con la mejor evidencia disponible.
