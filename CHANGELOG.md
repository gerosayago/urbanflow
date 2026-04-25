# Changelog

## [Sprint 1] - Ejercicio 01
### Added
- Inicialización del repositorio Git en rama Sprint_1.
- Creación de la estructura de directorios del proyecto.
- Creación de README.md con objetivo e introducción.
- Creación de CHANGELOG.md.

## [Sprint 1] - Ejercicio 02
### Added
- Descarga del dataset raw en urban_flow/data/raw/.
- Análisis exploratorio: primeras filas, tipos de datos y valores nulos.

## [Sprint 1] - Ejercicio 03
### Added
- Normalización de fechas al formato YYYY-MM-DD (inválidas → 1932-01-01).
- Sustitución de horas 00:00 originales por 12:00 antes de la normalización.
- Normalización de horas al formato HH:MM 24hs (inválidas → 00:00).
- Normalización de ubicaciones: mayúsculas y limpieza de caracteres especiales.
- Normalización de patentes: formato estándar (inválidas → NA).
- Eliminación de filas con nulos en columnas críticas.
- Eliminación de outliers por método IQR en velocidad_registrada.
- Cálculo de exceso_velocidad_real y exceso_velocidad (tolerancia 5%).
- Filtrado de registros sin infracción real.
- Guardado del dataset limpio en interim/.

## [Sprint 1] - Ejercicio 04
### Added
- Clase FineAnalyzer con encapsulamiento del DataFrame limpio.
- Método ranking_patentes: top 5 patentes más multadas.
- Método ranking_horarios: top 5 horarios con más multas.
- Método exceso_promedio: exceso medio como % sobre velocidad máxima.
- Método exceso_real_promedio: exceso medio en km/h.
- Método multas_por_ubicacion: conteo de multas por ubicación.

## [Sprint 1] - Punto 05
### Added
- fines.jpg: top 10 patentes más reincidentes (barras horizontal).
- hours.jpg: porcentaje de infracciones por hora (torta).
- months.jpg: infracciones por mes ordenadas (barras horizontal).
- hour.jpg: exceso de velocidad en registros con hora 00:00 (líneas).
- date.jpg: exceso de velocidad en registros con fecha 1932-01-01 (líneas).
