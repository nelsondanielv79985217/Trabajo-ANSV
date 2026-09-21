# Índice de la Wiki

Catálogo de todas las páginas. Ver `../CLAUDE.md` para el schema y los flujos de trabajo (INGEST/QUERY/LINT).

## Fuentes (`fuentes/`)

35 documentos relevados en la raíz del repo (30 PDF, incluido uno con extensión `.PDF` en mayúsculas, y 5 DOCX): **11 ingeridos** — bundle completo del PR-06 (6) + Ley 769/2002, Ley 1310/2009, Ley 1383/2010, Ley 1503/2011 y Decreto 2851/2013 (5 de la normativa nacional) — y **24 pendientes de ingest**. La agrupación de las pendientes es solo por lo que indica el nombre de archivo — no implica haber leído el contenido (regla de incertidumbre, `CLAUDE.md`).

### Ingeridas (6) — bundle PR-06 completo

- [Procedimiento de Asistencia Técnica DCI (ANSV-CPP-PR-06)](fuentes/ansv-pr-06-procedimiento-asistencia-tecnica.md) — procedimiento oficial que regula cómo la ANSV/DCI planifica, ejecuta y hace seguimiento a las asistencias técnicas territoriales; declara la transferencia de conocimiento como uno de sus tres criterios de calidad obligatorios. (ingerido)
- [Procedimiento Definición, Implementación y Seguimiento a Estrategias Interinstitucionales (ANSV-CPP-PR-07)](fuentes/ansv-pr-07-estrategias-interinstitucionales.md) — procedimiento previo/superior al PR-06: define y aprueba la estrategia interinstitucional (12 actividades, aprobación por Dirección General) que luego se ejecuta en territorio mediante el PR-06. (ingerido)
- [Formato Caracterización de Proceso (ANSV-CPP-CA-02)](fuentes/ansv-ca-02-caracterizacion-proceso.md) — caracterización del proceso "Coordinación y Articulación..." del que el PR-06 y el PR-07 son procedimientos operativos; ciclo PHVA de 12 actividades. (incierto — la tabla de proveedores/entradas/salidas no pudo extraerse con mapeo confiable fila por fila, ver nota metodológica en la página)
- [Procedimiento Articulación, Fortalecimiento y Participación en Instancias Territoriales de Seguridad Vial (ANSV-CPP-PR-08)](fuentes/ansv-pr-08-articulacion-instancias-territoriales.md) — el archivo `ANEXO4~1.PDF` identificado durante el ingest; define cómo una necesidad detectada en un Consejo/Comité Territorial de Seguridad Vial (CTSV/CLSV/CDSV) llega a la DCI y activa el PR-06 y/o el PR-07. (ingerido)
- [Formato Acta de Reunión (ANSV-GIP-FO-05)](fuentes/ansv-gip-fo-05-formato-acta-reunion.md) — plantilla transversal de la ANSV (no propia de la DCI) para registrar actas; exige nombrar toda actividad de asistencia técnica con el rótulo "Asistencia Técnica" en el campo TEMA. (ingerido)
- [Lineamientos para el Cargue de Evidencias — DCI](fuentes/dci-lineamientos-cargue-evidencias.md) — instructivo de nomenclatura de archivos, periodicidad mensual y prohibición de informes de comisión como evidencia de AT. (incierto — el documento no tiene código, versión ni sección de aprobación, no se puede confirmar su estatus documental formal)

### Ingeridas — normativa nacional (3 de 13)

