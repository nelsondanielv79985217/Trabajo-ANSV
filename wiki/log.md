# Log

Registro cronológico, append-only. No editar entradas pasadas — solo agregar al final.

## [2026-09-23] setup | Creación de la wiki (Paso 0)

- Se creó la estructura `/wiki` (`fuentes/`, `conceptos/`, `entidades/`, `sintesis/`, `index.md`, `log.md`) y `CLAUDE.md` en la raíz del repo, replicando el schema ya validado en `nelsondanielv79985217/programaGradoInnovacion` (rama `claude/llm-wiki-setup-nht7xw`, carpeta `/wiki`), adaptado a las reglas específicas de este proyecto (fuente exclusiva, citación exacta con página, APA 7, sin alucinación — ver `CLAUDE.md`).
- Se relevaron por nombre de archivo las 46 fuentes crudas de la raíz del repo (leyes, decretos, resoluciones, procedimientos y anexos del sistema de gestión ANSV/DCI, protocolos del Plan 365, planeación sectorial, correspondencia oficial, conceptos jurídicos, contratación, financiamiento/cooperación y productos propios del proyecto) y se listaron en `index.md`, agrupadas por categoría temática.
- Se migró la única página preexistente (`procedimiento-asistencia-tecnica-pr06.md`, en la raíz, ya redactada en formato compatible con `type: fuente`) a `wiki/fuentes/ansv-pr-06-procedimiento-asistencia-tecnica.md`, agregándole el front matter obligatorio del schema. Se marcó `status: incierto` (no `ingerido`) porque el resumen no registra número de página para ninguna afirmación, lo que impide citarla en el cuerpo de la tesis bajo la regla de citación exacta del proyecto — queda pendiente reabrir el PDF y anotar ubicaciones exactas.
- Un archivo (`ANEXO4~1.PDF`) tiene nombre truncado estilo DOS 8.3; su contenido real no fue verificado todavía (se marca como pendiente identificar en `index.md`, siguiendo la práctica documentada en el repo de referencia para casos análogos).
- No se leyó el contenido completo de ningún PDF/DOCX en este paso (salvo la página ya existente). El INGEST detallado de cada fuente, con número de página para cada dato citable, se hace uno por uno en turnos siguientes, con el usuario involucrado en cada paso (flujo INGEST de `CLAUDE.md`), salvo que el usuario pida explícitamente procesar en lote.

## [2026-09-23] ingest | Anexo 1 — ANSV-CPP-CA-02 (Caracterización del proceso)

- Se leyó completo (3 páginas) `Anexo 1. Caracterización ANSV-CPP-CA-02.pdf` y se creó `wiki/fuentes/ansv-ca-02-caracterizacion-anexo1.md`, `status: ingerido`, con citación por página para cada dato relevante.
- **Hallazgo que corrige la página de PR-06**: PR-06 no es el documento ancla del que "se desprenden" los anexos, como asumía esa página al escribirse sin haber leído este anexo. CA-02 caracteriza el proceso misional completo ("Coordinación y Articulación para la Implementación de la Política Pública en Seguridad Vial"); la asistencia técnica de PR-06 es una sola actividad del ciclo "Hacer" de ese proceso (CA-02, p. 2), junto con otras actividades no cubiertas por PR-06 (reportes de avance del PNSV, participación en instancias territoriales). Se actualizó la sección "Conexiones" de `wiki/fuentes/ansv-pr-06-procedimiento-asistencia-tecnica.md` para reflejar la jerarquía correcta (no se tocó su `status: incierto`, que sigue vigente por la falta de citación por página en esa página).
- Se creó `wiki/entidades/dci-direccion-coordinacion-interinstitucional.md` (primera entidad de la wiki), con link desde ambas fuentes que la mencionan.
- Se actualizó `index.md`: fuentes (PR-06 y CA-02) y entidades.
- Incertidumbre abierta: el documento remite indicadores, riesgos y normograma a un aplicativo SIG externo no accesible desde este repositorio — queda fuera del alcance de la fuente.
- Pendiente confirmación del usuario antes de continuar con el Anexo 3 (ANSV-CPP-PR-07).
