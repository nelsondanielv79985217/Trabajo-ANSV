---
title: "Metadatos: Operación Estadística de Fallecidos por Siniestros Viales (EFSV) 2021-A-2026 — ONSV"
type: fuente
tags: [onsv, efsv, metadatos, estadistica, fallecidos-siniestros-viales, sirdec, inmlcf, mortalidad-30-dias]
fuente_pdf: "METADATOS EFSV 2021-2026.pdf"
status: ingerido
last_updated: 2026-09-28
---

# Metadatos: Operación Estadística de Fallecidos por Siniestros Viales (EFSV) 2021-A-2026 — ONSV

**Archivo fuente:** `METADATOS EFSV 2021-2026.pdf` (10 páginas, texto extraíble vía `pdftotext -layout`, leído íntegramente).
**Fecha de producción:** 8 de agosto de 2025.
**Autora (Equipo Técnico):** Katherine Sánchez Casas.
**Entidad productora:** Agencia Nacional de Seguridad Vial (ANSV) — Observatorio Nacional de Seguridad Vial (ONSV).
**Firmas institucionales:** Mariantonia Tabares Pulgarín (Directora ANSV), Maderley Pérez Penagos (Secretaria General E), Rubiel de Jesús Zuleta Carmona (Director ONSV).

## Qué es y por qué es relevante

Ficha de metadatos técnicos (bajo estándar de documentación estadística) de la Operación Estadística de Fallecidos por Siniestros Viales (EFSV), la operación estadística oficial del ONSV sobre mortalidad vial en Colombia. Es la fuente más completa del corpus sobre la metodología, fuente de datos, periodicidad y estándares de calidad de la cifra oficial de fallecidos por siniestros viales, insumo directo de cualquier producto de asesoría que cite cifras de mortalidad vial.

## Contenido relevante

**Identificación**: Idno `ANSV-ONSV-EFSV-2021`; ID del documento `COL-ANSV-ONSV-EFSV-2021-A-2026`.

**Antecedentes y evolución metodológica**: Antes de la EFSV, el reporte de fallecidos se basaba en dos fuentes con diferencias metodológicas: las Estadísticas Vitales del DANE y las estadísticas de muertes por causas externas del Instituto Nacional de Medicina Legal y Ciencias Forenses (INMLCF). La ANSV/ONSV diseñó la EFSV a partir del aprovechamiento estadístico del registro administrativo **SIRDEC** (Sistema de Información Red de Desaparecidos y Cadáveres) del INMLCF, aplicando una metodología estandarizada. Un hito clave fue la adopción del estándar internacional de **"mortalidad a 30 días"** (documentado en el Anuario Nacional de Siniestralidad Vial 2019), alineado con las recomendaciones de la OMS y el International Transport Forum (ITF). En 2021, la operación obtuvo certificación de calidad bajo la **Norma Técnica del Proceso Estadístico (NTC PE 1000)**.

**Referentes internacionales**: OMS ("Data systems: A road safety manual for decision-makers and practitioners" — estándar de mortalidad a 30 días); International Transport Forum/OCDE ("Glossary for transport statistics" — definiciones de Siniestro Vial, Fallecido, tipologías de vehículos/usuarios); Clasificación Estadística Internacional de Enfermedades (CIE-10) para la clasificación de causas de muerte.

**Alcance**: Indicador principal — "Fallecido a 30 días". Variables: fecha del hecho, ubicación (departamento, capital, zona), características de la víctima (sexo, edad, rol en la vía), características del siniestro (clase de accidente, tipo de vehículo). Unidad de observación: registro de necropsia en la base SIRDEC del INMLCF. Unidad de análisis: persona fallecida a 30 días por siniestro vial en Colombia.

**Cobertura**: todo el territorio nacional, con desagregación departamental y municipal (ciudades capitales). Universo: fallecimientos no fetales por siniestros viales ocurridos en Colombia, captados por el SIRDEC.

