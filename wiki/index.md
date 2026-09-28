# Índice de la Wiki

Catálogo de todas las páginas. Ver `../CLAUDE.md` para el schema y los flujos de trabajo (INGEST/QUERY/LINT).

**Estado general (2026-09-28):** La wiki se migró de la rama `Contractual-OPS` a la rama `main` (ver `log.md`, entrada de migración) — desde ahora todo el trabajo continúa en `main`. **51 fuentes ingeridas** (las 45 migradas de `Contractual-OPS`, con categorías originales completas, más 6 de las 100 fuentes nuevas: la Circular 20234000000677/Ley 2197-2022, la Ley 336/1996, la Ley 2294/2023 y el Decreto 2106/2019) — de las 45 originales, 2 páginas (Concepto de Estabilidad Ocupacional Reforzada y su Solicitud DIV) referencian un `fuente_pdf` que no está presente en `main` (ver incertidumbre en `log.md`). **94 fuentes nuevas pendientes de ingest**, cargadas directamente por el usuario en `main` y relevadas por nombre de archivo en las secciones nuevas más abajo. Total del corpus: 145 fuentes. 3 entidades y 5 conceptos creados hasta ahora. *Nota (2026-09-25, heredada de `Contractual-OPS`): la wiki no se construye como insumo de tesis, sino como base de conocimiento para agentes de asesoría del usuario en la DCI/ANSV.* *Nota: el usuario pidió continuar el INGEST sin pausar a pedir autorización entre cada fuente — se mantiene para las fuentes nuevas.*

## Fuentes (`fuentes/`)

### Procedimientos y anexos del sistema de gestión — ANSV / DCI (6, 6 ingeridas — completo)

- [ANSV-CPP-PR-06 — Procedimiento de Asistencia Técnica (DCI)](fuentes/ansv-pr-06-procedimiento-asistencia-tecnica.md) — Procedimiento vigente que regula cómo la DCI planifica, ejecuta y hace seguimiento a las asistencias técnicas territoriales; uno de los mecanismos posibles para implementar una estrategia interinstitucional definida bajo PR-07. (incierto — falta citación por página)
- [Anexo 1 — ANSV-CPP-CA-02, Caracterización del proceso](fuentes/ansv-ca-02-caracterizacion-anexo1.md) — Caracteriza el proceso misional "Coordinación y Articulación..." del cual PR-06 es solo la actividad de AT dentro del ciclo Hacer (PHVA). (ingerido)
- [Anexo 3 — ANSV-CPP-PR-07, Estrategias interinstitucionales](fuentes/ansv-pr-07-estrategias-interinstitucionales.md) — Define cómo la DCI formula, aprueba, implementa y da seguimiento a cualquier estrategia interinstitucional; nombra a la AT (PR-06) como una vía de implementación entre otras. (ingerido)
- [Anexo 4 — ANSV-CPP-PR-08, Instancias territoriales](fuentes/ansv-pr-08-instancias-territoriales.md) — Regula la articulación con Consejos Territoriales (CTSV) y Comités Locales/Departamentales de Seguridad Vial (CLSV/CDSV); puerta de entrada territorial de necesidades hacia PR-07 y PR-06. Archivo con nombre truncado en el repositorio (`ANEXO4~1.PDF`), contenido real confirmado al abrirlo. (ingerido)
- [Anexo 5 — ANSV-GIP-FO-05, Formato acta de reunión](fuentes/ansv-gip-fo-05-formato-acta-reunion.md) — Plantilla instructiva del registro de reuniones exigido por PR-06/PR-07/PR-08; su campo TEMA obliga a nombrar toda actividad registrada como "Asistencia Técnica", sin distinguir modalidades. Pertenece al Proceso Gestión Integral de Procesos (GIP), no al proceso de la DCI. (ingerido)
- [Anexo 6 — Lineamientos para el cargue de evidencias](fuentes/ansv-dci-lineamientos-cargue-evidencias.md) — Instructivo interno de la DCI (sin código ni aprobación SIG) que endurece la obligación de nombrar todo como "Asistencia Técnica"; aporta el único ejemplo real del corpus (ACTA No. 4, Ajuste PDSV). (ingerido)

### Marco normativo — leyes, decretos, resoluciones (11, 11 ingeridas — completo)

