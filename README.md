# Adobe Stock AI Image System

Sistema operativo para crear, revisar y preparar contenido generado con IA para Adobe Stock.

> **Importante:** ningún prompt puede garantizar que Adobe Stock apruebe una imagen. La aprobación depende de la revisión de Adobe y de las políticas vigentes. Este repositorio busca reducir rechazos mediante generación controlada, revisión técnica, IP/legal, metadata y control de similitud.

## Objetivo

Flujo:

`idea comercial -> preflight -> prompt -> generación -> inspección 100% -> corrección/regeneración -> metadata -> revisión de licencia -> portal Adobe -> moderación -> registro`

## Estructura

- `prompts/MASTER_GPT_IMAGE_SYSTEM.md` — sistema maestro para GPT.
- `prompts/IMAGE_GENERATION_PROMPT_TEMPLATE.md` — plantilla de generación.
- `prompts/IMAGE_QC_REVIEW_PROMPT.md` — auditoría visual/técnica antes de subir.
- `templates/ADOBE_METADATA_TEMPLATE.md` — metadata.
- `templates/SUBMISSION_RECORD.md` — registro por asset.
- `rules/ADOBE_RULES.md` — reglas operativas consolidadas.
- `rules/PLATFORM_MATRIX.md` — qué plataformas usar con IA.
- `rules/REJECTION_GATES.md` — gates de bloqueo.

## Regla principal

**No subir automáticamente.** Una imagen solo entra en `READY_TO_UPLOAD` cuando pasa todos los gates y no tiene dudas legales, técnicas o de calidad.

## Fecha de referencia

17 de septiembre de 2026.

## Fuentes

Ver `rules/ADOBE_RULES.md` y `rules/PLATFORM_MATRIX.md`. Verificar siempre las páginas oficiales antes de operaciones masivas porque las políticas pueden cambiar.
