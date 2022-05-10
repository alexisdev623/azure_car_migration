# Azure Car Files Ingestion

Un problema cotidiano de las empresas consiste en la generación masiva de archivos, y en big data el principal reto es lograr generar insights y conclusiones de negocio del análisis de toda esa información.

Para nuestro caso el cliente ha solicitado:

Se tienen un total de 108 cvs con la información de las ventas históricas de una empresa de carros.
Se requiere su análisis usando las herramientas de Azure.

1. Generar las 3 zonas correspondientes a un datalake en Azure
2. Hacer un Pipeline de Ingesta en el datalake, que se dispare manualmente y que cargue los archivos de la ruta y luego los elimine

3. Generar un reporte analítico de los datos usando Pyspark

4. Generar un Dashboard que genere insghts

Para esta solución se parte de la aquitectura de las 3 zonas: Bronze, Silver y Gold.

Para la homologación de los nombres de la comuna/region, se puede consultar la siguiente API. https://apis.digital.gob.cl/dpa/

Nombre de las columnas PLACA;MARCA;MODELO;AÑO;ID_CLIENTE;COMUNA;REGION;SEXO;ACTIVIDAD;VALORVEHICULO;FEC_TRANSFE RENCIA;COLOR2;EDAD;VIGENCIA


![alt text](https://docs.microsoft.com/es-ES/azure/architecture/solution-ideas/media/ingest-etl-and-stream-processing-with-azure-databricks.png)
