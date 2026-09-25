# CLAUDE.md — Schema de la LLM Wiki (Trabajo-ANSV)

Este archivo define cómo Claude debe mantener la wiki de este repositorio. Se ajusta con el uso: si algo acá no funciona en la práctica, se discute con el usuario y se corrige.

La estructura y convenciones de este archivo replican el schema ya validado en el repositorio `nelsondanielv79985217/programaGradoInnovacion` (rama `claude/llm-wiki-setup-nht7xw`, carpeta `/wiki`), adaptado al corpus y las reglas propias de este proyecto.

## Propósito

*(Reencuadrado 2026-09-25 — ver `log.md` para la nota de cambio.)* Este repo es la base documental de trabajo del usuario como servidor/contratista de la Dirección de Coordinación Interinstitucional (DCI) de la Agencia Nacional de Seguridad Vial (ANSV). **La wiki no es un insumo para una tesis**: es una base de conocimiento reutilizable para que agentes (Claude u otros) generen productos de asesoría en el trabajo diario del usuario en la ANSV — oficios, conceptos técnicos y jurídicos, protocolos, informes de seguimiento, respuestas a peticiones, insumos para toma de decisiones — con citación exacta y trazable a las fuentes normativas e institucionales reales del corpus, sin inventar ni extrapolar contenido. Las fuentes son normativa (leyes, decretos, resoluciones), procedimientos y anexos del sistema de gestión de calidad de la ANSV, protocolos operativos, documentos de planeación sectorial, correspondencia oficial, conceptos jurídicos y productos/entregables propios del trabajo del usuario en la ANSV. En vez de releer y re-derivar todo desde cero cada vez que se necesita algo de ellas, se mantiene una wiki en Markdown (`/wiki`) que acumula resúmenes, páginas de conceptos/entidades y un índice — así el trabajo de lectura y síntesis se conserva entre sesiones y queda disponible para cualquier agente que deba producir un entregable citando estas fuentes con precisión.

## Reglas del proyecto que gobiernan esta wiki (no negociables)

Estas reglas aplican al contenido de `/wiki`, precisamente porque los agentes que la usarán producirán documentos oficiales/técnicos donde una cita mal atribuida o un hallazgo inventado tiene consecuencias reales:

1. **Fuente exclusiva**: solo se usa información contenida en los archivos cargados a este repositorio. No se usa conocimiento general, memoria del modelo ni resultados de búsqueda externa como sustento, salvo pedido explícito del usuario para un propósito distinto (ej. contexto normativo público).
2. **Citación exacta**: toda página de `fuentes/` debe registrar, cuando el documento lo permita identificar, el apartado/sección y el número de página exacto de cada dato, cifra o afirmación relevante que luego pueda citarse en un producto de asesoría (oficio, concepto, informe). Si no se puede identificar la ubicación precisa, la página debe decirlo explícitamente en vez de aproximarla — esto habilita que la wiki sirva de insumo citable, no solo de resumen.
3. **Sin datos disponibles = decirlo**: si una fuente no aclara algo, se marca (`status: incierto` y/o nota `[INCIERTO: ...]`) en vez de completar el hueco.
4. **Sin alucinación/extrapolación**: ninguna página de la wiki puede afirmar algo que no esté respaldado por el contenido real del PDF/DOCX correspondiente.

## Arquitectura de 3 capas (no mezclar)

1. **Fuentes crudas** — los archivos que ya existen en la raíz del repo (PDF/DOCX). Son **inmutables**: se leen, nunca se editan ni se mueven sin pedido explícito del usuario.
2. **Wiki** (`/wiki`) — páginas `.md` generadas y mantenidas enteramente por Claude: resúmenes, páginas de entidades/conceptos, índice, log.
3. **Schema** (este archivo) — estructura, convenciones y flujo de trabajo. Se co-crea y ajusta con el usuario.

## Estructura de `/wiki`

```
/wiki
  index.md          # catálogo de todas las páginas, por categoría
  log.md             # log cronológico append-only
  fuentes/           # una página por fuente cruda (PDF/DOCX) — resumen + hallazgos + metadatos + ubicación citable
  conceptos/         # páginas hub de temas transversales que cruzan varias fuentes
  entidades/         # páginas de organismos, dependencias o autores/firmantes recurrentes
  sintesis/          # páginas de síntesis cruzada / respuestas de QUERY guardadas / borradores de marco teórico o de capítulos
```