- [Ley 1702 de 2013 — Creación de la ANSV](fuentes/ley-1702-de-2013-creacion-ansv.md) — Ley fundacional de la ANSV; crea sus 7 dependencias estatutarias (incluida la DCI), el Consejo Directivo, el Fondo Nacional de Seguridad Vial y el Consejo Territorial de Seguridad Vial (base legal de los CTSV que cita PR-08). (ingerido)
- [Decreto 787 de 2015 — Funciones de la estructura interna](fuentes/decreto-787-de-2015-funciones-ansv.md) — Reglamenta la Ley 1702/2013; desarrolla las 14 funciones estatutarias de la DCI (Art. 10). Hallazgo: la "asistencia técnica" no aparece nombrada como tal en el decreto — es una figura operativa posterior de PR-06, no de rango legal/reglamentario. (ingerido)
- [Decreto 2851 de 2013 — Reglamenta la Ley 1503/2011 (educación vial, PESV, alcohol)](fuentes/decreto-2851-de-2013-educacion-vial-pesv.md) — Anterior en 3 semanas a la Ley 1702/2013 (no menciona ANSV/DCI). Define el Plan Estratégico de Seguridad Vial (PESV), instrumento distinto y anterior a la AT de la DCI; segundo uso del término "asistencia técnica" en el corpus (Mineducación, educación vial escolar). (ingerido)
- [Ley 1503 de 2011 — Hábitos y comportamientos seguros en la vía](fuentes/ley-1503-de-2011-habitos-comportamientos-seguros.md) — Ley madre reglamentada por el Decreto 2851/2013; crea el PESV (Art. 12) y, en su Art. 12A (adicionado en 2020), es la tercera fuente legal que atribuye competencias a la ANSV. Hallazgo: el régimen de aval del PESV descrito por el Decreto 2851/2013 podría estar tácitamente derogado desde 2019 (Decreto 2106/2019, no incluido en el corpus). (ingerido)
- [Ley 769 de 2002 — Código Nacional de Tránsito Terrestre](fuentes/ley-769-de-2002-codigo-nacional-transito.md) — Ley general del tránsito; base de casi todas las demás fuentes del corpus. Hallazgo central: el término "asistencia técnica" aparece ya en su redacción original de 2002 (Art. 7°), once años antes de la ANSV — ver [genealogía del término](conceptos/genealogia-asistencia-tecnica.md). Documenta 5 competencias de la ANSV insertadas por reformas posteriores (formación de conductores, velocidad, fotomultas) y el origen 2002 del mandato de Plan Nacional de Seguridad Vial. (ingerido)
- [Ley 1383 de 2010 — Reforma el Código Nacional de Tránsito](fuentes/ley-1383-de-2010-reforma-codigo-nacional-transito.md) — Reforma puntual de 28 artículos del Código (licencias, revisión técnico-mecánica, sanciones). Anterior en tres años a la ANSV; no la menciona. Confirma con texto primario dos citas ya registradas en la Ley 769/2002 (Arts. 3° y 122); no toca el Art. 7° (evidencia adicional del origen 2002 de "asistencia técnica"). Hallazgo abierto: en 2010 las multas del Art. 131 tenían 5 categorías (A–E), no 6 (A–F) como el texto consolidado actual. (ingerido)
- [Ley 2251 de 2022 — Política de seguridad vial con enfoque de Sistema Seguro (Ley Julián Esteban)](fuentes/ley-2251-de-2022-sistema-seguro.md) — Introduce el paradigma de "Sistema Seguro" para la política de seguridad vial; fuente más densa del corpus en competencias ANSV (10 competencias: armonización regulatoria vehicular, velocidad, planes locales de seguridad vial, fotomultas, SIRAS). Confirma 3 citas ya registradas en la Ley 769/2002 (Arts. 106, 107, 158A). Descarta la hipótesis de que esta ley hubiera ampliado a 6 las categorías de multas del Art. 131. (ingerido)
- [Resolución 583 de 2023 — Armonización PLSV con PNSV 2022-2031](fuentes/resolucion-583-de-2023-armonizacion-plsv-pnsv.md) — Primera fuente del corpus expedida directamente por la ANSV (Directora General). Reglamenta el Par. 1 del Art. 14 de la Ley 2251/2022: criterios de obligatoriedad de Planes Locales de Seguridad Vial para municipios/distritos según categorización e índice de fatalidad. Cita indirectamente el Decreto 1430/2022 (PNSV 2022-2031, no incluido en el corpus) y sus 8 áreas de acción del Sistema Seguro (incluida "gobernanza"). Confirma 3 citas ya registradas (Ley 769/2002 Art. 4° Par. 1; Ley 1702/2013 Arts. 2° y 5°). (ingerido)
- [Resolución 007 de 2023 — Reglamenta las Mesas de Articulación Interinstitucional (MAI)](fuentes/resolucion-007-de-2023-mesas-articulacion-interinstitucional.md) — Acto propio de la ANSV que reglamenta un instrumento de coordinación territorial liderado por la Línea Territorial de la DCI, no documentado en PR-06/PR-07/PR-08. Hallazgo central: cita el PNSV 2022-2031 vinculando expresamente "asistencia técnica" con entidades territoriales — primer eslabón normativo entre Sistema Seguro y AT territorial. Revela estructura interna de la DCI (líneas territorial/sectorial, Enlaces Territoriales) y aporta datos para fijar la secuencia de Directores de la DCI. (ingerido)
- [Ley 1310 de 2009 — Unificación de normas sobre agentes de tránsito](fuentes/ley-1310-de-2009-agentes-transito.md) — Profesionaliza y jerarquiza a los agentes de tránsito territoriales; define "Organismo de Tránsito y Transporte", "Agente de Tránsito y Transporte" y "Grupo de Control Vial" (complementa la Ley 769/2002). Fija el perfil profesional exigible al Director de Organismo de Tránsito (modifica Art. 4° CNT) — relevante para caracterizar al interlocutor territorial del protocolo de AT. Anterior en 4 años a la ANSV; no la menciona. (ingerido)
- [Resolución 4548 de 2013 — Profesionalización de Agentes de Tránsito](fuentes/resolucion-4548-de-2013-profesionalizacion-agentes-transito.md) — Mintransporte reglamenta el Art. 3° y numeral 5 del Art. 7° de la Ley 1310/2009: fija el contenido curricular (8 ejes) y el nivel educativo mínimo exigible a cada grado de agente de tránsito. Hallazgo: nuevo uso de "asistencia técnica", dirigido a conductores individuales (no a instituciones), dentro del eje "Ejercicio de la autoridad de tránsito". Documenta una demanda de nulidad activa contra su Art. 2° ante el Consejo de Estado. (ingerido)

### Planeación sectorial y política pública (6, 6 ingeridas — completo)

