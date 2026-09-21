---
title: "Manual Metodológico de la Operación Estadística — Estadísticas de Fallecidos por Siniestros Viales (EFSV)"
type: fuente
tags: [ondsv, metodologia-estadistica, definiciones, glosario, pnsv-2011-2021, indicadores]
fuente_pdf: "manual-metodologico operacion estadistica FPSV.pdf"
status: ingerido
last_updated: 2026-09-21
---

## Nota sobre el alcance de esta lectura

Documento técnico-estadístico (código **ANSV-IAD-MG-01**, versión 00, 25 de junio de 2021), producido por el Observatorio Nacional de Seguridad Vial (ONSV) de la ANSV, de 49 páginas con paginación explotable (extracción limpia con `pypdf`). Se leyó completo el marco introductorio/normativo, el diseño temático (objetivos, alcance, fuentes de datos, indicadores) y el glosario de definiciones (secciones 1, 2.1, 2.2 y 4); la sección de diseño operativo detallado del proceso estadístico (2.3 a 2.8, p. 30-42 — flujogramas de recolección, procesamiento, anonimización de microdatos, comités de expertos, sistemas de producción) se escaneó por estructura sin transcripción exhaustiva, por ser metodología estadística genérica (aplicable a cualquier operación estadística certificable bajo la norma DANE, no específica de la gestión territorial que es el objeto de este trabajo de grado) — decisión de alcance documentada, análoga a la aplicada a otros documentos extensos del repositorio.

## Referencia / origen del documento

- Título completo: "Manual Metodológico de la Operación Estadística de Estadísticas de Fallecidos por Siniestros Viales" (p. 1). Proceso: "Integración, Análisis y Divulgación de Datos de Seguridad Vial" (encabezado de todas las páginas).
- Firmantes (p. 49, "Control de firmas"): **Sergio D. Martínez M.** (Contratista, Dirección Observatorio Nacional de Seguridad Vial — elaboró), **Carlos A. Hernández L.** (Profesional Especializado, Dirección del Observatorio — revisó/aprobó, según estructura de la tabla). Documento inicial, versión 00, sin cambios registrados a la fecha del documento.
- Objetivo: articular la operación estadística "Estadísticas de Fallecidos por Siniestros Viales" (EFSV) del ONSV al sistema de gestión institucional, en el marco de un proceso de certificación bajo la **Norma Técnica de Calidad del Proceso Estadístico — NTC PE 1000:2020** ante el DANE (p. 5).

## Hallazgo — meta nacional previa (PNSV 2011-2021) y meta ODS 2030, distintas de la meta del PNSV 2022-2031 ya documentada

`[Hallazgo relevante para contextualizar históricamente la meta nacional ya registrada en otras fuentes]`. Este documento (2021, previo al PNSV 2022-2031) documenta **dos metas nacionales anteriores**, no vistas hasta ahora en este repositorio:

- Meta ODS/Colombia (p. 4, cita textual): "definió como meta nacional reducir a 8,35 la tasa de fallecidos por cada 100.000 habitantes para 2030, frente al indicador de 14,87 obtenido para 2015 como línea base" (CONPES 3918, Estadísticas Vitales DANE).
- **PNSV 2011-2021** (adoptado por Resolución 2273 de 2014 del Ministerio de Transporte, ajuste del PNSV 2011-2016): objetivo general de **reducir 26% las víctimas fatales para 2021** (línea base: promedio 2005-2012 = 5.708 víctimas); objetivos específicos: reducir mortalidad de peatones 18%, de motociclistas 27%, lesiones 21%, y víctimas fatales por alcohol/sustancias psicoactivas a 0% (p. 4-5).

`[INCIERTO: este documento no reporta si esas metas del PNSV 2011-2021 se cumplieron — sería necesario consultar el cierre de ese plan o el diagnóstico del PNSV 2022-2031 (Documento técnico de soporte Mintransporte, pendiente de ingest en este mismo grupo) para saberlo.]` Es, en todo caso, evidencia de un patrón recurrente de la ANSV: fijar metas porcentuales ambiciosas de reducción de mortalidad (26% para 2011-2021, 50% para 2022-2031) — relevante para una eventual sección de la tesis sobre la trayectoria histórica de las metas de la política pública de seguridad vial en Colombia.

## Objetivos y alcance de la operación estadística (p. 7-8)

