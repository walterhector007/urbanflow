# Changelog

## [Sprint 1] - Ejercicio 01
### Added
- Inicialización del repositorio Git en rama Sprint_1.
- Creación de la estructura de directorios del proyecto.
- Creación de README.md con objetivo, introducción y criterios.
- Creación de CHANGELOG.md.

## [Sprint 1] - Ejercicio 02
### Added
- Descarga del dataset raw y almacenamiento en urbanflow/data/raw.
- Análisis de tipos de datos.
- Conteo de valores nulos.

## [Sprint 1] - Ejercicio 03
### Added
- Normalización de fechas al formato YYYY-MM-DD.
- Normalización de horas al formato 24hs.
- Normalización de ubicaciones.
- Limpieza y normalización de patentes.
- Eliminación de filas con valores relevantes vacíos.
- Detección y eliminación de outliers.
- Creación de columna exceso_velocidad_real.
- Creación de columna exceso_velocidad.
- Eliminación de filas sin infracción.
- Dataset limpio guardado en urbanflow/data/interim.

## [Sprint 1] - Ejercicio 04
### Added
- Definición de la clase FineAnalyzer.
- Método ranking de patentes más multadas (top 5).
- Método ranking de horarios con más multas (top 5).
- Método exceso promedio de velocidad.
- Método exceso real promedio de velocidad.
- Método multas por ubicación.

## [Sprint 1] - Ejercicio 05
### Added
- Gráfico de ranking de las 10 patentes más reincidentes.
- Gráfico de torta de infracciones por hora.
- Gráfico de barras de infracciones por mes.
- Gráfico de líneas de excesos por hora 00:00.
- Gráfico de líneas de excesos por fecha 1932-01-01.

## [Sprint 1] - Ejercicio 06
### Added
- Porcentaje de infracciones en fecha 1932-01-01.
- Porcentaje de infracciones en hora 00:00.

## [Sprint 1] - Ejercicio 07
### Added
- Conclusión sobre el dataset de multas.

## [Sprint 2] - Ejercicio 01
### Added
- Clonación del repositorio del Sprint 1.
- Creación de la rama Sprint_2 desde Sprint_1.
- Descarga y descompresión del dataset de imágenes.
- Almacenamiento en urbanflow/data/raw/imgs.

## [Sprint 2] - Ejercicio 02
### Added
- Listado de imágenes con nombre y tamaño en kb.
- Separación de imágenes en grupos plates y completes.
- Guardado del diccionario group_images en JSON.
- Función para mostrar 8 imágenes aleatorias en tabla 2x4.

## [Sprint 2] - Ejercicio 03
### Added
- Conversión a escala de grises de las imágenes originales.
- Suavizado de imágenes en escala de grises.
- Detección de bordes con Canny sobre imágenes suavizadas.

## [Sprint 2] - Ejercicio 04
### Added
- Extracción de patentes con OCR usando easyocr.
- Función de match entre patentes con umbral del 80%.
- Relación de patentes extraídas con dataset del Sprint 1.
- Dataset final guardado en urbanflow/data/processed.

## [Sprint 2] - Ejercicio 05
### Added
- Cantidad de multas sin imágenes.
- Cantidad de multas con imágenes.
- Cantidad de imágenes sin match.
- Cantidad de multas pendientes de pago.
- Cantidad de multas pendientes de pago con imágenes.

## [Sprint 2] - Ejercicio 06
### Added
- Conclusión sobre las imágenes y los datos del Sprint 2.

## [Sprint 3] - Ejercicio 01
### Added
- Clonación del repositorio del Sprint 2.
- Creación de la rama Sprint_3 desde Sprint_2.
- Verificación de acceso a todos los datasets.
- Descarga del dataset raw faltante.

## [Sprint 3] - Ejercicio 02
### Added
- Inicialización de DVC.
- Configuración del remote DVC en /content/remote_dvc.
- Migración de imágenes a DVC.
- Migración del dataset zip a DVC.
- Migración del dataset processed a DVC.

## [Sprint 3] - Ejercicio 03
### Added
- Modelo lógico de entidades: Vehiculo, Radar, Evidencia, Multa.

## [Sprint 3] - Ejercicio 04
### Added
- Función procesar_fila_csv para mapear filas CSV a objetos.
- Validación de la función con datos de ejemplo.
