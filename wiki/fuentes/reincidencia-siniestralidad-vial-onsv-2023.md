---
title: "Reincidencia en siniestralidad vial: factores asociados con la probabilidad de que un conductor reincida en siniestros viales, Colombia 2018-2022 (ONSV-ANSV, febrero 2023)"
type: fuente
tags: [onsv, ansv, reincidencia, siniestros, conductores, runt, rnat, rna, rnc, simit, regresion-logistica, motocicletas, soat, rtm, antioquia]
fuente_pdf: "Documento investigación Reincidencia.pdf"
status: ingerido
last_updated: 2026-11-03
---

# Reincidencia en siniestralidad vial (ONSV, 2023)

**Archivo fuente:** `Documento investigación Reincidencia.pdf` (30 páginas, texto extraíble a dos columnas; los gráficos y las Tablas 1 y 2 de infracciones son imagen y su contenido numérico no se extrajo). Se cita por página impresa.
**Producido por:** ANSV, Observatorio Nacional de Seguridad Vial. Autora: Diana Carolina Nova Laverde. Directivos: Juan Carlos Beltrán Bedoya (Director ANSV), Carlos Fredy Carmona Ramírez (Secretario General), Dunella Maya Sánchez (Directora ONSV). "Bogotá - Colombia, febrero 2023" (p. 2).

## Qué mide (y qué no)

"Reincidencia" aquí significa **verse involucrado como conductor en más de un siniestro vial** entre 2018 y 2022 (p. 9). No es la reincidencia sancionatoria del Código Nacional de Tránsito (dos o más infracciones en un plazo, con efectos de suspensión de licencia) ni la reincidencia en comparendos. Ver [Reincidencia en tránsito: tres sentidos del término](../conceptos/reincidencia-en-transito.md).

**Datos:** RNAT, RNA y RNC del RUNT y SIMIT, desde la bodega de datos del ONSV, con filtros de calidad sobre el número de identificación (p. 9). El documento se presenta como "un ejercicio inicial" (p. 4).

## Hallazgos citables

| Dato | Página |
| --- | --- |
| En los últimos 15 años, cerca del 30 % de los conductores involucrados en siniestros lo estuvieron más de una vez; en los últimos 5 años, el 15 %. | 4 |
| 2018-2022: más de un millón de conductores involucrados en siniestros; 15,3 % (más de 160 mil) en más de uno. De los reincidentes, 74 % en dos siniestros y 17 % en tres; 6.201 conductores en cinco o más. | 11 |
| Siniestros con víctimas: más de 450 mil conductores; 6,7 % reincidieron. 26,7 mil con dos, 3,3 mil con tres, 555 con cuatro y **211 con cinco o más** siniestros con víctimas. | 11 |
| Reincidencia por sexo: 17 % hombres y 8,1 % mujeres; con víctimas, 7,4 % y 4,8 %. | 12 |
| Mayores porcentajes de reincidencia en quienes tuvieron el primer siniestro entre los 20 y 30 años (con víctimas, entre 20 y 25). | 13 |
| 86 % de los siniestros totales ocurrieron en zona urbana; 89 % de los siniestros con reincidentes y 92 % de los siniestros con víctimas con reincidentes. | 14 |
| Antioquia concentra la mayor cantidad de siniestros y una proporción aún mayor de siniestros con reincidentes ("45 % del total", p. 14); en Antioquia hubo conductores reincidentes en más del 56 % de los siniestros totales y en casi el 31 % de los siniestros con víctimas (p. 15). Junto con Bolívar es el único departamento donde la tasa por 10.000 vehículos activos con reincidentes supera la tasa sin reincidentes. En Bolívar, Risaralda y Atlántico la reincidencia supera el 45 % de los siniestros. | 14-16 |
| 51 % de los conductores reincidentes tuvo un siniestro con una o más motocicletas; 90 % en los que tuvieron más de 10 siniestros; en siniestros con víctimas, 89 % y 100 %. | 17 |
| Hipótesis de causa: conducción imprudente 47 % del total y 49 % con reincidentes; desobedecer señales o normas 22 % y 26 %. En siniestros con víctimas: 42 % y 46 %; 23 % y 26 %. | 18 |
| Comparendos promedio: 8 en reincidentes y 6 en el total de conductores siniestrados. | 19 |
| **Reincidentes críticos** (5 o más siniestros con víctimas): principalmente hombres de 25 a 30 años en el primer siniestro; 95,9 % urbanos; Antioquia y Valle del Cauca concentran el 84 % de sus siniestros graves; 11 comparendos promedio; 28 % de comparendos pendientes (frente a 6 %) y 21 % pagados (frente a 33 %); SOAT vigente 54 % (frente a 59 %) y RTM vigente 42 % (frente a 48 %). | 21-23 |
| Modelo: regresión logística binomial sobre 1.058.261 conductores; AUC 0,693; con punto de corte 0,242 clasifica bien el 79,16 % (sensibilidad 31,7 %, especificidad 87,7 %). El documento aclara que su objetivo no es predecir sino aproximar factores. | 24 |
| Razones de probabilidad (Tabla 4): mujer 0,44; mayores de 60 años 0,43; Grupo 3 de departamentos 0,40 frente a Antioquia; zona urbana 1,15; desobedecer señales 1,11; embriaguez o SPA 0,42; cada comparendo histórico adicional 1,05. | 26 |

