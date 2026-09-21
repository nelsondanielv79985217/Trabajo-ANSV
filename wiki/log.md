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
