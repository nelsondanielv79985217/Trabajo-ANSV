# Índice de la Wiki

Catálogo de todas las páginas. Ver `../CLAUDE.md` para el schema y los flujos de trabajo (INGEST/QUERY/LINT).

## Fuentes (`fuentes/`)

35 documentos relevados en la raíz del repo (30 PDF, incluido uno con extensión `.PDF` en mayúsculas, y 5 DOCX): **19 ingeridos** — bundle completo del PR-06 (6) + **las 13 fuentes de normativa nacional completas** (Ley 769/2002, Ley 1310/2009, Ley 1383/2010, Ley 1503/2011, Decreto 2851/2013, Ley 1702/2013, Decreto 787/2015, Ley 2251/2022, Resolución 007/2023, Resolución 583/2023, Resolución 10110/2023, Resolución 4548/2013, CONPES 4091) — y **16 pendientes de ingest**. La agrupación de las pendientes es solo por lo que indica el nombre de archivo — no implica haber leído el contenido (regla de incertidumbre, `CLAUDE.md`).

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
- [Ley 1702 de 2013 — Crea la Agencia Nacional de Seguridad Vial (ANSV)](fuentes/ley-1702-2013-creacion-ansv.md) — ley fundacional de la ANSV y, específicamente (art. 10), de la propia Dirección de Coordinación Interinstitucional (DCI); crea también el Consejo Territorial de Seguridad Vial (CTSV, art. 15.2) ya documentado operativamente en el PR-08. (ingerido)
- [Decreto 787 de 2015 — Funciones de la estructura interna de la ANSV](fuentes/decreto-787-2015-funciones-ansv.md) — da el listado legal completo de las 14 funciones de la DCI (art. 10), entre ellas "definir las obligaciones que en materia de seguridad vial le corresponden cumplir a los Organismos de Tránsito" — la base legal más precisa del corpus para el bundle PR-06. Documento escaneado, ingerido vía OCR (tesseract) — ver nota metodológica en la página. (ingerido)
- [Ley 2251 de 2022 — Sistema Seguro (Ley Julián Esteban)](fuentes/ley-2251-2022-sistema-seguro.md) — define formalmente el enfoque "Sistema Seguro" (art. 2) que el bundle PR-06 usa sin definir; asigna a la ANSV la potestad de determinar la obligatoriedad del Plan Local de Seguridad Vial para municipios no capitales (art. 14). (ingerido)
- [Resolución 007 de 2023 — Mesas de Articulación Interinstitucional (MAI)](fuentes/resolucion-007-2023-mai.md) — instancia de coordinación territorial de la "Línea Territorial" de la DCI, adicional al CTSV; identifica el Decreto 1430 de 2022 como norma de aprobación del PNSV 2022-2031; revela un cambio de Director(a) de la DCI entre 2023 y 2025. (ingerido)
- [Resolución 583 de 2023 — Criterios de obligatoriedad del PLSV y armonización con el PNSV](fuentes/resolucion-583-2023-armonizacion-plsv-pnsv.md) — cuatro criterios objetivos (categoría municipal, organismo de tránsito, índice de fatalidad, población) para determinar si un municipio no capital debe formular su PLSV; confirma que "gestión del conocimiento" es una de las 8 áreas de acción oficiales del PNSV 2022-2031 (Decreto 1430 del 29/07/2022). (ingerido)
- [Resolución 10110 de 2023 (Superintendencia de Transporte) — PECCIT](fuentes/resolucion-10110-2023-peccit.md) — crea el Plan Estratégico de Control al Cumplimiento del Marco Normativo en Transporte, obligatorio para organismos de tránsito, con reporte mensual de indicadores de control a la informalidad — una tercera carga de reporte paralela al PLSV/ANSV. (ingerido)
- [Resolución 4548 de 2013 (Ministerio de Transporte) — Formación de agentes de tránsito](fuentes/resolucion-4548-2013-formacion-agentes-transito.md) — pénsum académico de 8 ejes para agentes de tránsito; comparte definición textual de "seguridad vial" con el Decreto 2851/2013; aporta un tercer sentido de "asistencia técnica" en el corpus (agente de tránsito → conductor). (ingerido)
- [CONPES 4091 — Política para la Asistencia Técnica Territorial](fuentes/conpes-4091-asistencia-tecnica-territorial.md) — política nacional transversal de asistencia técnica territorial (DNP, 2022), sin ninguna mención al sector tránsito/transporte/seguridad vial (verificación de texto completo); aporta un marco teórico de gestión del conocimiento (capital humano/relacional/estructural) aplicable como herramienta analítica externa al bundle PR-06. **Con esta fuente se completan las 13 de la normativa nacional.** (ingerido)

### Pendientes de ingest (16)

Se procesarán de a una, en el orden que indique el usuario, siguiendo el flujo INGEST de `CLAUDE.md` (lectura completa con registro de página exacta, página de `fuentes/`, actualización de este índice y del log, pausa para confirmación).

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