## Inconsistencia entre la tabla y la conclusión sobre motocicletas

Las conclusiones (pp. 26-27) dicen que "haberse visto involucrado en siniestros con víctimas con participación de motocicletas" se asocia con **mayor** probabilidad de reincidir. La Tabla 3 (p. 25) no lo respalda así: el coeficiente de motocicleta es negativo (-0,388; razón 0,68), el de víctimas también (-0,254; razón 0,78) y la interacción es positiva pero pequeña (0,068; razón 1,07). Cálculo propio (no está en la fuente): el efecto combinado de un primer siniestro con moto y con víctimas es -0,574, una razón cercana a 0,56 frente a un primer siniestro sin moto y sin víctimas. Lo único que la tabla sostiene es que, **entre quienes tuvieron un primer siniestro con moto**, la presencia de víctimas reduce menos la probabilidad que en los demás. Además, la conclusión de la p. 27 menciona a Bogotá entre las zonas de concentración, pero en el modelo Bogotá está en el Grupo 2, con razón 0,54 frente a Antioquia (pp. 24 y 26).

**Recomendación de uso:** en un producto de asesoría, citar los factores con su razón de probabilidad de la Tabla 4 (p. 26) y no la frase de conclusiones sobre motocicletas.

## Lectura para el trabajo de la DCI

- Da una base cuantitativa para focalizar asistencia técnica en **Antioquia y Valle del Cauca** cuando el tema sea reincidencia en siniestros, y para pedir a los organismos de tránsito de esos territorios cruces RUNT-SIMIT sobre conductores críticos (211 con 5 o más siniestros con víctimas, p. 11).
- Refuerza el vínculo entre historial de comparendos y riesgo de siniestro (razón 1,05 por comparendo, p. 26), coherente con la recomendación de mejorar el cobro y la oportunidad de la sanción del documento [El control operativo y la fatalidad vial](control-operativo-y-fatalidad-vial-onsv.md) (p. 20).
- Limitación de dato a tener presente: el [oficio de la FCM a la DCI](oficio-fcm-reincidentes-2023-2024.md) advierte que el SIMIT no permite trazar con certeza las suspensiones por reincidencia sancionatoria; este estudio no depende de ese dato porque mide siniestros en el RUNT.

## Conexiones

- [ONSV](../entidades/onsv-observatorio-nacional-seguridad-vial.md) · [ANSV](../entidades/ansv-agencia-nacional-seguridad-vial.md)
- [Reincidencia en tránsito: tres sentidos del término](../conceptos/reincidencia-en-transito.md)
- [Circular Externa 20244000000407 de 2024](circular-externa-20244000000407-reincidencia-comparendos.md) (reincidencia sancionatoria)
- [Producto 4 — Análisis estadístico de la siniestralidad en motocicleta](producto4-analisis-informacion-estadistica-motociclistas.md)
