# Log

Registro cronológico, append-only. No editar entradas pasadas — solo agregar al final.

## [2026-09-21] setup | Creación de la wiki (Paso 0)

- Se creó la estructura `/wiki` (`fuentes/`, `conceptos/`, `entidades/`, `sintesis/`, `index.md`, `log.md`) y `CLAUDE.md` en la raíz, replicando y adaptando el formato de organización y análisis usado en el repositorio `programaGradoInnovacion` (rama `claude/llm-wiki-setup-nht7xw`, carpeta `wiki/`), a pedido explícito del usuario ("aplica el formato de organizacion y analisis de la informacion aplicado en el repo de innovacion del mismo github").
- El `CLAUDE.md` de este repo no es una copia literal: incorpora las reglas propias de este proyecto de grado (fuente exclusiva, citación exacta con número de página, APA 7, sin datos = decirlo, retroalimentación crítica activa) como requisitos obligatorios del flujo INGEST, más estrictos que en el repositorio de referencia.
- Se relevaron los 35 documentos de la raíz del repo (30 PDF + 5 DOCX) y se listaron en `index.md`, agrupados solo por lo que indica el nombre de archivo (procedimientos/anexos SGC-DCI, normativa nacional, Plan 365, planes/documentos técnicos, correspondencia). No se leyó el contenido completo de ningún documento en este paso, salvo el ya cubierto abajo.
- Se migró `procedimiento-asistencia-tecnica-pr06.md` (análisis ya existente en la raíz del repo, previo a esta wiki) a `wiki/fuentes/ansv-pr-06-procedimiento-asistencia-tecnica.md`, reorganizado bajo el schema de front matter y con `status: ingerido`. No se agregó contenido nuevo respecto al análisis original; se marcó como `[INCIERTO]` la falta de número de página exacto por cada dato, pendiente de una relectura dirigida a citación APA.
- El archivo `procedimiento-asistencia-tecnica-pr06.md` de la raíz se eliminó tras la migración (su contenido íntegro quedó preservado en `wiki/fuentes/`).
- El INGEST detallado de las 34 fuentes restantes queda pendiente, para procesarse **una por vez** según el flujo por defecto de `CLAUDE.md`, salvo que el usuario pida explícitamente un procesamiento en lote.

## [2026-09-21] ingest | ANSV-CPP-PR-07 (Anexo 3 — estrategias interinstitucionales)

- Por pedido del usuario ("Empieza con PR-07, CA-02 y los anexos del bundle PR-06"), se inició el INGEST del bundle documental del PR-06, comenzando por el PR-07.
- Se extrajo el texto completo del PDF (9 páginas) con `pypdf`, preservando la paginación original, y se creó `wiki/fuentes/ansv-pr-07-estrategias-interinstitucionales.md` con `status: ingerido` y cita de página exacta en cada dato.
- Hallazgo relevante: el PR-07 declara explícitamente al PR-06 como documento asociado (p. 9), pero el PR-06 no declara al PR-07 (su sección de documentos asociados dice "No aplica") — relación asimétrica documentada como incertidumbre en ambas páginas.
- Se actualizó la página del PR-06 con el link cruzado al PR-07 y se actualizó `index.md` (de 1 a 2 fuentes ingeridas, familia SGC-DCI de 5 a 4 pendientes).
- No se crearon páginas de concepto/entidad nuevas en este paso: DCI, ANSV, PNSV y los firmantes ya están cubiertos por el ingest del PR-06; se evalúa crear una página de concepto o entidad propia recién cuando haya evidencia de cruce con una tercera fuente.
- Pendiente: continuar con CA-02 (Anexo 1) y los demás anexos del bundle, de a uno, según lo acordado con el usuario.

## [2026-09-21] ingest | ANSV-CPP-CA-02 (Anexo 1 — Caracterización de proceso)