- [Ley 769 de 2002 — Código Nacional de Tránsito Terrestre](fuentes/ley-769-2002-codigo-nacional-transito.md) — define legalmente "organismo de tránsito" (art. 6) y "autoridades de tránsito" (art. 3); origen legal del Plan Nacional de Seguridad Vial (art. 4) y menciones puntuales de asistencia técnica de la ANSV (arts. 7 y 14, en su redacción reformada). Lectura completa del Título I; el resto del código (normas de comportamiento y sanciones) se escaneó por estructura, no artículo por artículo — ver nota de alcance en la página. (ingerido)
- [Ley 1310 de 2009 — Unificación de normas sobre agentes de tránsito y grupos de control vial](fuentes/ley-1310-2009-agentes-transito.md) — define "organismo de tránsito y transporte", "autoridad de tránsito y transporte" y "agente de tránsito y transporte"; crea la Comisión de Tránsito y Participación Ciudadana; modifica directamente el art. 4 de la Ley 769. (ingerido)
- [Ley 1383 de 2010 — Reforma la Ley 769 de 2002](fuentes/ley-1383-2010-reforma-cnt.md) — reforma licencias de conducción y régimen sancionatorio; sin contenido sustantivo sobre asistencia técnica. Resumida por estructura, no artículo por artículo — ver nota de alcance en la página. (ingerido)
- [Ley 1503 de 2011 — Formación de hábitos y comportamientos seguros en la vía](fuentes/ley-1503-2011-formacion-habitos-seguros.md) — obliga a las entidades territoriales a elaborar mapas de siniestralidad vial, incluir seguridad vial en sus Planes de Desarrollo y rendir cuentas anuales; crea el Plan Estratégico de Seguridad Vial (PESV); tercera base legal de una función de coordinación de la ANSV (art. 12A). (ingerido)
- [Decreto 2851 de 2013 — Reglamenta artículos de la Ley 1503](fuentes/decreto-2851-2013-reglamenta-ley-1503.md) — asigna a los organismos de tránsito la función de revisar, avalar y controlar los PESV registrados en su jurisdicción (art. 11); listado más amplio del corpus de entidades del sistema de seguridad vial (art. 14, Portal de la Seguridad Vial). (ingerido)

### Pendientes de ingest (24)

Se procesarán de a una, en el orden que indique el usuario, siguiendo el flujo INGEST de `CLAUDE.md` (lectura completa con registro de página exacta, página de `fuentes/`, actualización de este índice y del log, pausa para confirmación).

#### Normativa nacional — leyes, decretos, CONPES, resoluciones (8 restantes de 13)

- `Ley_1702_de_2013.pdf`
- `Ley_2251_de_2022.pdf Ley julian Esteban.pdf` — nombre de archivo con "pdf" duplicado en el medio; extensión real al final.
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

- [Asistencia Técnica de la DCI — Marco documental completo (bundle PR-06)](conceptos/asistencia-tecnica-bundle-pr06.md) — arma la cadena documental completa (detección de necesidad territorial → estrategia → ejecución de AT → caracterización de proceso → registro → trazabilidad) a partir de las 6 fuentes del bundle PR-06 ya ingeridas. (ingerido)

Candidatos previsibles para próximas páginas, aún sin crear porque no hay evidencia de cruce con una tercera fuente ajena al bundle: "Sistema Seguro", "Plan 365", "Instancias territoriales de seguridad vial (CTSV/CLSV/CDSV)".

## Entidades (`entidades/`)

- [Dirección de Coordinación Interinstitucional (DCI) — ANSV](entidades/dci-direccion-coordinacion-interinstitucional.md) — dependencia responsable de las 6 fuentes del bundle PR-06; rol en cada documento, firmantes recurrentes y entidades externas con las que se relaciona. (ingerido)

Candidata previsible para próxima página: Agencia Nacional de Seguridad Vial (ANSV) como entidad propia (distinta de la DCI) — aún sin crear porque, hasta ahora, todo lo ingerido es específicamente de la DCI.

## Síntesis (`sintesis/`)

Ninguna todavía — se crean cuando una respuesta de QUERY vale la pena conservar.

## Nota sobre el repositorio hermano

Este repositorio comparte parte de su corpus (documentos del sistema de gestión de calidad y protocolos operativos de la ANSV) con el repositorio `programaGradoInnovacion` (rama `claude/llm-wiki-setup-nht7xw`, carpeta `wiki/`), que trata un trabajo de grado distinto (innovación/gestión del conocimiento). Son dos trabajos de grado independientes: **no se debe traer contenido de la wiki de ese repositorio como fuente de este trabajo de grado** (viola la regla de "fuente exclusiva"); solo se usa como referencia de formato/organización, tal como se pidió al crear esta wiki.
