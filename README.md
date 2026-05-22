# Urban Flow

## Sprint actual: Sprint 2

## Objetivo
Aplicar conocimientos adquiridos en el tratamiento de imágenes,
la programación limpia y clara.

## Introducción y contexto Sprint 1
La localidad de Vaalserberg (Bélgica), ubicada en zona fronteriza
con Países Bajos y Alemania, cuenta con un sistema de radares
urbanos para detección de infracciones por exceso de velocidad.
Los registros históricos provienen de sistemas heredados con
errores de formato y datos faltantes.

## Introducción y contexto Sprint 2
Los radares urbanos generan registros administrativos de multas
de forma automática y las cámaras asociadas registran la evidencia
visual que acompaña y valida la infracción. El objetivo es
desarrollar un sistema que determine qué multas tienen evidencia
visual válida.

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
errores de detección del radar o imágenes de baja calidad.

Finalmente, de las 430 multas pendientes de pago, solo 6 cuentan con
evidencia visual validada, lo que dificulta el proceso de cobro y
seguimiento de infracciones.
