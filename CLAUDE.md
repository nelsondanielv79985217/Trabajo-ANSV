# CLAUDE.md — Schema de la LLM Wiki

Este archivo define cómo Claude debe mantener la wiki de este repositorio. Se ajusta con el uso: si algo acá no funciona en la práctica, se discute con el usuario y se corrige.

Estructura y flujo inspirados, con adaptaciones, en el repositorio hermano `programaGradoInnovacion` (rama `claude/llm-wiki-setup-nht7xw`, carpeta `wiki/`) — mismo método de organización documental, aplicado acá a un corpus distinto y con un propósito distinto (ver nota abajo).

## Propósito

Este repo es la base documental de **trabajo del usuario en la Agencia Nacional de Seguridad Vial (ANSV)**, específicamente en o en relación con la **Dirección de Coordinación Interinstitucional (DCI)** — normativa, procedimientos, planes y correspondencia institucional en materia de seguridad vial, incluyendo el protocolo de asistencia técnica que la DCI ejecuta con municipios y organismos de tránsito. **No es el repositorio de la tesis de maestría del usuario** — esa tesis se documenta y desarrolla en el repositorio `programaGradoInnovacion`. Este repo es de uso laboral/profesional: sirve para responder consultas de trabajo, preparar intervenciones institucionales, análisis normativos y de política pública, y cualquier otra tarea derivada de las funciones del usuario en la ANSV — no para producir un documento académico con jurado evaluador.

Las fuentes son normativa nacional, procedimientos y anexos del Sistema Integrado de Gestión de la ANSV, planes y documentos técnicos de política pública en seguridad vial, y correspondencia institucional (oficios, circulares). En vez de releer y re-derivar todo desde cero cada vez que se necesita algo de ellas, se mantiene una wiki en Markdown (`/wiki`) que acumula resúmenes, páginas de conceptos/entidades, y un índice — así el trabajo de lectura y síntesis se conserva entre sesiones.

## Reglas del proyecto (obligatorias, definidas por el usuario — no negociables por Claude)

Estas reglas gobiernan todo el trabajo en este repositorio y tienen prioridad sobre cualquier convención genérica de este schema:

1. **Fuente exclusiva**: solo se puede usar información contenida en los archivos/documentos subidos a este repo. No se usa conocimiento general, memoria propia, ni resultados de búsqueda externa como sustento de una respuesta o de contenido de la wiki, salvo pedido explícito del usuario para un propósito distinto (ej. contexto normativo público, o un análisis marcado explícitamente como opinión propia).
2. **Citación exacta obligatoria**: todo dato, cifra, argumento o cita textual debe indicar documento, sección/apartado y **número de página exacto** (o sección/pregunta si el documento no tiene paginación explotable, dejándolo dicho explícitamente). Si no se puede identificar la ubicación exacta, se debe decir explícitamente en vez de aproximarla.
3. **Sin datos disponibles = decirlo**: si algo no está en los documentos cargados, la respuesta es "esto no está en las fuentes del proyecto" — nunca completar, inferir o inventar.
4. **Rigor metodológico**: toda afirmación causal, diagnóstica o de recomendación debe estar respaldada por fuente y página explícitas. Una opinión propia (del usuario o de Claude) debe marcarse claramente como tal — esto es especialmente importante porque el contenido de esta wiki puede usarse para preparar intervenciones, respuestas institucionales o decisiones de trabajo reales.
5. **Retroalimentación crítica activa**: ante una debilidad, vacío, supuesto no sustentado o inconsistencia con las fuentes, señalarlo directamente y proponer una alternativa — no validar sin más.

No se exige un formato de citación académico (APA u otro) ni se escribe pensando en un jurado evaluador — la audiencia es el propio usuario y, eventualmente, sus contrapartes institucionales en la ANSV. La exigencia de citación exacta (regla 2) se mantiene igual de estricta que antes: sigue siendo la base para poder responder con precisión en un contexto de trabajo donde una cifra o cita mal atribuida tiene consecuencias reales.

## Arquitectura de 3 capas (no mezclar)

1. **Fuentes crudas** — los archivos que ya existen en la raíz del repo (PDF y DOCX). Son **inmutables**: se leen, nunca se editan ni se mueven sin pedido explícito del usuario.
2. **Wiki** (`/wiki`) — páginas `.md` generadas y mantenidas enteramente por Claude: resúmenes, páginas de entidades/conceptos, índice, log.
3. **Schema** (este archivo) — estructura, convenciones y flujo de trabajo. Se co-crea y ajusta con el usuario.

## Estructura de `/wiki`

```
/wiki
  index.md          # catálogo de todas las páginas, por categoría
  log.md             # log cronológico append-only
  fuentes/           # una página por fuente cruda (PDF/DOCX) — resumen + hallazgos + metadatos + páginas exactas
  conceptos/         # páginas hub de temas transversales que cruzan varias fuentes
  entidades/         # páginas de instituciones, dependencias o personas recurrentes
  sintesis/          # páginas de síntesis cruzada / respuestas de QUERY guardadas
```

Tipos de página:
- **fuente** — un documento del repo (PDF o DOCX). Resume objeto, contenido clave, hallazgos y relevancia para el trabajo en la ANSV, siempre con número de página cuando la fuente lo permite. Nunca reemplaza al documento original, es un resumen navegable con referencias precisas.
- **concepto** — un tema transversal (ej. "Asistencia Técnica como mecanismo de transferencia de conocimiento", "Plan 365", "Sistema Seguro"). Agrega qué dice cada fuente sobre ese tema, con links a `fuentes/` y páginas exactas.
- **entidad** — una dependencia (ej. DCI-ANSV), institución externa (municipio, organismo de tránsito, Superintendencia, Procuraduría) o persona firmante recurrente.
- **sintesis** — cruces entre conceptos/fuentes que valen la pena conservar (ej. respuestas de QUERY que el usuario decide guardar, insumos para una intervención o comunicación institucional).
- **metodo** — referencias metodológicas transversales, si se incorporan.

