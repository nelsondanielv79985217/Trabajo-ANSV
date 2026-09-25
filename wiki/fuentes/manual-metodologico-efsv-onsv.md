---
title: "Manual Metodológico de la Operación Estadística de Estadísticas de Fallecidos por Siniestros Viales (EFSV)"
type: fuente
tags: [onsv, observatorio, estadisticas, metodologia, cooperacion-internacional, bloomberg, vital-strategies, siniestralidad]
fuente_pdf: "manual-metodologico operacion estadistica FPSV.pdf"
status: ingerido
last_updated: 2026-09-25
---

# Manual Metodológico de la Operación Estadística de Estadísticas de Fallecidos por Siniestros Viales (EFSV)

**Archivo fuente:** `manual-metodologico operacion estadistica FPSV.pdf` (49 páginas) — **Código: ANSV-IAD-MG-01, Versión 00, Fecha: 2021-06-25**. Nota de nomenclatura: el nombre del archivo dice "FPSV", pero el documento y su código oficial usan la sigla **EFSV** ("Estadísticas de Fallecidos por Siniestros Viales") — se registra la discrepancia sin corregir el nombre del archivo original.
**Elaboró:** Sergio D. Martínez M., contratista, Dirección del Observatorio Nacional de Seguridad Vial (ONSV). **Revisó:** Carlos A. Hernández L., Profesional Especializado, ONSV. **Aprobó:** Jasson Cruz Villamil, Director Técnico, ONSV (p. 49, firmas digitales 2021-06-29/30).

## Qué es y por qué es relevante

Es el manual metodológico oficial de la operación estadística que produce las cifras de fallecidos por siniestros viales del país — la fuente primaria de todos los datos de siniestralidad que se citan en el resto del corpus (Plan 70D, PNSV 2022-2031, etc.). Pertenece al **Observatorio Nacional de Seguridad Vial (ONSV)**, una de las siete dependencias estatutarias de la ANSV, no a la DCI. Es útil para el trabajo de asesoría porque documenta con precisión de dónde vienen las cifras oficiales de siniestralidad que cualquier producto (oficio, concepto, informe) pueda necesitar citar.

## Marco normativo y de datos

- Base legal: Ley 1702 de 2013 (creación ANSV, funciones del ONSV); Decreto 787 de 2015; **Resolución 2273 de 2014** (Mintransporte, adopta el PNSV 2011-2021 — cita nueva para el corpus, no incluida); Art. 2° de la Ley 769 de 2002 (definiciones).
- **Fuente de datos**: registro administrativo SIRDEC (Sistema de Información de la Red de Desaparecidos y Cadáveres) del Instituto Nacional de Medicina Legal y Ciencias Forenses (INMLCF), con base en necropsias.
- **Convenio de intercambio de información**: formalizado mediante la **Resolución 1055 de 2017** del Ministerio de Transporte (cita nueva para el corpus, no incluida), que establece las condiciones de reporte de fallecimientos/lesiones por accidentes de tránsito del INMLCF a la ANSV; respaldado también en la [Ley 1702 de 2013](ley-1702-de-2013-creacion-ansv.md), Art. 18 (acceso gratuito a registros públicos) — confirma esa cita ya registrada.
- **Dos metodologías de indicadores conviven**: los "indicadores estándar nacional/tradicionales" (sin límite de tiempo entre el siniestro y la muerte) y los nuevos "indicadores a 30 días" (adoptados en este manual de 2021, alineados con el estándar internacional de comparabilidad de la OMS).

## Hallazgo — confirmación reiterada de la cooperación ANSV-Bloomberg Philanthropies-Vital Strategies

Este documento **confirma, por tercera vez en el corpus** (tras el Plan 70D), la cooperación internacional activa de la ANSV: en 2019, como iniciativa conjunta entre el **Ministerio de Salud y Protección Social**, la **ANSV** y la **Iniciativa Datos para la Salud** de **Vital Strategies**, se conformó la **Mesa Técnica Nacional Asesora para el Análisis de Información de Seguridad Vial** (p. 20, 37), integrada además por Mintransporte, DANE, INMLCF, Fiscalía General de la Nación, Superintendencia de Transporte, Instituto Nacional de Salud, Policía Nacional, Fasecolda, Federación Colombiana de Municipios y la Secretaría Distrital de Movilidad de Bogotá. La bibliografía del documento (p. 48) cita directamente: "Agencia Nacional de Seguridad Vial - Ministerio de Salud - Bloomberg Philantropies. (2019). Mesa Técnica Nacional Asesora Para el Análisis de Información de Seguridad Vial - Informe Ejecutivo." Esta Mesa discute anualmente los resultados de la operación estadística y contextualiza los indicadores comparándolos con la información de las demás entidades miembro.

