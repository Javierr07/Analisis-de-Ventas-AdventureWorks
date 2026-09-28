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


### 1.1. Rango de fechas

Se identificó el período de ventas registrado
en la base de datos.

<img width="350" height="219" alt="image" src="https://github.com/user-attachments/assets/a27ec153-5166-4ee0-b48f-07b0867e9f4d" />

---

### 1.2. Ventas totales

Se calculó el importe total de las ventas
registradas durante el período analizado.

<img width="500" height="361" alt="image" src="https://github.com/user-attachments/assets/8c4fd677-0a31-4314-a150-174b44c186ad" />


---

### 1.3. Categorías de productos

Se identificaron las categorías disponibles
en la base de datos.

<img width="500" height="281" alt="image" src="https://github.com/user-attachments/assets/6428d913-adfc-4f2c-813f-4930006011f7" />

---

### 1.4. Productos sin subcategoría

Se identificaron los productos que no tienen
una subcategoría asignada.

  <img width="450" height="472" alt="image" src="https://github.com/user-attachments/assets/68e69dff-e583-4f14-baf6-ba34b907f360" />

---

### 1.5. ventas de productos sin subcategoria

Posteriormente, se verificó si estos productos
tenían ventas registradas.

<img width="600" height="591" alt="image" src="https://github.com/user-attachments/assets/d34c2504-ec5a-4735-b413-5556bc5f797b" />



## 2. Limpieza y transformación con Power Query.

lo que realizamos con power query es lo siguiente.
- Eliminamos las columnas innesesarias para el analis.
- Correjimos los tipos de datos de cada columna para garantizar la presicion de los calculos.
- Filtramos los productos sin subcategoria ya que no cuentan con valores dentro de las ventas totales como confirmamos en las consultas SQL.
- Manejo de nulos y reemplazo de valores.

<img width="1250" height="645" alt="image" src="https://github.com/user-attachments/assets/1ce6f523-a4b0-4670-ade1-aef1001aa41c" />



## 3. Modelado de datos y creación de relaciones.

diagrama del modelado de datos en el cual realizamos las respectivas relaciones entre tablas y se genero la tabla de fechas la cual es fundamental para el manejo de fechas dentro del analisis.
<img width="1025" height="584" alt="image" src="https://github.com/user-attachments/assets/366e10ed-9a66-4a04-80e6-a1242bc6ccab" />



## 4. Definición de métricas con DAX.

Despues del proceso de Modelado de datos utilizamos Dax para obtener las KPIS nesesaria para tener un analisis completo y dinamico.

### Indicadores principales
| Indicador | Descripción |
|---|---|
| Ventas totales | Importe total de las ventas. |
| Variación interanual | Cambio porcentual respecto al año anterior |
| Ventas por categoría | Distribución de ventas por categoría |
| Top 3 meses | Meses con mayores ventas en el año |
| Total de Unidades vendidas | Suma total de los productos vendidos |

ejemplo de uso de dax dentro de Power BI.

<img width="414" height="250" alt="image" src="https://github.com/user-attachments/assets/a3ed4151-400a-46cf-9b21-79dee64758b2" />

---


## 5. Construcción del dashboard.

el dashboard esta compuesto de la siguiente manera:
- dos filtros importantes que son Año y Categoria con los que se podra filtrar las ventas por año y categoria.
- los diferentes KPIs que nos indican los datos mas relevantes como lo es, Ventas Totales, Ticket Promedio, Total Unidades Vendidas, Cantidad de Pedidos y variacion de ventas por año.
- grafico de barras el cual muestra las ventas totales por año.
- grafico de linea que muestra la evolucion de las ventas mes a mes.
- variacion de ventas interanual donde comparamos las ventas de un año con el anterior.
- el Top 3 meses mas rentables del año.
- grafico de barras en el que mostramos las ventas totales por categoria.

<img width="1250" height="630" alt="image" src="https://github.com/user-attachments/assets/6314dc55-5b66-4386-b8e7-9df5e024521c" />



## 6. Hallazgos

### Comparacion de Ventas Anuales.

los resultados nos muestran que el año 2013 fue el que mas ventas genero de todos pero hay que tener dos consideraciones

- las ventas el año 2011 fueron solo del periodo de Mayo a Diciembre por lo que comparar con los demás año seria un error debido a que las ventas fueron en un tiempo parcial del año.
- las ventas de año 2014 también fueron durante un tiempo parcial ya que solo se tienen registros desde Enero hasta Junio.

<img width="494" height="276" alt="image" src="https://github.com/user-attachments/assets/c5c6039e-bdcd-4634-8191-27d8a898165b" />

### Ventas 2011
Las ventas generadas en el 2011 nos dan los siguientes resultados.
- Ventas Totales $12.64 millones.
- los meses con mas ingresos que fueron Julio, Agosto y Octubre.
- El grafico mensual muestra claramente que es mes de inicio de las ventas fue Mayo.
- la Categoria Bikes Abarcaca el 94% de las ventas.

<img width="1253" height="634" alt="image" src="https://github.com/user-attachments/assets/7c76241c-9645-4b79-9ecf-3de1211038b1" />




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