- [CONPES 4091 de 2022 — Política para la Asistencia Técnica Territorial](fuentes/conpes-4091-de-2022-politica-asistencia-tecnica-territorial.md) — Política nacional de mayor jerarquía sobre AT en Colombia (DNP + DAFP + Min. Hacienda + APC-Colombia + ESAP); define formalmente AT y ATT, diagnostica 4 problemas estructurales (descoordinación, desarticulación técnica, débil seguimiento/evaluación, débil gestión de conocimiento) y crea una política 2022-2026 con presupuesto ($6.015 millones). Hallazgo central: **no menciona a la ANSV ni a la DCI en ningún punto**. (ingerido)
- [PNSV 2022-2031 — Documento técnico de soporte](fuentes/pnsv-2022-2031-documento-tecnico-soporte.md) — Fuente más extensa del corpus (214 páginas). Plan vigente de la ANSV (Decreto 1430/2022); confirma con texto primario las MAI, el enfoque de Sistema Seguro y sus 8 áreas de acción. Hallazgo central: **indicadores oficiales que miden "asistencia técnica" con metas a 2031** (p. ej. "Municipios asistidos técnicamente en Sistema Seguro", 24 %→41 %). Autocrítica institucional (86,7 % de entidades con dificultades de cumplimiento 2011-2021). Resuelve la incertidumbre sobre la derogatoria del aval del PESV (Decreto 2106/2019). (ingerido)
- [Plan 70D — Sector Transporte](fuentes/plan-70d-sector-transporte.md) — Plan operativo interinstitucional de 70 días (31 oct 2024-10 ene 2025) de todo el Sector Transporte (ANSV, Mintransporte, SuperTransporte, ANI, INVÍAS, DITRA). Hallazgo: nueva mención de "asistencia técnica a las autoridades" como componente de un plan operativo real y reciente. Aporta cifras de siniestralidad, despliegue territorial (543 ciudades, 78 personas en territorio) y primera mención de cooperación internacional activa (Bloomberg Philanthropies, Vital Strategies). (ingerido)
- [Resolución 10110 de 2023 — PECCIT/SISI (SuperTransporte)](fuentes/resolucion-10110-de-2023-peccit-supertransporte.md) — Acto de la Superintendencia de Transporte (no de la ANSV/DCI) que crea el Plan Estratégico de Control al Cumplimiento del Marco Normativo en Transporte y su sistema digital de reporte (SISI/PECCIT), dirigido a los mismos organismos de tránsito/municipios con los que trabaja la DCI. Aporta cita nueva de la Ley 769/2002 (Art. 3° Par. 3°, facultad de SuperTransporte) y documenta una carga de reporte periódico preexistente en el interlocutor territorial del protocolo de AT. (ingerido)
- [Manual Metodológico EFSV (ONSV)](fuentes/manual-metodologico-efsv-onsv.md) — Manual metodológico oficial de la operación estadística de fallecidos por siniestros viales (ONSV, 2021), fuente primaria de las cifras de siniestralidad citadas en el resto del corpus. Confirma, con origen institucional preciso (2019), la cooperación de la ANSV con Bloomberg Philanthropies y Vital Strategies. No menciona a la DCI ni "asistencia técnica". (ingerido)
- [Anexo Técnico Plan 365 (Circular Conjunta 023/2025)](fuentes/anexo-tecnico-plan-365.md) — Instrumento complementario del Plan 70D, de cobertura anual: prioriza 2.307 combinaciones festivo-municipio para 2025 según siniestralidad histórica (8.271 fallecidos nacionales en 2024). Reutiliza la "gráfica de la ballena" del Plan 70D. Hallazgo: no usa el término "asistencia técnica" (usa "presencia institucional") — evidencia de inconsistencia terminológica dentro de la misma familia de instrumentos. (ingerido)

### Protocolos operativos y Plan 365 (4, 4 ingeridas — completo)

- [Protocolo de Prácticas Seguras para Motociclistas](fuentes/protocolo-practicas-seguras-motociclistas.md) — Protocolo conjunto Ministerio de Trabajo–ANSV (Dirección de Comportamiento, no DCI) para empleadores/trabajadores que usan motocicleta como herramienta de trabajo. Confirma la Resolución 40595/2022 como metodología PESV vigente. No menciona a la DCI ni "asistencia técnica". (ingerido)
- [Circular Conjunta No. 023 de 2025 — Plan 365](fuentes/circular-conjunta-023-2025-plan-365.md) — Documento matriz del Plan 365 (Mintransporte, ANSV, SuperTransporte, DITRA). Usa expresamente "asistencia técnica" (corrige la lectura inicial del Anexo Técnico Plan 365). Resuelve tres incertidumbres de nombres del Plan 70D (Luis Yair Aguilar Rojas —DCI—, Darlyn Dávila —ONSV—, William Vallejo —Infraestructura y Vehículos—) y confirma continuidad de Mariantonia Tabares Pulgarín como Directora General hasta marzo de 2025. Hallazgo: contiene errores de cita normativa en su propio marco normativo (Ley 1702 "de 2003", Decreto "143"/2022, Ley 1310 "de 2014"). (ingerido)
- [Análisis de los Reportes Presentados por los Organismos de Tránsito — Plan 365](fuentes/analisis-reportes-organismos-transito-plan-365.md) — **Producto propio de la DCI** (noviembre de 2025, Andrés Alfonso González). Hallazgo central: 44 % de los 625 municipios priorizados por el Plan 365 no reportó ninguna acción durante 2025; de esos, 39 % aumentó su siniestralidad. Fuente muy reciente y de uso directo para informes de gestión. (ingerido)
- [Circular Externa 157 de 2024 — Videos como prueba de infracciones](fuentes/circular-externa-157-2024-videos-infracciones.md) — Mintransporte (Dirección de Transporte y Tránsito, no ANSV/DCI) instruye a organismos de tránsito sobre procesar videos de infracciones difundidos en redes/medios como prueba, incluso sin sistemas automáticos de detección. No menciona a la ANSV ni a la DCI. (ingerido)

### Correspondencia oficial / oficios (7, 7 ingeridas — completo)