## Referentes internacionales del ONSV

OMS, OPS, ITF (Foro Internacional de Transporte, integrado a la OCDE), FIA, PIARC, IRF, **IRTAD** (grupo internacional de datos de seguridad vial, Colombia en proceso de inclusión desde 2019), UNRSC, GRSP, y el Observatorio Iberoamericano de Seguridad Vial (OISEVI). Referentes nacionales: INMLCF (manual SIAVAC-SIVELCE), Grupo Centro de Referencia Nacional sobre la Violencia (GCRNV), Resolución 0011268 de 2012 de Mintransporte (Manual de Diligenciamiento del Informe Policial de Accidente de Tránsito).

## Contenido metodológico (resumen)

- **Objetivo general**: producir información estadística relevante sobre víctimas fallecidas por siniestros viales en Colombia, como insumo para la gestión de política pública.
- **Objetivos específicos**: identificar departamentos/ciudades capitales con mayores víctimas; caracterizar víctimas por sexo y edad; identificar actores viales más afectados; identificar condiciones de tiempo (meses, días, horarios) de mayor siniestralidad.
- **Desagregación**: nacional, departamental, capitales; por condición de víctima, sexo, rango de edad, mes, día de la semana, rango horario.
- **Flujo de datos**: INMLCF envía tablas mensuales al ONSV → carga y ETL en bodega de datos Azure → validación/depuración (estandarización de variables, eliminación de duplicados y de registros no terrestres) → almacenamiento → consulta y publicación en ansv.gov.co/observatorio.
- **Productos de difusión**: boletines mensuales y anuales (nacional, por departamento y por ciudad capital), tableros en Power BI, Anuario de estadísticas sobre seguridad vial. La información mensual preliminar se publica en los primeros 20 días de cada mes; la definitiva, una vez consolidada por Medicina Legal.
- **Confidencialidad**: la ANSV no publica microdatos, solo agregados vía tablero de consulta.
- **Glosario extenso** (pp. 43–47): definiciones operativas de siniestro vial, fallecido/lesionado por siniestro vial, lesionado grave, peatón (incluida la definición de "ayuda técnica" como dispositivo de movilidad reducida — término distinto de "asistencia técnica", no debe confundirse en el corpus), y decenas de definiciones de tipos de vehículo, vía e infracción, alineadas con la Ley 769/2002 y el CIE-10.

## Conexiones

- [ANSV — Agencia Nacional de Seguridad Vial](../entidades/ansv-agencia-nacional-seguridad-vial.md): se actualiza con la confirmación reiterada de la cooperación Bloomberg Philanthropies/Vital Strategies (ya documentada desde el Plan 70D) — ahora con origen institucional preciso (2019, Mesa Técnica Nacional Asesora).
- [Ley 1702 de 2013](ley-1702-de-2013-creacion-ansv.md): confirma la cita del Art. 18 (acceso gratuito a registros públicos).
- [PNSV 2022-2031](pnsv-2022-2031-documento-tecnico-soporte.md) y [Plan 70D](plan-70d-sector-transporte.md): ambas fuentes citan cifras de siniestralidad del ONSV — este manual es la fuente metodológica de esos datos.

## Incertidumbres

- No se ha verificado en este corpus el texto de la Resolución 2273 de 2014 (adopta el PNSV 2011-2021) ni de la Resolución 1055 de 2017 (condiciones de reporte INMLCF-ANSV) — ninguna está incluida en el repositorio.
- No se menciona a la DCI ni el término "asistencia técnica" en ningún punto del documento — es una fuente de otra dependencia de la ANSV (el ONSV), sin relación directa con el procedimiento PR-06.