- Se extrajo el texto del PDF (3 páginas) con `pypdf` y, adicionalmente, se probó `pdfplumber` para extracción estructurada de tablas — ambas herramientas dieron una extracción de contenido correcta pero **sin mapeo confiable fila por fila** entre proveedor/entrada/actividad/salida/cliente, por el diseño de celdas combinadas del formato de caracterización. Se documentó esto como limitación metodológica explícita en la página, y se marcó `status: incierto` en vez de `ingerido` — es la primera fuente de este repo que no alcanza el estado pleno de ingest por una limitación de extracción, no de lectura.
- Sí se pudo extraer con confianza el ciclo PHVA completo (12 actividades: 4 Planear, 3 Hacer, 2 Verificar, 3 Actuar), con cita de página, porque esas celdas aparecen aisladas y sin ambigüedad en la extracción.
- Se creó `wiki/fuentes/ansv-ca-02-caracterizacion-proceso.md`.
- Hallazgos relevantes marcados como incertidumbre: (1) el cuerpo del documento nombra a la dependencia responsable como "Dirección de Coordinación Institucional" (sin "Inter"), mientras el resto del corpus usa "Dirección de Coordinación Interinstitucional"; (2) el patrón de firmantes difiere del PR-06/PR-07 (aparece un firmante nuevo, Cesar Mauricio Salcedo, e Ivana Carolina González Murcia cambia de rol de "elaboró" a "revisó").
- Se actualizaron los cross-links en las páginas del PR-06 y del PR-07, y se actualizó `index.md` (de 2 a 3 fuentes ingeridas — una de ellas con status incierto —, familia SGC-DCI de 4 a 3 pendientes).
- Pendiente: continuar con `ANEXO4~1.PDF`, luego Anexo 5 y Anexo 6, para cerrar el bundle del PR-06. Al cerrar el bundle completo se evaluará crear una página de concepto ("asistencia técnica como mecanismo de transferencia de conocimiento" o similar) y una página de entidad (DCI), dado que ya hay evidencia de cruce entre 3 fuentes.

## [2026-09-21] ingest | ANEXO4~1.PDF → identificado como ANSV-CPP-PR-08

- Se leyó el contenido completo del archivo de nombre truncado `ANEXO4~1.PDF` (9 páginas, `pypdf`) y se confirmó que es el **ANSV-CPP-PR-08** ("Procedimiento Articulación, Fortalecimiento y Participación en Instancias Territoriales de Seguridad Vial"), tal como advertía `index.md` que había que verificar antes de asumir. El `fuente_pdf` de la página se dejó como `ANEXO4~1.PDF` (nombre exacto en el repo), no como un nombre inferido.
- Se creó `wiki/fuentes/ansv-pr-08-articulacion-instancias-territoriales.md` con `status: ingerido` y cita de página exacta en cada dato.
- Hallazgo relevante: el PR-08 define explícitamente a la DCI citando al PR-06 y al PR-07 en su propio glosario (p. 2), y declara a ambos como "documentos asociados" (p. 9) — esto confirma, con una tercera fuente, el patrón asimétrico ya detectado: PR-07 y PR-08 referencian al PR-06, pero el PR-06 no referencia a ninguno de los dos.
- Se identificó normativa citada pero no disponible en este repositorio (Resolución 097 de 2019, Resolución 516 de 2022) y normativa sí disponible pero aún no ingerida (Ley 1702 de 2013).
- Se actualizaron los cross-links en PR-06, PR-07 y CA-02, y se actualizó `index.md` (de 3 a 4 fuentes ingeridas, familia SGC-DCI de 3 a 2 pendientes: quedan Anexo 5 y Anexo 6).
- Pendiente: continuar con Anexo 5 (instrucciones registro de acta de reunión) y Anexo 6 (lineamientos cargue de evidencias) para cerrar el bundle completo del PR-06.

## [2026-09-21] ingest | Anexo 5 — Formato Acta de Reunión (ANSV-GIP-FO-05)

- Se extrajo el texto completo del PDF (3 páginas) con `pypdf`. A diferencia de los cuatro documentos anteriores, este no es un procedimiento de la DCI (código "ANSV-CPP-...") sino una **plantilla transversal de la ANSV** del proceso Gestión Integral de Procesos (código "ANSV-GIP-FO-05"), reutilizada por la DCI para sus actas de asistencia técnica.
- Se creó `wiki/fuentes/ansv-gip-fo-05-formato-acta-reunion.md` con `status: ingerido` y cita de página exacta.
- Hallazgo relevante para el trabajo de grado: el formato exige explícitamente que el campo TEMA de toda acta de asistencia técnica se nombre siempre "Asistencia Técnica" seguido del enfoque (con ejemplos como "Asistencia Técnica – PLSV de Cartagena" y "Asistencia Técnica a Organismos de Tránsito"), y exige que cada compromiso adquirido tenga entregable, responsable y fecha para trazabilidad.
- Se identificó un formato relacionado citado pero no disponible en este repositorio: ANSV-GIP-FO-06 (registro de asistencia).
- Se actualizaron los cross-links en PR-06, PR-07, PR-08 y CA-02 (los cuatro usan "acta de reunión" como registro, aunque ninguno cita el código GIP-FO-05 explícitamente), y se actualizó `index.md` (de 4 a 5 fuentes ingeridas, familia SGC-DCI de 2 a 1 pendiente: queda solo el Anexo 6).
- Pendiente: cerrar el bundle con el Anexo 6 (lineamientos cargue de evidencias); luego evaluar con el usuario la síntesis de concepto/entidad de todo el bundle antes de continuar con el resto del repositorio.