- [Oficio ANSV 20254000114441 de 2025 — Vigilancia especial SuperTransporte/Procuraduría, Plan 365](fuentes/oficio-20254000114441-supertransporte-plan-365.md) — Escalamiento formal de la DCI ante SuperTransporte (con copia a la Procuraduría) por el 44 % de incumplimiento de reporte del Plan 365. Aporta cita nueva (Ley 1702/2013, Art. 19 num. 11; Ley 336/1996, Art. 46 lit. c) y confirma con fecha exacta (10 nov. 2025) a Paula Katerine Ramos Navarro como Directora de la DCI. (ingerido)
- [Oficio (plantilla) — Convocatoria socialización 14-11-2025](fuentes/oficio-convocatoria-socializacion-14-11-2025.md) — Plantilla (sin radicar) de convocatoria nacional a la jornada de socialización del Plan 365 del 21 de noviembre de 2025; confirma nuevamente a Ramos Navarro como Directora de la DCI y un nuevo uso de "asistencia técnica a los territorios". (ingerido)
- [Oficio (plantilla) — Gobernadores y Alcaldes: Plan 365 e Instancias](fuentes/oficio-gobernadores-alcaldes-plan-365-instancias.md) — Reitera a gobernadores y alcaldes la obligación de conformar/activar CLSV, CDSV y CTSV, en armonía con el Plan 365; aporta contenido parcial nuevo sobre la Resolución 516/2022 y menciona el "equipo de Regionalización" de la DCI. (ingerido)
- [ORFEO_Oficio_ANSV_2024 (22) — Plantilla del oficio SuperTransporte/Procuraduría](fuentes/orfeo-oficio-22-super-procuraduria.md) — Plantilla/borrador del mismo oficio ya ingerido (20254000114441/2025); aporta texto verbatim completo de la Ley 1702/2013 Art. 19 num. 11 y de la Ley 336/1996 Art. 46 lit. c. (ingerido)
- [Solicita info 365 Oficio (22) — Tercera versión del oficio SuperTransporte/Procuraduría](fuentes/solicita-info-365-oficio-22-super-procuraduria.md) — Tercera versión del mismo oficio; aporta cita verbatim con encabezado del Art. 19 y rango sancionatorio completo del Art. 46, y revela el framing probatorio-sancionatorio explícito del informe de incumplimiento. (ingerido)
- [Respuesta a petición congresista 20266600072782](fuentes/respuesta-peticion-congresista-20266600072782.md) — Borrador (corte sept. 2026) de respuesta a un debate de control político del Senado sobre siniestralidad, avance del PNSV (55 %) y presupuesto; confirma que "asistencia técnica" es práctica transversal a 4 direcciones de la ANSV ($149.175 millones, 2022-2026) y revela que las preguntas asignadas a la DCI quedan sin responder. (ingerido)
- [Estrategia de Asistencia Técnica y Pedagógica — Acción 2.2.1](fuentes/estrategia-asistencia-tecnica-pedagogica-sistema-seguro.md) — Documento estratégico propio de la DCI (PNSV, Gobernanza) que define sus dos líneas de asistencia técnica territorial y confirma su responsabilidad directa sobre el indicador oficial "Municipios asistidos técnicamente en Sistema Seguro", con metas anuales completas 2022-2031. (ingerido)

### Conceptos jurídicos y laborales (2, 2 ingeridas — completo)

`[INCIERTO]` Los dos archivos fuente de esta categoría (`20266700034703 Concepto Estabilidad Laboral Reforzada 07092026.pdf` y `Solicitud concepto estabilidad ocupacional (1).pdf`) no están presentes en la rama `main` — se leyeron y documentaron en `Contractual-OPS`; el contenido de las páginas sigue siendo válido y trazable, pero el archivo referenciado en `fuente_pdf` no puede reabrirse desde esta rama.

- [Concepto de Estabilidad Ocupacional Reforzada (2026)](fuentes/concepto-estabilidad-ocupacional-reforzada-2026.md) — Pronunciamiento del Grupo de Gestión Contractual sobre estabilidad ocupacional reforzada de contratistas (salud, prepensión, maternidad/lactancia, paternidad), con citación completa de jurisprudencia y conceptos CCE. Hallazgo: nueva Directora General de la ANSV (Alexandra Acelas Rodríguez, sept. 2026). (ingerido)
- [Solicitud de concepto — estabilidad ocupacional (DIV)](fuentes/solicitud-concepto-estabilidad-ocupacional-div.md) — Solicitud de la Dirección de Infraestructura y Vehículos sobre tres casos de estabilidad ocupacional reforzada; trámite distinto al concepto anterior pese al mismo tema. (ingerido)

### Contratación (1, 1 ingerida — completo)

- [Manual Unificado de Contratación ANSV (ANSV-CON-MG-01, V4)](fuentes/manual-unificado-contratacion-ansv.md) — Regula el proceso de gestión contractual de la ANSV (régimen público) y el Fondo Nacional de Seguridad Vial (régimen privado, vía fiducia); competencias, comité de contratación, modalidades de selección y cuantías, supervisión, régimen sancionatorio y liquidación. Instrumento genérico, sin mención específica a la DCI. (ingerido)

### Financiamiento y cooperación (4, 4 ingeridas — completo)

