# Urban Flow - Sprint 1

## Sprint actual: Sprint 1

## Objetivo
Aplicar conocimientos de versionado de código, organización,
limpieza del código y utilización de pandas para analizar
infracciones de velocidad en la localidad de Vaalserberg.

## Introducción y contexto
La localidad de Vaalserberg (Bélgica), en zona fronteriza
con Países Bajos y Alemania, cuenta con radares urbanos
para detección de infracciones por exceso de velocidad.
Los registros históricos provienen de sistemas heredados
con errores de formato y datos faltantes que generan
inconsistencias en el nuevo sistema.
El objetivo es analizar y depurar los datos del viejo
sistema para incorporarlos al nuevo sin inconsistencias.

## Conclusión del análisis - Sprint 1

El dataset original contenía 4000 registros de infracciones de velocidad.
Tras la normalización y limpieza, se obtuvieron 1685 infracciones reales
(registros donde la velocidad supera el límite con tolerancia del 5%).

Los principales hallazgos son:

- Las ubicaciones con mayor cantidad de infracciones son avenidas principales,
  lo que sugiere que los radares están correctamente ubicados en zonas de alto flujo.
- Una fracción significativa de los registros presentaba fechas inválidas
  normalizadas a 1932-01-01, lo que indica problemas en el sistema heredado.
- La hora 00:00 agrupa tanto capturas reales de medianoche como todas aquellas
  horas que no pudieron ser interpretadas por el nuevo sistema. Esto implica que
  este valor no puede tomarse como referencia horaria confiable sin un análisis
  adicional de la fuente original.
- El exceso de velocidad promedio entre los infractores reales supera los 15 km/h
  sobre el límite permitido, lo que representa un riesgo significativo para la
  seguridad vial de la localidad.