Tipos de página:
- **fuente** — un documento del repo. Resume objeto/alcance, contenido clave, y qué conceptos/entidades toca, registrando página/sección de cada dato citable. Nunca reemplaza al documento original, es un resumen navegable con referencias exactas.
- **concepto** — un tema transversal (ej. "Asistencia Técnica como mecanismo de transferencia de conocimiento", "Sistema Seguro", "Gobernanza territorial en seguridad vial"). Agrega qué dice cada fuente sobre ese tema, con links a `fuentes/`.
- **entidad** — un organismo, dependencia (ej. DCI, ANSV, Mintransporte, organismos de tránsito territoriales) o persona firmante recurrente.
- **sintesis** — cruces entre conceptos/fuentes que valen la pena conservar (ej. respuestas de QUERY que el usuario decide guardar), o borradores de productos de asesoría (oficios, conceptos técnicos/jurídicos, informes) que se elaboran a partir de la wiki. Todo borrador generado acá debe seguir cumpliendo citación exacta y trazabilidad a la fuente.
- **metodo**: no aplica corpus metodológico propio todavía; se agrega si el usuario carga una referencia metodológica transversal (ej. un manual de investigación).

Una página de concepto/entidad se crea la primera vez que hace falta (durante un INGEST), no se prepoblán de antemano — evita inventar categorías antes de tener evidencia real de que se repiten.

## Convenciones de nombres

- Un archivo por página, ruta = `wiki/<carpeta>/<slug>.md`.
- Slug: ASCII kebab-case, sin tildes ni mayúsculas, derivado del título.
- No duplicar páginas: antes de crear una nueva página de concepto/entidad, buscar si ya existe una con el mismo tema.
- Links entre páginas: rutas relativas Markdown estándar, ej. `[Asistencia Técnica](../conceptos/asistencia-tecnica-como-mecanismo-de-transferencia.md)`.

## Front matter (obligatorio en toda página)

```yaml
---
title: "Título legible de la página"
type: fuente | concepto | entidad | sintesis | metodo
tags: [tag1, tag2]
fuente_pdf: "nombre-exacto-del-archivo.pdf"   # solo en type: fuente
status: pendiente-ingest | ingerido | incierto
last_updated: YYYY-MM-DD
---
```

## `index.md`

Catálogo de todas las páginas, agrupado por categoría temática. Cada fila: `- [Título](ruta) — resumen de una línea. (status)`. Se actualiza en cada INGEST/QUERY que agregue o modifique una página.

## `log.md`

Registro cronológico, **append-only** (nunca se edita retroactivamente, solo se agrega al final). Formato de entrada:

```
## [YYYY-MM-DD] tipo | Nombre de la fuente o tema
- qué se hizo
- páginas creadas/actualizadas
```

`tipo` ∈ `{setup, ingest, query, lint}`.

## Flujo INGEST

Se procesa **una fuente a la vez** — nunca todo el repo de una pasada, salvo pedido explícito del usuario para lote (como se documenta en `log.md` cuando ocurra). El usuario se queda involucrado revisando cada actualización antes de seguir con la próxima ("metodología Karpathy": un paso, revisar el resultado, recién ahí seguir con el próximo).

1. Leer la fuente completa (PDF vía skill `pdf`, o el `.docx` correspondiente).
2. Discutir los puntos clave con el usuario (objeto, alcance, hallazgos, relevancia para el trabajo de asesoría del usuario en la DCI/ANSV).
3. Escribir/actualizar la página de `fuentes/`, registrando página/sección exacta de cada dato citable. Puede tocar varias páginas: crear/actualizar conceptos y entidades relevantes con link a esta fuente.
4. Actualizar `index.md`.
5. Agregar entrada a `log.md` con prefijo `## [YYYY-MM-DD] ingest | <nombre de la fuente>`.
6. Pausar y esperar confirmación del usuario antes de pasar a la próxima fuente.

## Flujo QUERY

1. Buscar primero en `index.md`.
2. Entrar a las páginas relevantes (`fuentes/`, `conceptos/`, `entidades/`, `sintesis/`) y sintetizar con referencias explícitas (documento + página).
3. Si la respuesta vale la pena conservar, proponer guardarla como página nueva en `sintesis/` en vez de que se pierda en el chat.
4. Si el dato pedido no está en ninguna fuente ingerida, decirlo explícitamente ("esto no está en las fuentes del proyecto") en vez de completarlo.

## Flujo LINT

Cuando se pida, revisar la wiki en busca de:
- Contradicciones entre páginas.
- Afirmaciones desactualizadas (`status: incierto` sin resolver, o `last_updated` viejo vs. cambios recientes en fuentes).
- Páginas huérfanas: sin links entrantes desde `index.md` u otras páginas.
- Conceptos/entidades mencionados en el texto de una página pero sin página propia.
- Cross-references faltantes.
- Citas sin número de página cuando el documento sí lo permite identificar.

Reportar hallazgos al usuario antes de corregir, salvo que pida corrección automática.

## Regla de incertidumbre

No inventar contenido. Si una fuente no aclara algo, marcarlo explícitamente en la página (`status: incierto` en el front matter, y/o una nota inline `[INCIERTO: ...]` en el cuerpo) en vez de completar el hueco.

## Evolución del schema

Este archivo se ajusta con el uso real. Si una convención no tiene sentido en la práctica, decirlo y se corrige acá mismo.
