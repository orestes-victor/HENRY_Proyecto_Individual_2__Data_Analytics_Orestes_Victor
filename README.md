# Análisis de Homicidios Viales en CABA, Argentina

## Introducción
Este proyecto emula el papel de un Analista de Datos dentro de un equipo de una consultora. El Observatorio de Movilidad y Seguridad Vial (OMSV), una entidad especializada adscrita a la Secretaría de Transporte del Gobierno de la Ciudad Autónoma de Buenos Aires, nos encargó desarrollar un análisis detallado de datos.

El propósito de este análisis es proveer a las autoridades de información clave para implementar estrategias que reduzcan el número de muertes resultantes de accidentes viales en CABA. Se nos ha proporcionado un conjunto de datos sobre los fallecimientos en accidentes viales entre 2016 y 2021 para este fin.

Los entregables del proyecto incluyen un informe detallado sobre las actividades realizadas, las metodologías empleadas, y las conclusiones principales, además de un dashboard interactivo que mejore la visualización y análisis de los datos.

## Contexto
Los accidentes de tránsito son incidentes que involucran vehículos y pueden ser causados por múltiples factores, resultando en daños materiales y/o físicos a los implicados. En la densamente poblada Ciudad Autónoma de Buenos Aires, con un tráfico considerable, estos eventos son una preocupación constante por su impacto en la seguridad pública, la infraestructura vial, y los servicios de emergencia.

Con una población de 3,120,612 habitantes en un área de 200 km2 según el censo de 2022, y más de 12 millones de vehículos circulando por sus autopistas en julio de 2023, la prevención de accidentes y la implementación de políticas de seguridad vial eficaces son cruciales.

## Datos
El análisis se basó en la Base de [Datos de Víctimas Fatales en Siniestros Viales](https://data.buenosaires.gob.ar/dataset/victimas-siniestros-viales), disponible en formato Excel con dos secciones: HECHOS y VÍCTIMAS, interconectadas por un ID único. Se proporcionan detalles sobre las definiciones y variables utilizadas en este documento, y los datos pueden consultarse aquí.

## Tecnologías Utilizadas
El proyecto involucró el uso de Python y Pandas para la manipulación de datos, seguido de un análisis exploratorio. Para estimar la población de 2021, se recurrio a un excel de la pagina de la ciudad de Buenos Aires en [INDEC](https://www.indec.gob.ar/indec/web/Nivel4-Tema-2-41-165). El dashboard interactivo fue desarrollado en Power BI y está disponible [aquí](./Presentación/Presentación_accidentes_CABA - MySQL.pbix)

## ETL y EDA
Inicialmente, se realizó un ETL para limpiar y preparar los datos, seguido de un análisis exploratorio detallado (EDA) para identificar patrones relevantes para la toma de decisiones. Los detalles se encuentran aquí.

Tambien recurrimos a alojar nuestro dataset en un servidor en la nube [Clever-Cloud](https://console.clever-cloud.com/), para que PowerBi consulte online y se conecte a una base de MySQL.

## Análisis de Datos
El análisis comenzó evaluando la distribución temporal de los homicidios, identificando patrones semanales y horarios significativos, y perfilando las víctimas por género, edad, y medio de transporte utilizado al momento del accidente. Se examinó también la distribución espacial de los incidentes, destacando la prevalencia de accidentes en avenidas y mas justamente en las esquinas.

## KPI
Basados en el análisis, se establecieron tres KPIs para monitorear la reducción de víctimas fatales, accidentes mortales de motociclistas, y la tasa de homicidios en avenidas