- [ABC del apalancamiento de recursos para la seguridad vial territorial](fuentes/abc-apalancamiento-recursos-seguridad-vial.md) — Documento matriz (163 páginas) de la serie de apalancamiento: marco conceptual, fuentes tradicionales, socios externos, mecanismos innovadores (FPR, crowdfunding, finanzas mixtas, bonos temáticos), ruta metodológica y recomendaciones. Cita el contrato ANSV-035-2025. (ingerido)
- [Apalancamiento de Recursos — Cooperación Internacional (Documento Base)](fuentes/apalancamiento-cooperacion-internacional-base.md) — Plantilla y guía para estructurar propuestas de cooperación internacional en seguridad vial; caso ilustrativo hipotético (Buenaventura). (ingerido)
- [Apalancamiento de Recursos — Alianzas Privadas](fuentes/apalancamiento-alianzas-privadas.md) — Plantilla y guía para invitar al sector privado (RSE/ESG) a alianzas de seguridad vial; caso ilustrativo con empresa ficticia (Tocancipá). (ingerido)
- [Apalancamiento de Recursos — Apalancamiento Público (Entidades Públicas)](fuentes/apalancamiento-publico-entidades.md) — Plantilla y guía para solicitar cofinanciación pública (MGA/SGR); caso ilustrativo (Aguachica). (ingerido)

### Productos propios del proyecto / análisis técnico (4, 4 ingeridas — completo)

- [Análisis Técnico de la Siniestralidad Vial en Colombia — comparativo 1er semestre 2025-2026 (Mateus)](fuentes/analisis-tecnico-siniestralidad-vial-mateus-2026.md) — Producto propio de la DCI (14 sept. 2026), autoría individual identificada (Javier Alejandro Mateus Perafán); incremento del 20 % en fallecidos, con motociclistas explicando 87,5 % del aumento. (ingerido)
- [Producto 2 — Estado del Arte: motociclistas (Consorcio Prevención Motovial)](fuentes/producto2-estado-del-arte-motociclistas.md) — Consultoría contratada por la ANSV/DCI (180 páginas, V5, oct. 2025), supervisada por Nelson Daniel Vega (DCI); revisión sistemática de evidencia normativa/técnica/económica y benchmarking internacional sobre seguridad vial de motociclistas, por las 8 áreas del Sistema Seguro. (ingerido)
- [Producto 3 — Caracterización de usuarios de motocicleta (Consorcio Prevención Motovial)](fuentes/producto3-caracterizacion-usuarios-motocicleta.md) — Misma consultoría (contrato IAP-009-2024), estudio mixto (encuesta nacional + cualitativo) con desagregación por las 8 regiones ANSV/DCI; hallazgo central: la siniestralidad de motociclistas no sigue un patrón único, varía fuertemente por territorio. (ingerido)
- [Producto 4 — Análisis de información estadística de la siniestralidad en motocicleta (Consorcio Prevención Motovial)](fuentes/producto4-analisis-informacion-estadistica-motociclistas.md) — Análisis estadístico oficial (INMLCF 2015-2024) por las 8 regiones ANSV/DCI, con matriz multicriterio de priorización territorial (municipio priorizado: Yopal, Casanare, tasa de 31,17 fallecidos por 100.000 hab.) y tramos críticos georreferenciados. Cierra la secuencia de los tres productos de esta consultoría (contrato IAP-009-2024). (ingerido)

### Gestión de la velocidad (5, pendientes)

- 230607 - Anexo - Lineamientos Planes gestión de la velocidad V4.pdf — (pendiente-ingest)
- 230607 - Programa Nacional de Gestión de velocidad.pdf — (pendiente-ingest)
- Guia_de_Control_en_Velocidad (1).pdf — (pendiente-ingest)
- R. 20233040025895 - 22-06-2023 planes de gestión de velocidad.pdf — (pendiente-ingest; posible duplicado o versión distinta del Anexo/Lineamientos PGV V4 — verificar durante el ingest)
- Uso_de_Tecnologias_para_el_Cumplimiento_de_Limites_de_Velocidad.pdf — (pendiente-ingest)

### Alcoholimetría y control metrológico (2, pendientes)

- CONTROL METROLOGICO ALCOHOSENSORES Resolucion-88919-de-2017.pdf — (pendiente-ingest)
- REGLAMENTO-TECNICO-ALCOHOSENSORES.pdf — (pendiente-ingest; posible relación directa con la resolución anterior — verificar)

### Organismos y agentes de tránsito — conceptos y circulares Mintransporte (≈35, pendientes)

Bloque más numeroso de la carga nueva: conceptos jurídicos, circulares y resoluciones de Mintransporte/ANSV sobre habilitación, categorización, competencias, sanciones y funcionamiento de Organismos de Tránsito (OT) y Agentes de Tránsito (AT). Varios archivos comparten número de radicado o de resolución — no se asume duplicación de contenido sin verificar cada uno durante el ingest.