- Objetivo general (cita textual, p. 7): "Producir información estadística relevante sobre víctimas fallecidas por siniestros viales en Colombia, que sirva como insumo para la gestión de la política pública en la prevención, reducción y control de la siniestralidad vial."
- Usuarios identificados de la información (p. 7): ANSV y Ministerio de Transporte (principales), y explícitamente **"entidades territoriales como Gobernaciones, Alcaldías, Secretarías de Tránsito o Movilidad"**, además de congresistas e instituciones de educación superior — confirma que los organismos de tránsito/entidades territoriales son usuarios formalmente reconocidos de las estadísticas del ONSV, no solo receptores pasivos.
- Alcance: cifras mensuales/anuales de fallecidos por condición de víctima, sexo, grupo etario, día de la semana, rango horario, zona (rural/urbana), departamento y capitales departamentales; tasa nacional y departamental por 100.000 habitantes (p. 8).

## Fuente única de datos y metodología de conteo (p. 8, 28-29)

- Fuente: registro administrativo **SIRDEC** del INMLCF (necropsias), exclusivamente — cobertura nacional, sin desagregación municipal más allá de capitales departamentales (p. 28).
- **Explica el mecanismo detrás de las discrepancias de cifras ya detectadas entre fuentes de este repositorio** (cita textual, p. 25, nota del propio manual): "el indicador 'Número total de fallecidos por siniestros viales' no contabiliza todos los fallecidos del país en un año en particular, esto se debe a las restricciones inherentes a la base de datos... El indicador real del total de fallecidos en un año en particular dependerá de la **cifra oficial de fallecidos que reporta el DANE** como parte de las estadísticas vitales." Es decir: **la cifra del ONSV/INMLCF (usada en casi todas las demás fuentes de este repositorio) no es, por diseño metodológico propio, la cifra oficial definitiva** — esta es reportada por el DANE, con una fuente y momento de corte distintos. Esto aporta una explicación metodológica (no una resolución numérica) a la discrepancia ya registrada entre las cifras de 2024 de la Circular 023/Anexo Técnico Plan 365 (8.271) y la Respuesta al cuestionario del Congreso (8.433).
- Metodología "a 30 días" (p. 25, alineada con estándar OMS ya visto en el Antecedentes, p. 6): fallecidos "causados dentro de los 30 días a partir del hecho" — el manual documenta que este es un indicador "producto de una actualización metodológica" reciente (2021) respecto de la metodología previa sin límite de tiempo. Período de referencia mensual, con datos "provisionales hasta 30 días después del último día del mes" y consolidación definitiva "hacia mediados del año siguiente" (p. 29) — **explica textualmente por qué tantas fuentes de este repositorio usan las expresiones "cifras preliminares" / "cifras definitivas con corte a..."**.

## Glosario — definiciones oficiales (p. 43-46, selección)

- **Organismo de tránsito** (p. 44, cita textual): "Son unidades administrativas municipales distritales o departamentales que tienen por reglamento la función de organizar y dirigir lo relacionado con el tránsito y transporte en su respectiva jurisdicción." — **tercera definición independiente de "organismo de tránsito" encontrada en el corpus** (además de la Ley 769/2002 art. 6 y la Ley 1310/2009), con una redacción más breve pero sustancialmente compatible. Útil para el marco conceptual de la tesis: tres fuentes normativas/técnicas distintas convergen en la misma noción básica.
- **Accidente de tránsito** (p. 44, cita textual): "Evento generalmente involuntario, generado al menos por un vehículo en movimiento, que causa daños a personas y bienes involucrados en él e igualmente afecta la normal circulación de los vehículos..."
- Otras definiciones técnicas relevantes: peatón, conductor, pasajero, ocupante, objeto de colisión, vehículo fantasma, agente de tránsito, comparendo, croquis, infracción (simple/compleja), licencia de conducción/tránsito — dan una base terminológica formal para el marco conceptual de la tesis, aunque no específica de la asistencia técnica territorial.

## Marco teórico sobre comportamiento vial (p. 8-11, resumen)

El documento incluye un extenso marco teórico sobre determinantes conductuales de la siniestralidad (teoría del compromiso social, del aprendizaje social, de la conducta planeada; efecto de la distracción por celular; uso de luces diurnas) — de relevancia tangencial para esta tesis (se orienta a explicar por qué ocurren los siniestros, no a la gestión institucional/territorial de la asistencia técnica), por lo que no se transcribe en detalle. Se destaca un dato comparativo internacional (p. 9): países como Suecia, Dinamarca, Suiza, Francia y Japón tienen tasas de 2,8-4,5 fallecidos/100.000 hab., y España pasó de >15/100.000 a 3,7/100.000 en 15 años — contraste útil para dimensionar la magnitud de la brecha de Colombia (tasa 2024 de 15,4/100.000 según la Respuesta al cuestionario del Congreso).

