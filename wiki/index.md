# Índice de la Wiki

Catálogo de todas las páginas. Ver `../CLAUDE.md` para el schema y los flujos de trabajo (INGEST/QUERY/LINT).

## Fuentes (`fuentes/`)

35 documentos relevados en la raíz del repo (30 PDF, incluido uno con extensión `.PDF` en mayúsculas, y 5 DOCX): **1 ingerido** (PR-06) y **34 pendientes de ingest**. La agrupación de las pendientes es solo por lo que indica el nombre de archivo — no implica haber leído el contenido (regla de incertidumbre, `CLAUDE.md`).

### Ingeridas (1)

- [Procedimiento de Asistencia Técnica DCI (ANSV-CPP-PR-06)](fuentes/ansv-pr-06-procedimiento-asistencia-tecnica.md) — procedimiento oficial que regula cómo la ANSV/DCI planifica, ejecuta y hace seguimiento a las asistencias técnicas territoriales; declara la transferencia de conocimiento como uno de sus tres criterios de calidad obligatorios. (ingerido)

### Pendientes de ingest (34)

Se procesarán de a una, en el orden que indique el usuario, siguiendo el flujo INGEST de `CLAUDE.md` (lectura completa con registro de página exacta, página de `fuentes/`, actualización de este índice y del log, pausa para confirmación).

#### Procedimientos y anexos del SGC-DCI (ANSV) — familia del PR-06 (5)

- `Anexo 1. Caracterización ANSV-CPP-CA-02.pdf`
- `Anexo 3. Definición, implementación y seguimiento a estrategias interinstitucionales.ANSV-CPP-PR-07.pdf`
- `ANEXO4~1.PDF` — nombre truncado estilo DOS 8.3; el título real se confirma al leer el contenido (no asumir que es "Anexo 4" del PR-06 sin verificar).
- `Anexo 5. Instrucciones para el registro de acta de reunión.pdf`
- `Anexo 6. Lineamientos para el cargue de evidencias.pdf`

#### Normativa nacional — leyes, decretos, CONPES, resoluciones (13)

- `Ley 1503 de 2011 Promueve formacion de habitos y comportamientos seguros en la via.pdf`
- `Ley_1310_de_2009 Unificacion normas sobre Agentes de transito y grupos control vial.pdf`
- `Ley_1383 de 2010 Reforma la ley 769 de 2002 CNT y dicta otras disposiciones.pdf`
- `Ley_1702_de_2013.pdf`
- `Ley_2251_de_2022.pdf Ley julian Esteban.pdf` — nombre de archivo con "pdf" duplicado en el medio; extensión real al final.
- `Ley_769 de 2002 Codigo Nacional de transito.pdf`
- `DECRETO787 de 2015 funciones ANSV.pdf`
- `Decreto 2851 de 2013 reglamenta articulos de la ley 1503 definiciones en seg vial.pdf`
- `COMPES  Asistencia tecnica 4091.pdf` — CONPES 4091 (política de asistencia técnica territorial); el repositorio hermano de innovación ya tiene una página de esta misma política ([referencia externa, no citable directamente aquí sin verificar que sea el mismo documento](#nota-sobre-el-repositorio-hermano)).
- `Resolucion_007_de_2023_MAI (1).pdf`
- `Resolucion_583_2023armonizacion PLSV con PNSV 2022 2031.pdf`
- `Plan estrategico de control  SIT Resolucion 10110_231205_123130.pdf`
- `resolucion_mintransporte_4548_2013 profesionalización Agentes de transito.pdf`

#### Plan 365 (7)

- `CIRCULAR CONJUNTA PLAN 365 ANSV_VF.pdf`
- `ANEXO TÉCNICO PLAN 365.pdf`
- `ANÁLISIS DE LOS REPORTES PRESENTADOS POR LOS ORGANISMOS DE TRÁNSITO PLAN 365.pdf`
- `OFICIO CONVOCATORIA SOCIALIZACIÓN 14-11-2025.docx`
- `OFICIO GOBERNADORES Y ALCALDES PLAN 365 E INSTANCIAS.docx`
- `circular externa 20244000000157  VIDEOS INFRACCIONES Mintransporte.pdf`
- `16032026 2.2.1 Estrategia de Asistencia...s entidades territoriales.pdf`

#### Planes y documentos técnicos de política / protocolos (5)

- `Documento técnico de soporte Mintransporte- PNSV 2022-2031.pdf`
- `PLAN 70D SECTOR TRANSPORTE.pdf`
- `140926 ANÁLISIS TÉCNICO DE LA SINIESTRALIDAD VIAL EN COLOMBIA (Mateus).pdf`
- `manual-metodologico operacion estadistica FPSV.pdf`
- `Protocolo_Practicas_Seguras_Motociclistas.pdf`

#### Correspondencia / oficios (4)

- `20254000114441_Oficio_ANSV_2024 Super y Procuraduría VR.pdf`
- `ORFEO_Oficio_ANSV_2024 (22) super y procuraduría.docx`
- `Solicita info 365 Oficio_ANSV_2024 (22) super y procuraduría.docx`
- `Respuesta a peticion congresista 20266600072782.docx`

## Conceptos (`conceptos/`)

Ninguna todavía — se crean durante el INGEST cuando un tema transversal se repite entre varias fuentes (ver `CLAUDE.md`). Candidatos previsibles a partir de la única fuente ingerida: "Asistencia técnica como mecanismo de transferencia de conocimiento", "Sistema Seguro", "Plan 365" — se confirman recién cuando haya evidencia real de cruce entre fuentes.

## Entidades (`entidades/`)

Ninguna todavía. Candidatas previsibles a partir de la única fuente ingerida: ANSV, Dirección de Coordinación Interinstitucional (DCI) — se crean cuando una entidad se repita entre varias fuentes.

## Síntesis (`sintesis/`)

Ninguna todavía — se crean cuando una respuesta de QUERY vale la pena conservar.

## Nota sobre el repositorio hermano

Este repositorio comparte parte de su corpus (documentos del sistema de gestión de calidad y protocolos operativos de la ANSV) con el repositorio `programaGradoInnovacion` (rama `claude/llm-wiki-setup-nht7xw`, carpeta `wiki/`), que trata un trabajo de grado distinto (innovación/gestión del conocimiento). Son dos trabajos de grado independientes: **no se debe traer contenido de la wiki de ese repositorio como fuente de este trabajo de grado** (viola la regla de "fuente exclusiva"); solo se usa como referencia de formato/organización, tal como se pidió al crear esta wiki.
