# Visualización de datos

Notebook de trabajo para construir un pipeline ETL reproducible con Python y
preparar datos para su visualización en Power BI.

## Requisitos

- Python 3.10 o posterior
- Jupyter Notebook o Visual Studio Code con soporte para notebooks

Instale las dependencias con:

```powershell
python -m pip install -r requirements.txt
```

## Datos de entrada

El archivo fuente no se incluye en este repositorio por su tamaño. Descárguelo
desde [datos.gov.co](https://www.datos.gov.co/Econom-a-y-Finanzas/Tasas-de-inter-s-activas-por-tipo-de-cr-dito-ltimo/qzsc-9esp/about_data)
y colóquelo en `datos/crudos/` con el nombre configurado en el notebook. También
puede definir `RUTA_CSV_LOCAL` en el bloque de configuración del notebook para
usar una ruta distinta.

Los archivos generados se guardan en `salidas/`. El CSV curado también se omite
porque supera el límite de tamaño por archivo de GitHub; los demás resultados
que sí caben en el repositorio se conservan.

## Ejecución

Abra `visualizacion_datos_etl_powerbi_local.ipynb` en Jupyter o VS Code y ejecute
las celdas en orden. La primera ejecución instala automáticamente las
dependencias del pipeline si faltan.
