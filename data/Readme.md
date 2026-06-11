
## Conclusión Sprint 2

El dataset de imágenes del sistema de radares urbanos de Vaalserberg
presentó una cobertura parcial de las multas registradas. De un total
de 1713 multas procesadas, solo 28 contaban con una imagen asociada
que pudo ser validada mediante OCR, lo que representa menos del 2%
del total.

El sistema de extracción de patentes mediante easyocr mostró resultados
variables. Algunas patentes fueron detectadas con precisión del 100%
como BP717, BB8986 y MPX9357, mientras que otras presentaron ruido
adicional como caracteres especiales o texto del fondo de la imagen.

De las 91 imágenes del grupo plates procesadas, 63 no encontraron
coincidencia con ninguna multa del dataset, lo que puede indicar
errores de detección del radar, patentes de vehículos no registrados
en el sistema, o imágenes de baja calidad que afectaron la lectura OCR.

Finalmente, de las 430 multas pendientes de pago, solo 6 cuentan con
evidencia visual validada, lo que dificulta el proceso de cobro y
seguimiento de infracciones.

## Conclusión Sprint 3

En este sprint se profesionalizó la solución incorporando persistencia
en base de datos relacional mediante SQLAlchemy y control de versiones
de datos con DVC.

Se migró exitosamente el dataset procesado del Sprint 1 a una base de
datos SQLite con 4 tablas relacionadas: 1713 multas, 66 vehículos,
4 radares y 28 evidencias. Las consultas SQL permitieron obtener
información relevante como las patentes más reincidentes, los radares
más activos y el porcentaje de multas con evidencia visual.

Se implementó además una base de datos vectorial con ChromaDB y OpenClip
que permite búsquedas por similitud de imágenes. Se vectorizaron 106
imágenes de patentes, permitiendo identificar vehículos a partir de
una imagen de consulta.

La integración entre la base de datos relacional y la vectorial
representa un avance significativo en la capacidad del sistema para
validar y procesar evidencias visuales de infracciones de velocidad.

## Conclusión Sprint 3

En este sprint se profesionalizó la solución incorporando persistencia
en base de datos relacional mediante SQLAlchemy y control de versiones
de datos con DVC.

Se migró exitosamente el dataset procesado del Sprint 1 a una base de
datos SQLite con 4 tablas relacionadas: 1713 multas, 66 vehículos,
4 radares y 28 evidencias. Las consultas SQL permitieron obtener
información relevante como las patentes más reincidentes, los radares
más activos y el porcentaje de multas con evidencia visual.

Se implementó además una base de datos vectorial con ChromaDB y OpenClip
que permite búsquedas por similitud de imágenes. Se vectorizaron 106
imágenes de patentes, permitiendo identificar vehículos a partir de
una imagen de consulta.

La integración entre la base de datos relacional y la vectorial
representa un avance significativo en la capacidad del sistema para
validar y procesar evidencias visuales de infracciones de velocidad.