Una página de concepto/entidad se crea la primera vez que hace falta (durante un INGEST), no se prepoblán de antemano — evita inventar categorías antes de tener evidencia real de que se repiten.

## Convenciones de nombres

- Un archivo por página, ruta = `wiki/<carpeta>/<slug>.md`.
- Slug: ASCII kebab-case, sin tildes ni mayúsculas, derivado del título. Ej: `fuentes/ansv-pr-06-procedimiento-asistencia-tecnica.md`.
- No duplicar páginas: antes de crear una nueva página de concepto/entidad, buscar si ya existe una con el mismo tema.
- Links entre páginas: rutas relativas Markdown estándar, ej. `[Asistencia Técnica](../conceptos/asistencia-tecnica.md)`.

## Front matter (obligatorio en toda página)

```yaml
---
title: "Título legible de la página"
type: fuente | concepto | entidad | sintesis | metodo
tags: [tag1, tag2]
fuente_pdf: "nombre-exacto-del-archivo.pdf"   # solo en type: fuente; usar el nombre exacto tal como está en el repo, aunque sea un nombre truncado estilo DOS 8.3
status: pendiente-ingest | ingerido | incierto
last_updated: YYYY-MM-DD
---
```

## `index.md`

Catálogo de todas las páginas, agrupado por categoría (Fuentes / Conceptos / Entidades / Síntesis). Las fuentes pendientes de ingest se agrupan por tipo documental visible en el nombre de archivo (normativa, procedimientos SGC-DCI, Plan 365, planes/documentos técnicos, correspondencia) — esta agrupación es solo organizativa por nombre de archivo, no implica haber leído el contenido. Cada fila: `- [Título](ruta) — resumen de una línea con página si aplica. (status)`. Se actualiza en cada INGEST/QUERY que agregue o modifique una página.

## `log.md`

Registro cronológico, **append-only** (nunca se edita retroactivamente, solo se agrega al final). Formato de entrada:

```
## [YYYY-MM-DD] tipo | Nombre de la fuente o tema
- qué se hizo
- páginas creadas/actualizadas
```

`tipo` ∈ `{setup, ingest, query, lint}`.

## Flujo INGEST

Se procesa **una fuente a la vez** — nunca todo el repo de una pasada, salvo pedido explícito del usuario. El usuario se queda involucrado revisando cada actualización antes de seguir con la próxima ("metodología Karpathy": un paso, revisar el resultado, recién ahí seguir con el próximo).

1. Leer la fuente completa (PDF/DOCX vía skill correspondiente), **registrando el número de página de cada dato, cifra o cita relevante** — esto es obligatorio en este proyecto (ver "Reglas del proyecto" arriba), no opcional.
2. Discutir los puntos clave con el usuario (objeto del documento, contenido normativo/procedimental, hallazgos, relevancia para el protocolo de asistencia técnica).
3. Escribir/actualizar la página de `fuentes/`, con página exacta en cada afirmación citable. Puede tocar varias páginas: crear/actualizar conceptos y entidades relevantes con link a esta fuente.
4. Marcar explícitamente cualquier vacío o ambigüedad con `[INCIERTO: ...]` y `status: incierto` — nunca completar con supuestos.
5. Actualizar `index.md`.
6. Agregar entrada a `log.md` con prefijo `## [YYYY-MM-DD] ingest | <nombre de la fuente>`.
7. Pausar y esperar confirmación del usuario antes de pasar a la próxima fuente.

## Flujo QUERY

1. Buscar primero en `index.md`.
2. Entrar a las páginas relevantes (`fuentes/`, `conceptos/`, `entidades/`, `sintesis/`) y sintetizar con referencias explícitas (documento + página).
3. Si un dato no tiene página registrada en la wiki, decirlo en vez de aproximarla, y proponer volver a la fuente cruda para el INGEST correspondiente.
4. Si la respuesta vale la pena conservar, proponer guardarla como página nueva en `sintesis/` en vez de que se pierda en el chat.

## Flujo LINT

Cuando se pida, revisar la wiki en busca de:
- Contradicciones entre páginas o con la normativa vigente.
- Afirmaciones sin página exacta o con `status: incierto` sin resolver.
- Páginas huérfanas: sin links entrantes desde `index.md` u otras páginas.
- Conceptos/entidades mencionados en el texto de una página pero sin página propia.
- Cross-references faltantes (fuente menciona un concepto que sí tiene página, pero no hay link).

Reportar hallazgos al usuario antes de corregir, salvo que pida corrección automática.

## Regla de incertidumbre

No inventar contenido. Si una fuente no aclara algo, o no permite identificar la página exacta de un dato, marcarlo explícitamente en la página (`status: incierto` en el front matter, y/o una nota inline `[INCIERTO: ...]` en el cuerpo) en vez de completar el hueco. Esto aplica con más rigor que en una wiki bibliográfica genérica, porque el contenido de este repositorio puede usarse directamente en comunicaciones, análisis o decisiones de trabajo reales en la ANSV.

## Evolución del schema

Este archivo se ajusta con el uso real. Si una convención no tiene sentido en la práctica, decirlo y se corrige acá mismo.