## [2026-09-21] ingest | Anexo 6 — Lineamientos para el cargue de evidencias (cierre del bundle PR-06)

- Se extrajo el texto completo del PDF (3 páginas) con `pypdf`. A diferencia de los cinco documentos anteriores del bundle, este no tiene código, versión, fecha de vigencia ni sección de aprobación — parece ser un instructivo interno de la DCI, no un documento controlado del SIG/MIPG. Se marcó `status: incierto` por esta razón.
- Se creó `wiki/fuentes/dci-lineamientos-cargue-evidencias.md` con cita de página exacta.
- Hallazgo relevante: el documento refuerza y hace más estricta la regla de nomenclatura del Anexo 5 (campo TEMA = "Asistencia técnica" siempre), agregando la prohibición explícita de sinónimos ("mesa técnica", "reunión de seguimiento") y un formato de nomenclatura de archivo (fecha_tipo_documento_entidad territorial); también descalifica explícitamente los informes de comisión como evidencia válida de AT.
- Se identificó una nueva entidad no vista en las 5 fuentes anteriores: Oficina Asesora de Planeación (ANSV).
- Con esta fuente **se cierra el bundle documental completo del PR-06** solicitado por el usuario (PR-06, PR-07, CA-02, PR-08, Anexo 5, Anexo 6).

## [2026-09-21] sintesis | Conceptos y entidades del bundle PR-06

- Con el bundle completo (6 fuentes), se aplicó el mismo patrón de dos pasos usado en el repositorio de innovación de referencia: ingest fuente por fuente, seguido de una síntesis de concepto/entidad cuando ya hay evidencia real de cruce.
- Se creó `wiki/entidades/dci-direccion-coordinacion-interinstitucional.md`: rol de la DCI en cada uno de los 6 documentos, firmantes recurrentes (con sus variaciones de rol entre documentos) y entidades externas mencionadas (Dirección General, Gobernadores/Alcaldes, Oficina Asesora de Planeación).
- Se creó `wiki/conceptos/asistencia-tecnica-bundle-pr06.md`: arma la cadena documental completa (detección de necesidad territorial en CTSV/CLSV/CDSV → estrategia PR-07 → ejecución PR-06 → caracterización CA-02 → registro GIP-FO-05 → trazabilidad Anexo 6), la definición textualmente idéntica de "Asistencia Técnica" en PR-06 y PR-07, y un señalamiento crítico propio: ninguna de las 6 fuentes describe el protocolo desde la perspectiva del municipio/organismo de tránsito receptor — todas están escritas desde la perspectiva de la DCI como ejecutor. Se marcó explícitamente como observación propia, no como vacío confirmado del repositorio completo (quedan 29 fuentes sin ingerir).
- Se enlazaron ambas páginas nuevas desde las 6 páginas de fuente del bundle (sección "Ver también") y se actualizó `index.md` (secciones Conceptos y Entidades, antes vacías).
- Pendiente: definir con el usuario el orden de ingest de las 29 fuentes restantes (normativa nacional, Plan 365, planes/documentos técnicos, correspondencia).

## [2026-09-21] ingest | Ley 769 de 2002 — Código Nacional de Tránsito (primera de la normativa nacional)

- El usuario pidió continuar con el grupo "normativa nacional" (13 documentos). Se decidió empezar por la Ley 769 de 2002 (Código Nacional de Tránsito) por ser la norma base de la que derivan varias de las demás leyes/decretos de este grupo (1310/2009, 1383/2010 la reforman directamente).
- El documento tiene 54 páginas. Se leyó completo el Título I (Disposiciones Generales, arts. 1-8, p. 1-9) con cita de página exacta, por ser la sección que define autoridades y organismos de tránsito. El resto del código (normas de comportamiento y sanciones, ~45 páginas) se escaneó por estructura de títulos/capítulos y se buscaron menciones puntuales de "asistencia técnica" y "ANSV", sin lectura artículo por artículo — decisión de alcance documentada explícitamente en la página, dado que esas secciones son mayoritariamente ajenas al objeto de este trabajo de grado.
- Se creó `wiki/fuentes/ley-769-2002-codigo-nacional-transito.md`.
- Hallazgos relevantes: (1) el art. 6 (p. 7-8) da la **definición legal exacta de "organismo de tránsito"** — el destinatario de la propuesta de protocolo de esta tesis; (2) el art. 4, parágrafo 1° (p. 7) es el origen legal del Plan Nacional de Seguridad Vial; (3) el art. 7, parágrafo 3° (p. 8) y el art. 14, parágrafo 2° (p. 11-12) mencionan a la ANSV asistiendo técnicamente, pero acotado a instituciones de educación superior y currículos de formación de conductores — no a la asistencia técnica territorial amplia del PR-06. Se marcó como incertidumbre que el texto consolidado no identifica con precisión qué ley posterior a 2013 introdujo la mención de la ANSV en el art. 7.
- Se actualizó `index.md` (de 6 a 7 fuentes ingeridas; normativa nacional de 13 a 12 pendientes).
- Pendiente: continuar con el resto de la normativa nacional. Se sugiere seguir con Ley 1310 de 2009 y Ley 1383 de 2010 por ser reformas directas de esta Ley 769.