**Productores y financiación**: Entidad autora — ONSV; agencia financiadora/ejecutora — ANSV.

**Recolección de datos**: período de recolección 2014-2025; ciclo mensual con carácter preliminar y anual con carácter definitivo; acopio mediante convenio interadministrativo (sin entrenamiento de recolectores, al ser transferencia de archivos); proceso ETL (Extracción, Transformación y Carga) para la ingesta a la bodega institucional; validación/depuración post-cargue; sin procesos de imputación de datos.

**Análisis estadístico**: de tipo descriptivo y coyuntural (frecuencias, proporciones, tasas, variaciones), desagregado por condición agrupada de la víctima, sexo, rango de edad, mes, día de la semana y rango horario.

**Advertencia de calidad**: las cifras de los boletines mensuales son **preliminares**; para análisis definitivos deben usarse los datos consolidados del Anuario Nacional de Siniestralidad Vial.

**Acceso a los datos**: acceso agregado, público y gratuito vía el portal web del ONSV; acceso a microdatos anonimizados sujeto a solicitud formal y protocolos de seguridad de la entidad. Declaración de confidencialidad conforme a la **Ley 2335 de 2023**. Cita textual requerida: "Fuente: Agencia Nacional de Seguridad Vial www.ansv.gov.co"; prohibida la reproducción/copia electrónica masiva sin autorización previa por escrito de la ANSV. Derechos de autor protegidos por la Ley 1032 de 2006.

## Conclusión

Los metadatos formalizan que la cifra oficial de fallecidos por siniestros viales de Colombia (EFSV) se produce a partir del SIRDEC del INMLCF, bajo el estándar de mortalidad a 30 días y certificación NTC PE 1000, con periodicidad mensual (preliminar) y anual (definitiva/consolidada en el Anuario Nacional de Siniestralidad Vial) — insumo metodológico esencial para citar correctamente cifras de mortalidad vial en cualquier producto de asesoría de la DCI/ANSV.

## Conexiones

- [Manual Metodológico de la Operación Estadística EFSV (ANSV-IAD-MG-01, 2021)](manual-metodologico-efsv-onsv.md): manual metodológico completo (49 páginas, Versión 00, 2021-06-25) de la misma operación estadística; esta ficha de metadatos (2025) es una actualización sintética posterior, con el mismo estándar de mortalidad a 30 días y la misma fuente SIRDEC/INMLCF, que no reemplaza al manual pero lo complementa con la documentación formal de metadatos exigida por buenas prácticas estadísticas.
- [Manual Único de Policía Judicial — Fiscalía General de la Nación](manual-unico-policia-judicial-fiscalia.md): el INMLCF, fuente primaria del SIRDEC/EFSV, es la misma entidad que ese manual identifica como responsable de la identificación técnico-científica de elementos materiales de prueba en accidentes de tránsito con víctimas.
- [Producto 4 — Análisis de información estadística de motociclistas](producto4-analisis-informacion-estadistica-motociclistas.md): fuente ya ingerida que usa datos del INMLCF; se puede verificar en un futuro QUERY si utilizó específicamente la EFSV o una fuente distinta de medicina legal.
- [Modelo Nacional de Gestión del Conocimiento — ONSV (V2, 2025)](modelo-nacional-gestion-conocimiento-onsv-v2.md): el ONSV, entidad productora de esta operación estadística, es también la entidad que define ese modelo transversal de gestión del conocimiento en seguridad vial, ingerido en el mismo bloque del corpus (ROT — gestión del conocimiento).

## Incertidumbres

- No se verifica en este corpus el texto íntegro de la Ley 2335 de 2023 (reserva estadística) ni de la Norma Técnica del Proceso Estadístico NTC PE 1000, citadas solo por referencia.
- No se identifica en este corpus el Anuario Nacional de Siniestralidad Vial (fuente de los datos consolidados/definitivos), que no forma parte de los archivos cargados.
