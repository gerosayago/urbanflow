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
