# Notas de transformación

## Propósito
Este documento resume las transformaciones aplicadas para construir una tabla calendario reutilizable en Power Query.

## Revisión inicial en Excel
Antes de transformar la tabla, se realizó una revisión visual en Excel para:
- Verificar el orden de la columna `Fecha`.
- Confirmar consistencia en la estructura.
- Detectar posibles errores visibles antes del proceso en Power Query.

## Transformaciones en Power Query
La tabla calendario fue generada y enriquecida en Power Query mediante la creación de columnas derivadas a partir de una columna principal de fecha.

### Pasos aplicados
- Definición del rango de fechas.
- Conversión de `Fecha` al tipo fecha.
- Creación de una clave de fecha (`FechaSK`).
- Generación de columnas numéricas para análisis temporal:
  - `Año`
  - `Trimestre_Num`
  - `Mes_Num`
  - `Día_Num`
- Generación de columnas descriptivas:
  - `Trimestre`
  - `Mes`
  - `MesCorto`
  - `Día`
  - `DíaCorto`
- Generación de columnas semanales:
  - `Día_Semana_Num`
  - `Semana_Año`
  - `CierreSemana`
- Generación de columnas de agrupación:
  - `AñoTrimestre`
  - `AñoMes`
  - `AñoMesCorto`
- Generación de columnas de control mensual:
  - `InicioMes`
  - `FinMes`

## Estructura final
La tabla final quedó compuesta por las siguientes columnas:
- `Fecha`
- `FechaSK`
- `Año`
- `Trimestre_Num`
- `Mes_Num`
- `Día_Num`
- `Trimestre`
- `Mes`
- `MesCorto`
- `Día_Semana_Num`
- `Semana_Año`
- `CierreSemana`
- `Día`
- `DíaCorto`
- `AñoTrimestre`
- `AñoMes`
- `AñoMesCorto`
- `InicioMes`
- `FinMes`

## Uso en el modelo
Esta tabla no se creó como análisis independiente.  
Su función es actuar como dimensión calendario para relacionarse con otras bases del proyecto y facilitar el análisis temporal en Power BI.

## Aplicación prevista
La tabla calendario será utilizada como extensión de otras bases del portafolio, en especial la base 1 y la base 3, para mejorar jerarquías de fecha, filtros y segmentación temporal.