## [2026-09-21] ingest | Ley 1310 de 2009 (agentes de tránsito y transporte)

- Documento corto (4 páginas, 16 artículos), se leyó completo con cita de página exacta. Se creó `wiki/fuentes/ley-1310-2009-agentes-transito.md`.
- Confirma textualmente la anotación de reforma ya registrada en la Ley 769 de 2002: el art. 8 de esta ley (p. 2) modifica el inciso 1° del art. 4° de la Ley 769.
- Aporta definiciones propias de "organismo de tránsito y transporte", "autoridad de tránsito y transporte", "agente de tránsito y transporte" y crea la Comisión de Tránsito y Participación Ciudadana (arts. 11-13).
- Se identificó una entidad no vista antes en este repositorio: el Fondo de Prevención Vial (art. 13, p. 3), posible antecedente institucional previo a la ANSV.
- Se actualizaron los cross-links en la página de la Ley 769 y se actualizó `index.md` (de 7 a 8 fuentes ingeridas; normativa nacional de 12 a 11 pendientes).
- Pendiente: continuar con Ley 1383 de 2010 (siguiente reforma directa de la Ley 769).

## [2026-09-21] ingest | Ley 1383 de 2010 (reforma la Ley 769)

- Documento de 13 páginas, 28 artículos. Se revisó la estructura completa y se buscaron menciones de "asistencia técnica" y "seguridad vial" en todo el texto: no se encontró ninguna mención de asistencia técnica, y "seguridad vial" aparece una sola vez de forma tangencial (art. 50, condiciones del vehículo). Dado que el contenido es mayoritariamente ajeno al objeto de este trabajo de grado (licencias de conducción y régimen sancionatorio), se resumió por estructura sin transcribir artículo por artículo — decisión de alcance documentada explícitamente en la página, igual que con la Ley 769.
- Se confirmó que los arts. 1-3 de esta ley son la fuente original de la redacción de los arts. 1°, 3° y 5° de la Ley 769 ya citados en esa página (texto idéntico).
- Se creó `wiki/fuentes/ley-1383-2010-reforma-cnt.md` y se actualizó el cross-link en la página de la Ley 769.
- Se actualizó `index.md` (de 8 a 9 fuentes ingeridas; normativa nacional de 11 a 10 pendientes).
- Pendiente: continuar con el resto de la normativa nacional. Quedan Ley 1503/2011, Ley 1702/2013, Ley 2251/2022, Decreto 787/2015, Decreto 2851/2013, CONPES 4091, Resolución 007/2023, Resolución 583/2023, Plan estratégico SIT/Resolución 10110, y Resolución Mintransporte 4548/2013.

## [2026-09-21] ingest | Ley 1503 de 2011 (formación de hábitos y comportamientos seguros en la vía)

- Documento de 8 páginas, 25 artículos, leído completo con cita de página exacta (alta relevancia temática, sin necesidad de acotar alcance). Se creó `wiki/fuentes/ley-1503-2011-formacion-habitos-seguros.md`.
- Hallazgos relevantes: (1) obliga a las entidades territoriales a elaborar "mapas de siniestralidad vial" (art. 21), incluir seguridad vial en sus Planes de Desarrollo (art. 22) y rendir cuentas anuales (art. 23); (2) crea el Plan Estratégico de Seguridad Vial — PESV (art. 12) para entidades con flota >10 vehículos; (3) el art. 12A (adicionado en 2020) es la tercera base legal identificada en este repositorio de una función de coordinación de la ANSV, esta vez sobre PESV.
- Se identificó que casi todo el articulado está reglamentado por el Decreto 2851 de 2013, pendiente de ingest en este mismo repositorio — se decidió continuar por ese documento a continuación por ser su reglamentación directa.
- Se actualizó `index.md` (de 9 a 10 fuentes ingeridas; normativa nacional de 10 a 9 pendientes).
