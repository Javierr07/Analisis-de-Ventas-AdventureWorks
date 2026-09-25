# Análisis de ventas | AdventureWorks

## 1. Descripción
Análisis de ventas utilizando AdventureWorks 2022 para identificar kpis importantes para analizar el comportamiento yt evolucion de las ventas.

## 2. Objetivos
- relizar una analitica profunda dentro de la base de datos AdventureWorks.
- identificar las tendencias de las ventas a nivel anual y mensual.
- obtener metricas especificas que nos ayuden a responder preguntas del negocio.

## 3. Herramientas
- SQL Server: extracción y consultas.
- Power Query: limpieza y transformación.
- Power BI y DAX: modelado, métricas y visualización.

## 4. Fuente de datos
- Fuente: AdventureWorks.
- Período analizado: 05/2011 - 06/2014.
- Tablas utilizadas:
Production.Product
Production.ProductSubcategory
Production.ProductCategory
Sales.SalesOrderDetail
Sales.SalesOrderHeader

## 5. Metodología



## 1. Exploración de datos con SQL

| Período de ventas | Ventas totales |
|:---:|:---:|
| <img width="562" height="407" alt="image" src="https://github.com/user-attachments/assets/c46f4e00-b538-41c6-9c07-ff58f0464b75" />
 | <img width="350" height="248" alt="image" src="https://github.com/user-attachments/assets/b0d521d3-d615-4d17-88c8-d338bcee094f" /> |

| Categorías | Productos sin categoría |
|:---:|:---:|
| <img src="images/categorias.png" width="350"> | <img src="images/sin_categoria.png" width="350"> |



















1. Extracción de datos con SQL.

con SQL investigaremos los datos relevantes que nos datan una guia clave para extraerlos a power BI.


- rango de fecha en que se realizaron las ventas nos servira para saber que periodos estamos analizando.
  <img width="343" height="219" alt="image" src="https://github.com/user-attachments/assets/a27ec153-5166-4ee0-b48f-07b0867e9f4d" />

  --Ventas totales durante el periodo a evaluar
  

  -Categorias
  <img width="548" height="281" alt="image" src="https://github.com/user-attachments/assets/6428d913-adfc-4f2c-813f-4930006011f7" />

  -- Productos que no tienen Subcategoria.
  <img width="461" height="472" alt="image" src="https://github.com/user-attachments/assets/68e69dff-e583-4f14-baf6-ba34b907f360" />

--verificamos que los productos que no tienen subcategoria no tuvieran registros de ventas, lo cual indica que estos productos no producienron importe a las ventas totales.
<img width="646" height="591" alt="image" src="https://github.com/user-attachments/assets/d34c2504-ec5a-4735-b413-5556bc5f797b" />






2. Limpieza y transformación con Power Query.
3. Modelado de datos y creación de relaciones.
4. Definición de métricas con DAX.
5. Construcción del dashboard.
6. Interpretación de los resultados.

## 6. Indicadores principales
| Indicador | Descripción |
|---|---|
| Ventas totales | Importe total de ventas |
| Variación interanual | Cambio porcentual respecto al año anterior |
| Ventas por categoría | Distribución de ventas por categoría |
| Top 3 meses | Meses con mayores ventas |

## 7. Dashboard
![Dashboard de ventas](images/dashboard.png)

El dashboard permite filtrar los resultados por año y categoría y comparar las ventas entre períodos.

## 8. Hallazgos
1. **[Hallazgo 1]:** [Dato que lo respalda].
2. **[Hallazgo 2]:** [Dato que lo respalda].
3. **[Hallazgo 3]:** [Dato que lo respalda].

## 9. Conclusiones
[Explica qué indican los resultados, sus limitaciones y qué decisiones podrían apoyar.]

## 10. Archivos del proyecto
- `sql/`: consultas SQL.
- `powerbi/`: dashboard de Power BI.
- `images/`: capturas.
- `docs/`: documentación adicional.

## 11. Autor
[Tu nombre] — [Enlace a LinkedIn]