- 20201340148641 REQUISITOS PARA HBILITACIÓN.pdf — (pendiente-ingest)
- 20201340395541 PUESTOS DE CONTROL.pdf — (pendiente-ingest)
- 20214201376171 INCORMPORACIÓN cia en runt.pdf — (pendiente-ingest)
- 20221340926831 CAUSALES PARA PERDIDA DE HABILITACIÓN OT-AT.pdf — (pendiente-ingest)
- 20221341034361 Tránsito. Agente de tránsito competente. negarse a la prueba de alcoholimetria.pdf — (pendiente-ingest)
- 20221341274911 de 3-11-2022 como elaborar IPAT.pdf — (pendiente-ingest)
- 20231341331961 TR_NSITO - Formulario _nico Nacional de Comparendo.pdf — (pendiente-ingest)
- [Circular Externa 20234000000677 de 2023 — Efectos de la Ley 2197 de 2022](fuentes/circular-externa-20234000000677-ley-2197-2022.md) — resuelve la incertidumbre "Ley 2197" ya registrada en `fuentes/circular-externa-157-2024-videos-infracciones.md`: es una norma real y distinta (seguridad ciudadana), cuyo Art. 58 reforma el Art. 7 de la Ley 769/2002. Los tres archivos con este radicado (`20234000000677 CIRULAR EFECTOS LEY 2197 DE 2022 MINTRANSPORTE.pdf`, `20234000000677 municipio y la función de control y vigilancia.pdf` y `MT 20234000000677 EFECTOS LEY 2197 DE 2022.pdf`) corresponden al mismo acto administrativo (dos son escaneos duplicados sin texto extraíble; el tercero, con texto OCR, fue la fuente usada). (ingerido)
- 2024000000257 explica proc para asigna rangos a los municipios.pdf — (pendiente-ingest)
- 202411000000277 a las auto nacion ANSV-ANI-INVIAS EXCPE DEL USO DE LA CONTRAT DIREC.pdf — (pendiente-ingest)
- 20241340092641 organismos de transito su denominación y tipo de organización.pdf — (pendiente-ingest)
- 20241340750291 ORGANISMOS DE TRANSITO COMPE -JURIS.pdf — (pendiente-ingest)
- 20241340750291 concepto funciones de las autoridad y OT.pdf — (pendiente-ingest; mismo radicado que el anterior — verificar)
- 20244000000407 instruc suspención por reincidencia.pdf — (pendiente-ingest)
- 20244000000407 reincidencia y sanción.pdf — (pendiente-ingest; mismo radicado que el anterior — verificar)
- 20244000000877 imparte instrucción a la ANSV, OT, AT, OAT control condiciones tec meca y seguro obli.pdf — (pendiente-ingest)
- 20245000000907 DEL 27-12-2024 CIRCULAR AUTORIDADES DEL SECTOR TRANSPORTE NACIONAL PRINCIPOS DE CORDINACIÓN.pdf — (pendiente-ingest)
- 20251340204461 CONCE CONVENIOS ENTRE PROVINCIAS.pdf — (pendiente-ingest)
- 20251340239201 OT AREAS METROPOLITANAS.pdf — (pendiente-ingest)
- 20251340864151 PRESCRIPCION EN MATERIA DE TRÁNSITO.pdf — (pendiente-ingest)
- Tránsito – Prescripción en materia de tránsito. 20211340731911.pdf — (pendiente-ingest; ¿mismo tema que el anterior, radicado distinto? verificar)
- 20251340953491 vinculación del propietario.pdf — (pendiente-ingest)
- 2025400000037 circula zonas diferenciales para la pres ser públi instrucción ejercicio de control.pdf — (pendiente-ingest)
- zonaas diferenciales.pdf — (pendiente-ingest; posible material de apoyo del anterior)
- 20254000000377 DEL 17-07-2025 INST EMP TRAN PUBL ESCO USO CINTURON DE TRES PUNTOS SEGURIDAD NIÑOS.pdf — (pendiente-ingest)
- 20254000000387 BAHIAS DE ASCENSO Y DESCENSO DE PASAJEROS LINEAMIENTOS A LAS AUT SEGURIDAD VIAL.pdf — (pendiente-ingest)
- 20254000000567 CIRCULAR INSTRUCCION AGENTES DE TRÁNSITO Y DITRA VEH DE CARGA PROCESO.pdf — (pendiente-ingest)
- 20254000000627 de 24-09-2025 ordena la inmoviliz vehiculos con traspaso a persona indeterminada.pdf — (pendiente-ingest)
- FACULTADES AGENTES DE TRANSITO MT 20231340406361 -2023.pdf — (pendiente-ingest)
- GUÍA PARA EL REGISTRO DE ENTIDADES COMO ORGANISMOS DE APOYO.pdf — (pendiente-ingest)
- ANEXO 1 A LA GUIA PARA EL REPORTE.pdf — (pendiente-ingest; posible anexo del anterior — verificar)
- RESOLUCION ORGANISMOS DE APOYO AL TRANSITO 21-08-2020.pdf — (pendiente-ingest)
- Resolucion_0011268_2012 manual elaboración informe de siniestros.pdf — (pendiente-ingest)
- Resolucion_3027 de 2010  Mintransporte actualiza la codificacion de infracciones.pdf — (pendiente-ingest)
- CHALECOS 20241340489771.pdf — (pendiente-ingest)
- REINSIDENCIA.pdf — (pendiente-ingest)
- concepto mintransporte agentes de tránstio.pdf — (pendiente-ingest)
- organismos de tránsito y agentes de tránsito.pdf — (pendiente-ingest)
- ´20251340026531 CONCEPTO FUNCIONES DE LOS INSPECTORES DE POLICIA CON FUNCIONES DE TRÁNSITO.pdf — (pendiente-ingest)
- PROPUESTA PARA MEJORAR LA EFECTIVIDAD EL SISTEMA SANCIONATORIO DE INFRACCIONES DE TRÁNSITO EN COLOMBIA.pdf — (pendiente-ingest)
- manual-de-policia-judicial.pdf — (pendiente-ingest)
- Actualización Cartilla manejo presupuestal multas tránsito OT 2016.pdf.pdf — (pendiente-ingest)
- circular 00000018 de 2012 super transporte.pdf — (pendiente-ingest)

### Fotodetección y circulares de control ya conocidas — versiones adicionales (5, pendientes)

- Circular_Externa_016_de_2025 zonas urbanas, escolares, dotación y residenciales.pdf — (pendiente-ingest)
- Circular_Externa_051_de_2025 foto detención.pdf — (pendiente-ingest)
- Circular_Externa_Fotodeteccion 2023300074061-2023.pdf — (pendiente-ingest)
- Circular-externa-05-de-2017 siras.pdf — (pendiente-ingest)
- Circular_042_de_2024 SAST.pdf — (pendiente-ingest)
- Circular_049_de_2024.pdf — (pendiente-ingest)

### ROT — Red de Observatorios Territoriales y gestión del conocimiento (5, pendientes)

