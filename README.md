# Argentina Energy Monitor

Plataforma de datos orientada a la integración y análisis de información histórica del sistema eléctrico argentino.

## Objetivo

Desarrollar un pipeline de Data Engineering que permita integrar, transformar, validar y analizar datos de demanda, oferta y generación eléctrica en Argentina.

El proyecto busca construir una solución reproducible que facilite el análisis de la evolución del sistema eléctrico y la exploración de sus principales patrones.

## Preguntas de investigación

- ¿Cómo evoluciona la demanda eléctrica argentina?
- ¿Qué diferencias existen entre los patrones de demanda de las provincias?
- ¿Cómo cambia la composición de la oferta eléctrica?
- ¿Cómo se distribuye la generación eléctrica local entre centrales, agentes y tecnologías?

## Fuentes de datos

Los datos iniciales provienen de CAMMESA e incluyen:

- Demanda horaria por provincia.
- Oferta total horaria por fuente de energía.
- Generación local mensual por máquina.

Período inicial relevado: enero de 2023 a septiembre de 2026.

## Tecnologías

- Python
- PySpark
- SQL
- Databricks
- Delta Lake
- Git / GitHub

## Arquitectura

El proyecto implementará una arquitectura basada en el enfoque Medallion, complementada con una zona Landing para la recepción y conservación de los archivos originales.

El flujo de datos estará organizado en cuatro zonas:

- **Landing:** almacenamiento de los archivos originales recibidos desde CAMMESA.
- **Bronze:** ingesta de los datos originales en tablas Delta.
- **Silver:** limpieza, normalización y validación de los datos.
- **Gold:** modelado de información e indicadores orientados al análisis.

## Estado del proyecto

En desarrollo — relevamiento de fuentes y definición del alcance completados.
