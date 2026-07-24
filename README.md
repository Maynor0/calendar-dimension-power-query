# Tabla calendario en Excel y Power Query

## Descripción
Este proyecto documenta la construcción de una tabla calendario utilizando Excel y Power Query.  
La tabla fue diseñada como una dimensión temporal auxiliar para complementar otras bases del portafolio, especialmente la base 1 y la base 3.

## Objetivo
Crear una tabla calendario reutilizable para análisis temporal en Power BI, con columnas que permitan trabajar jerarquías de fecha, filtros y segmentación por periodos.

## Herramientas usadas
- Excel
- Power Query
- Power BI (como uso posterior dentro del modelo)

## Contenido del repositorio
- `data/TablaCalendario.xlsx`: archivo base trabajado.
- `images/calendario-excel.png`: revisión visual inicial en Excel.
- `images/calendario-power-query.png`: tabla final transformada en Power Query.
- `docs/notas-transformacion.md`: detalle técnico de los pasos aplicados.

## Enfoque del proyecto
Esta base no se presenta como dashboard independiente.  
Se construyó como una extensión del modelo de datos para enriquecer otras bases del portafolio mediante una dimensión temporal consistente.

## Resultado
Se obtuvo una tabla calendario funcional con campos de año, trimestre, mes, semana, día y columnas auxiliares para agrupación temporal.

## Uso dentro del portafolio
La tabla calendario está pensada para relacionarse con las columnas de fecha de otras bases del proyecto y facilitar:
- Jerarquías de fecha.
- Segmentadores temporales.
- Comparaciones por mes, trimestre y año.
- Orden correcto de periodos en visualizaciones.

## Nota
El detalle de las transformaciones realizadas se encuentra en `docs/notas-transformacion.md`.