- Resolución No 20263040005765 de 17-02-2026 ROT.pdf — (pendiente-ingest; ya citada indirectamente en `fuentes/producto4-analisis-informacion-estadistica-motociclistas.md` y `fuentes/respuesta-peticion-congresista-20266600072782.md` — ingest prioritario para verificación con texto primario)
- resolucion 20263040005765 17-02-2026.pdf — (pendiente-ingest; posible duplicado exacto del archivo anterior — verificar)
- RESOL SE ADOPA LA ROT 2026.pdf — (pendiente-ingest; ¿tercera copia o documento distinto? verificar)
- METADATOS EFSV 2021-2026.pdf — (pendiente-ingest)
- Modelo Nacional de Gestión del Conocimiento V2.pdf — (pendiente-ingest)

### Plan 365 / Plan 70D — materiales adicionales (4, pendientes)

- CIRCULAR CONJUNTA 023 DE 2025 plan 365 de 2025.pdf — (pendiente-ingest; posible copia adicional de la ya ingerida `fuentes/circular-conjunta-023-2025-plan-365.md` — verificar si el contenido es idéntico)
- La grafica de la ballena_24_dic_2025.pdf — (pendiente-ingest)
- aNEXO TECNICO CIRCULAR CONJUNTA 058 DE 2024.pdf — (pendiente-ingest)
- cIRCULAR CONJUNTA 058 DE 2024 LINEAMIENTOS AUT FORTALECER EL EJERCICIO DEL CONTROL.pdf — (pendiente-ingest)

### SOAT, aseguramiento y atención a víctimas (2, pendientes)

- Situación del SOAT 2024.pdf — (pendiente-ingest)
- 20254000000597 LINEAMIENTOS ASEGURAMIENTO -VICTIMAS RESP CIVIL EXTRA DE LAS EMPRESAS.pdf — (pendiente-ingest)

### Informes de gestión y seguimiento del PNSV (2, pendientes)

- Informe al Congreso de la Republica 2024.pdf — (pendiente-ingest)
- Informe de Seguimiento PNSV 2024 (1).pdf — (pendiente-ingest)

### Movilidad escolar (1, pendiente)

- Guia_de_Seguimiento_al_Plan_de_Movilidad_Escolar_para_Entidades_de_Gobiernos_Locales.pdf — (pendiente-ingest)

### Marco normativo adicional — leyes y decretos (7 catalogados; 3 ingeridos, 4 pendientes)

- Ley 105 de 1993 - Gestor Normativo - Función Pública.pdf — (pendiente-ingest)
- Ley 1242 de 2008 - Gestor Normativo - Función Pública.pdf — (pendiente-ingest)
- [Ley 336 de 1996 — Estatuto Nacional de Transporte](fuentes/ley-336-de-1996-estatuto-nacional-transporte.md) — completa con texto primario las citas ya registradas (Art. 46 lit. c, sanciones; Arts. 40-42, CONSET) en `fuentes/oficio-20254000114441-supertransporte-plan-365.md` y otras. (ingerido)
- [Ley 2294 de 2023 — PND 2022-2026, artículos sobre seguridad vial y ANSV](fuentes/ley-2294-de-2023-plan-nacional-desarrollo.md) — Arts. 174-180: amplía el mandato de la ANSV a los modos férreo y fluvial (Art. 177), ordena estrategia de campañas (Art. 178) y tecnologías de control (Art. 180). Ley ómnibus de 159 páginas; solo se revisó el capítulo de transporte. (ingerido)
- Decreto_1147_1971 categorias OT.pdf — (pendiente-ingest)
- Decreto_19_de_2012.pdf — (pendiente-ingest)
- [Decreto 2106 de 2019 — Simplificación de trámites, artículos de transporte](fuentes/decreto-2106-de-2019-simplificacion-tramites.md) — resuelve la incertidumbre ya registrada en `wiki/conceptos/plan-estrategico-seguridad-vial-pesv.md`: confirma con texto primario el Art. 110 (elimina el aval del PESV) y aporta el Art. 109 (autorización conjunta Mintransporte-ANSV de sistemas de fotodetección). Decreto de 49 páginas; solo se revisaron los Arts. 108-111. (ingerido)

### Contratación — Colombia Compra Eficiente (1, pendiente)

- cce_guia_COLOMBIA COMPRA EFICIENTE ENTIDADES DE regimen_especial.pdf — (pendiente-ingest)

### Movilidad urbana, regional y políticas conexas (5, pendientes)

- 3991 DE 2020 POL NAC MOVI URBANA Y REGIONAL.pdf — (pendiente-ingest)
- 4034 APOYO GOB NAC ACTUA PROGRAMA MOVI DE LA REGIÓN BOGOTA-CUNDINAMARCA 2021.pdf — (pendiente-ingest)
- 4161 vias para la paz.pdf — (pendiente-ingest)
- compes D.C 036 -2024 distaL PP DEL PEATON, EN BOGOTÁ PRIMERO EL PEATON 2023-2035.pdf — (pendiente-ingest)
- cartilla-movilidad-sss MINSALUD.pdf — (pendiente-ingest)
- cartilla_movilidad_segura.pdf — (pendiente-ingest; ¿misma cartilla que la anterior u otra? verificar)

### Presentaciones y materiales de difusión (2, pendientes)

- presentación Supertransporte.pptx — (pendiente-ingest)
- PRESENTACION-1-SESION AT-OT FUNCIONES Y COMPETENCIAS.pdf — (pendiente-ingest)

### Estudios técnicos, académicos y de referencia (5, pendientes)

