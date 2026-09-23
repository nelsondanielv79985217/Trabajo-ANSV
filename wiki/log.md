# Log

Registro cronológico, append-only. No editar entradas pasadas — solo agregar al final.

## [2026-09-23] setup | Creación de la wiki (Paso 0)

- Se creó la estructura `/wiki` (`fuentes/`, `conceptos/`, `entidades/`, `sintesis/`, `index.md`, `log.md`) y `CLAUDE.md` en la raíz del repo, replicando el schema ya validado en `nelsondanielv79985217/programaGradoInnovacion` (rama `claude/llm-wiki-setup-nht7xw`, carpeta `/wiki`), adaptado a las reglas específicas de este proyecto (fuente exclusiva, citación exacta con página, APA 7, sin alucinación — ver `CLAUDE.md`).
- Se relevaron por nombre de archivo las 46 fuentes crudas de la raíz del repo (leyes, decretos, resoluciones, procedimientos y anexos del sistema de gestión ANSV/DCI, protocolos del Plan 365, planeación sectorial, correspondencia oficial, conceptos jurídicos, contratación, financiamiento/cooperación y productos propios del proyecto) y se listaron en `index.md`, agrupadas por categoría temática.
- Se migró la única página preexistente (`procedimiento-asistencia-tecnica-pr06.md`, en la raíz, ya redactada en formato compatible con `type: fuente`) a `wiki/fuentes/ansv-pr-06-procedimiento-asistencia-tecnica.md`, agregándole el front matter obligatorio del schema. Se marcó `status: incierto` (no `ingerido`) porque el resumen no registra número de página para ninguna afirmación, lo que impide citarla en el cuerpo de la tesis bajo la regla de citación exacta del proyecto — queda pendiente reabrir el PDF y anotar ubicaciones exactas.
- Un archivo (`ANEXO4~1.PDF`) tiene nombre truncado estilo DOS 8.3; su contenido real no fue verificado todavía (se marca como pendiente identificar en `index.md`, siguiendo la práctica documentada en el repo de referencia para casos análogos).
- No se leyó el contenido completo de ningún PDF/DOCX en este paso (salvo la página ya existente). El INGEST detallado de cada fuente, con número de página para cada dato citable, se hace uno por uno en turnos siguientes, con el usuario involucrado en cada paso (flujo INGEST de `CLAUDE.md`), salvo que el usuario pida explícitamente procesar en lote.
