
# ETL Coordinador Eléctrico Nacional

## Descripción

Este proyecto desarrolla un proceso ETL (Extract, Transform, Load) para manejar y analizar datos de medidas eléctricas existentes en el coordinador electrico nacional (CEN). Los datos son proporcionados por en la plataforma de mediciones del CEN, y están disponibles en archivos CSV segmentados por intervalos de 15 minutos o 1 hora.


## Objetivo

El objetivo principal del proyecto es facilitar la extracción, transformación y carga de estos datos en una base de datos Postgres, proporcionando una arquitectura de datos sólida y un conjunto de herramientas para el análisis y la visualización de las mediciones de energía activa y reactiva, tanto de retiro como de inyección.

## Arquitectura

La arquitectura del sistema se compone de las siguientes partes:

1. **Extracción de Datos**: Se extraen los archivos CSV desde la fuente https://medidas.coordinador.cl/reportes/, los cuales contienen información detallada sobre las medidas eléctricas.
2. **Transformación de Datos**: Se realiza una limpieza y transformación de los datos para asegurar la calidad y la consistencia a través de scripts de Python.
3. **Carga de Datos**: Los datos transformados se cargan en una base de datos Postgres, diseñada para soportar consultas complejas y análisis de datos.

## Estructura del Repositorio

- `/etl`: Contiene los scripts de Python para el proceso ETL.
- `/db`: Incluye los esquemas de la base de datos y las migraciones necesarias.
- `/docs`: Documentación adicional y referencias.
- `README.md`: El archivo que estás leyendo actualmente.

## Uso

Para ejecutar el proceso ETL:

```bash
python etl/main.py
```

## Contacto

Para más información o consultas, contacta a Joaquín Rohland H. en joaquinrohland@gmail.com