- SDP-publication2 BID ESTUDIO DE CASO.pdf — (pendiente-ingest)
- REGIMEN JURIDICO DE TRANSITO ALTA FINAL (1) version 2012 oscar david gomez pineda.pdf — (pendiente-ingest; posible tesis/monografía externa — verificar autoría y estatus como fuente secundaria durante el ingest)
- ManualControldeVelocidadpdf 2008.pdf — (pendiente-ingest)
- Matriz diánostico acción 1.1.2.xls — (pendiente-ingest; único archivo en formato Excel de todo el corpus — requiere lectura con herramienta distinta a PDF/docx)

### Resoluciones sobre estándares técnicos de vehículos — posible mismo acto en varias versiones (3, pendientes)

- RESOLUCION 20223040045295 de 2022.pdf — (pendiente-ingest)
- esca RESOLUCION 20223040045295 de 2022.pdf — (pendiente-ingest; mismo número de resolución que el anterior — verificar si "esca" indica una copia escaneada o un anexo distinto)
- Titulo 5 Res. 2022040045295 2022 (1).pdf — (pendiente-ingest; posible extracto/título específico de la misma resolución)
- MinTransporte-Resolucion-2022-N0045295_20220804.pdf — (pendiente-ingest; cuarto archivo con el mismo número — verificar)
- PLANEACIÓN CIRCULAR INTERNA NASV.pdf — (pendiente-ingest)

## Método (`fuentes/`, type: metodo)

Ninguna todavía — se crea si el usuario carga una referencia metodológica transversal.

## Conceptos (`conceptos/`)

- [Jerarquía documental del proceso de Coordinación y Articulación Interinstitucional (DCI)](conceptos/jerarquia-documental-coordinacion-interinstitucional-dci.md) — Cruce de CA-02, PR-06, PR-07 y PR-08: mapea los tres procedimientos que operativizan el ciclo "Hacer" de CA-02, y la cadena territorio (PR-08) → estrategia (PR-07) → asistencia técnica (PR-06). Incluye hallazgo de inconsistencia en la gestión documental del SIG (PR-07 y PR-08 apuntan a PR-06 sin reciprocidad).
- [Plan Estratégico de Seguridad Vial (PESV)](conceptos/plan-estrategico-seguridad-vial-pesv.md) — Cruce de la Ley 1503/2011 y el Decreto 2851/2013: instrumento de cumplimiento obligatorio para entidades/empresas con flotas de vehículos, distinto y anterior a la asistencia técnica de la DCI. Incluye hallazgo, ya resuelto con el PNSV 2022-2031, de la derogatoria (2019, Decreto 2106) del régimen de aval descrito en el Decreto 2851/2013, y de la nueva metodología ANSV (2020, Resolución 1565/2014).
- [Organismos y autoridades de tránsito](conceptos/organismos-y-autoridades-de-transito.md) — Definición legal (Ley 769/2002, Arts. 3, 6, 7; complementada por la Ley 1310/2009) del sujeto territorial con el que trabaja directamente la DCI (PR-06, PR-08); confirma que la ANSV/DCI no tienen, en el corpus ingerido, carácter de autoridad u organismo de tránsito en sentido estricto sobre los entes territoriales.
- [Genealogía normativa de "asistencia técnica"](conceptos/genealogia-asistencia-tecnica.md) — Línea de tiempo del término desde la Ley 769/2002 (2002, autoridades de tránsito en general) hasta PR-06 (2025, DCI), pasando por el Decreto 2851/2013 (2013, Mineducación), la reforma del Art. 7° Par. 3 (ANSV) y el PNSV 2022-2031 (con indicadores oficiales medibles). Incluye la definición de referencia AT/ATT del CONPES 4091 (2022, DNP) y una rama distinta dirigida a conductores individuales (Resolución 4548/2013). Hallazgo: el concepto es polisémico, no una invención de la DCI; lo nuevo en 2025 es el procedimiento, no el término.
- [Sistema Seguro — enfoque de la política de seguridad vial](conceptos/sistema-seguro-enfoque-politica-seguridad-vial.md) — Paradigma internacional (*Safe System*) adoptado por la Ley 2251/2022 y desarrollado en el PNSV 2022-2031 (ya ingerido íntegramente) para toda la política pública de seguridad vial colombiana. Incluye indicadores oficiales de "asistencia técnica" ligados a Sistema Seguro (Gobernanza), sin nombrar a la DCI — cualquier atribución a la DCI sería interpretación propia, marcada como tal.

## Entidades (`entidades/`)

- [ANSV — Agencia Nacional de Seguridad Vial](entidades/ansv-agencia-nacional-seguridad-vial.md) — Entidad matriz del corpus; creada por la Ley 1702 de 2013, con 7 dependencias estatutarias, Consejo Directivo, Fondo Nacional de Seguridad Vial y Consejo Territorial de Seguridad Vial.
- [DCI — Dirección de Coordinación Interinstitucional (ANSV)](entidades/dci-direccion-coordinacion-interinstitucional.md) — Una de las 7 dependencias estatutarias de la ANSV (Ley 1702/2013, Art. 10.6); responsable del proceso de coordinación interinstitucional y del procedimiento de asistencia técnica.
- [Corporación Fondo de Prevención Vial](entidades/corporacion-fondo-prevencion-vial.md) — Entidad predecesora del Fondo Nacional de Seguridad Vial de la ANSV; coordinadora activa de la seguridad vial antes de 2013 (Decreto 2851/2013), liquidada y traspasada a la ANSV por la Ley 1702/2013 (Arts. 7 y 21).

Otras candidatas visibles solo por nombre de archivo (a confirmar durante el ingest): Mintransporte, DNP (CONPES 4091), Superintendencia y Procuraduría, organismos de tránsito territoriales.

## Síntesis (`sintesis/`)

Ninguna todavía — se crean cuando una respuesta de QUERY o un borrador de capítulo de tesis vale la pena conservar.
