# Challenge 1

## Propósito del análisis

Este proyecto tiene como objetivo analizar el desempeño de cuatro tiendas a partir de sus datos de ventas, calificaciones y costos logísticos, utilizando exclusivamente **Python** y la librería **Pandas**.

El análisis busca responder una pregunta de negocio concreta: **¿qué tienda debería cerrarse?** Para ello, se evaluaron cinco frentes principales:

- **Facturación total por tienda**
- **Ventas por categoría**
- **Calificación promedio de los clientes**
- **Productos más y menos vendidos**
- **Costo de envío promedio**

Con base en estos indicadores, se identificó cuál tienda presenta el desempeño más bajo en términos generales.

---

## Estructura del proyecto y organización de archivos

Una organización recomendada para el repositorio es la siguiente:

```bash
challenge1-analisis-tiendas/
│
├── Challenge1_FM.ipynb   # Notebook principal con todo el análisis
├── README.md             # Descripción del proyecto
├── tienda_1.csv          # Datos de la Tienda 1 (opcional en repo si se usan URLs)
├── tienda_2.csv          # Datos de la Tienda 2 (opcional en repo si se usan URLs)
├── tienda_3.csv          # Datos de la Tienda 3 (opcional en repo si se usan URLs)
└── tienda_4.csv          # Datos de la Tienda 4 (opcional en repo si se usan URLs)
```

### Contenido del notebook

El notebook `Challenge1_FM.ipynb` está organizado por secciones:

1. **Importación de datos**
2. **Análisis de facturación**
3. **Ventas por categoría**
4. **Calificación promedio de la tienda**
5. **Productos más y menos vendidos**
6. **Envío promedio por tienda**
7. **Comparación final y conclusión**

> Nota: el notebook carga los datos desde las URLs originales del reto, por lo que los archivos CSV dentro del repositorio son opcionales si deseas mantener una copia local.

---

## Ejemplos de gráficos e insights obtenidos

Aunque el notebook actual se centra en tablas y resúmenes con Pandas, los resultados pueden representarse fácilmente con gráficos como los siguientes:

### 1. Gráfico de barras: facturación total por tienda
Este gráfico permite comparar los ingresos totales de cada tienda.

**Insight obtenido:**
- **Tienda 1** presentó la mayor facturación con **$1,150,880,400.00**.
- **Tienda 4** registró la menor facturación con **$1,038,375,700.00**.
- La menor facturación de la Tienda 4 fue una de las señales más importantes para considerarla como candidata a cierre.

### 2. Gráfico de barras apiladas: ventas por categoría
Este gráfico muestra el peso de cada categoría dentro de cada tienda.

**Insights obtenidos:**
- En las cuatro tiendas, la categoría con mayor impacto económico fue **Electrónicos**.
- La categoría **Muebles** también mostró alta participación en volumen de ventas.
- A pesar de tener un comportamiento similar por categoría, la **Tienda 4** quedó por debajo del resto en el consolidado general.

### 3. Gráfico de barras: calificación promedio por tienda
Permite comparar la satisfacción promedio de los clientes.

**Insights obtenidos:**
- **Tienda 3** obtuvo la mejor calificación promedio con **4.05**.
- **Tienda 1** obtuvo la menor calificación promedio con **3.98**.
- **Tienda 4** no tuvo la peor calificación, pero tampoco lideró este indicador, por lo que no compensó su menor facturación.

### 4. Gráfico de barras: costo de envío promedio por tienda
Este gráfico ayuda a comparar la eficiencia logística.

**Insights obtenidos:**
- **Tienda 4** tuvo el menor costo de envío promedio con **$23,459.46**.
- **Tienda 1** tuvo el mayor costo de envío promedio con **$26,018.61**.
- Aunque la Tienda 4 fue más eficiente en este aspecto, esta ventaja no fue suficiente para superar su bajo desempeño en ingresos.

### 5. Tabla o gráfico de ranking: productos más y menos vendidos
Este análisis permite identificar productos destacados y con baja rotación.

**Ejemplos encontrados:**
- En **Tienda 1**, los productos más vendidos fueron **Microondas**, **TV LED UHD 4K** y **Armario**.
- En **Tienda 2**, el producto más vendido fue **Iniciando en programación**.
- En **Tienda 3**, el producto más vendido fue **Kit de bancas**.
- En **Tienda 4**, el producto más vendido fue **Cama box**.

### Conclusión general del análisis
Después de comparar todos los indicadores, la tienda con menor desempeño global fue la **Tienda 4**. Aunque presentó el menor costo de envío promedio, también registró la **facturación total más baja**, por lo que se concluye que es la mejor candidata para ser cerrada.

---

## Instrucciones para ejecutar el notebook

### Opción 1: Google Colab
1. Abre Google Colab.
2. Sube el archivo `Challenge1_FM.ipynb`.
3. Ejecuta las celdas en orden, desde la importación de datos hasta la conclusión final.
4. No es necesario descargar los CSV si se mantienen las URLs originales en el notebook.

### Opción 2: Jupyter Notebook en local
1. Asegúrate de tener instalado **Python 3**.
2. Instala las dependencias necesarias:

```bash
pip install pandas notebook
```

3. Abre una terminal en la carpeta del proyecto.
4. Ejecuta Jupyter Notebook:

```bash
jupyter notebook
```

5. Abre el archivo `Challenge1_FM.ipynb`.
6. Ejecuta todas las celdas en orden.

---

## Tecnologías utilizadas

- **Python 3**
- **Pandas**
- **Jupyter Notebook / Google Colab**

---

## Autor

Proyecto desarrollado como parte del **Challenge 1 de Data Science LATAM**, utilizando análisis de datos con Pandas para apoyar la toma de decisiones de negocio.
