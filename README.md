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

lo que realizamos con power query es lo siguiente
- eliminar las columnas que no son utiles dentro del analis.
- correjimos los tipos de datos de cada columna para evitar errores de calculo.
- eliminamos los productos sin subcategoria ya que no son relevantes dentro del analisis.
- manejo de nulos y reemplazo de valores.

<img width="1250" height="645" alt="image" src="https://github.com/user-attachments/assets/1ce6f523-a4b0-4670-ade1-aef1001aa41c" />



## 3. Modelado de datos y creación de relaciones.

diagrama del modelado de datos con sus respectivas relaciones.
<img width="1025" height="584" alt="image" src="https://github.com/user-attachments/assets/366e10ed-9a66-4a04-80e6-a1242bc6ccab" />





## 4. Definición de métricas con DAX.
## 5. Construcción del dashboard.
## 6. Interpretación de los resultados.

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