## Relación con las demás fuentes de este repositorio

- [respuesta-peticion-congresista-20266600072782](respuesta-peticion-congresista-20266600072782.md) y [circular-023-2025-plan-365](circular-023-2025-plan-365.md): este manual **explica metodológicamente** la discrepancia numérica ya detectada entre ambas fuentes (8.271 vs. 8.433 fallecidos 2024) — atribuible a que el indicador del ONSV/INMLCF no es la cifra oficial definitiva (esa la reporta el DANE), y a la existencia de cortes preliminares/definitivos con rezago de varios meses.
- [ley-769-2002-codigo-nacional-transito](ley-769-2002-codigo-nacional-transito.md) y [ley-1310-2009-agentes-transito](ley-1310-2009-agentes-transito.md): esta fuente aporta una tercera definición de "organismo de tránsito", sustancialmente compatible con las otras dos.
- [analisis-tecnico-siniestralidad-mateus](analisis-tecnico-siniestralidad-mateus.md): usa exactamente las mismas variables de desagregación que este manual describe como diseño oficial de la operación estadística (actor vial, sexo, edad, día, hora, zona, departamento) — confirma que ese análisis de 2026 sigue la metodología EFSV aquí documentada.
- `wiki/index.md` — pendiente `Documento técnico de soporte Mintransporte- PNSV 2022-2031.pdf`: sería la fuente más indicada para verificar si las metas del PNSV 2011-2021 aquí documentadas (26% de reducción) se cumplieron, dato que este manual no reporta.

## Relevancia para el trabajo de grado

`[Interpretación propia, no una afirmación de la fuente]`: el valor principal de este documento para la tesis no es normativo ni institucional, sino **metodológico**: aporta un fundamento técnico riguroso para entender por qué las cifras de siniestralidad varían entre fuentes del mismo repositorio (preliminar vs. definitivo, ONSV/INMLCF vs. DANE, metodología "a 30 días"), lo cual es directamente relevante para la regla de citación exacta y rigor metodológico de este proyecto: cualquier cifra de fallecidos citada en el cuerpo de la tesis debe indicar explícitamente su fuente (INMLCF/SIRDEC vs. DANE), su fecha de corte y si es preliminar o definitiva, y no asumir que dos cifras "de 2024" de fuentes distintas son comparables sin verificar estos tres elementos.

## Conceptos y entidades mencionados

**Entidades**: ANSV, Observatorio Nacional de Seguridad Vial (ONSV), INMLCF (SIRDEC), DANE, DNP, Ministerio de Transporte, OMS.

**Personas**: Sergio D. Martínez M. (elaboró, contratista ONSV), Carlos A. Hernández L. (revisó/aprobó, ONSV).

**Conceptos/instrumentos**: Estadísticas de Fallecidos por Siniestros Viales (EFSV), NTC PE 1000:2020, metodología "a 30 días" (estándar OMS), Código Divipola, PNSV 2011-2021 (Resolución 2273/2014), CONPES 3918 (ODS).

## Incertidumbres

- `[INCIERTO: no se reporta en este documento si las metas del PNSV 2011-2021 (reducción del 26%) se cumplieron.]`
- No se transcribió en detalle la sección de diseño operativo del proceso estadístico (p. 30-42: recolección, procesamiento, anonimización, comités de expertos) — ver nota de alcance al inicio de esta página; consultar el PDF original si se requiere el detalle de esos procedimientos internos del ONSV.
- El glosario completo (p. 43-48) no se transcribió íntegramente — se citan solo las definiciones de mayor relevancia para el marco conceptual de la tesis.

## Ver también

- [fuentes/respuesta-peticion-congresista-20266600072782](respuesta-peticion-congresista-20266600072782.md)
- [fuentes/analisis-tecnico-siniestralidad-mateus](analisis-tecnico-siniestralidad-mateus.md)
- [fuentes/ley-769-2002-codigo-nacional-transito](ley-769-2002-codigo-nacional-transito.md)
- [conceptos/asistencia-tecnica-bundle-pr06](../conceptos/asistencia-tecnica-bundle-pr06.md)
