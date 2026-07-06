# Proyecto Final - Analisis Exploratorio de Datos (EDA)

## Tema
Analisis exploratorio de ventas y rentabilidad usando el dataset **Sample Superstore**.

## Objetivo
Transformar un conjunto de datos comercial en hallazgos accionables mediante un flujo profesional de EDA con Python.

## Dataset
- Archivo original: `dataset/SampleSuperstore.csv`
- Registros originales: 9994
- Columnas originales: 13
- Archivo limpio generado: `dataset/SampleSuperstore_limpio.csv`

## Herramientas utilizadas
- Python
- NumPy
- Pandas
- Matplotlib

## Estructura del proyecto

```text
proyecto_eda/
├── dataset/
│   ├── SampleSuperstore.csv
│   └── SampleSuperstore_limpio.csv
├── graficos/
│   ├── 01_ventas_categoria.png
│   ├── 02_utilidad_region.png
│   ├── 03_subcategorias_menor_utilidad.png
│   ├── 04_descuento_vs_utilidad.png
│   ├── 05_histograma_ventas.png
│   ├── 06_boxplot_utilidad_categoria.png
│   ├── 07_top_estados_ventas.png
│   └── 08_tendencia_temporal.png
├── notebook/
│   └── proyecto_eda_superstore.ipynb
├── README.md
└── informe_ejecutivo_eda_superstore.pdf
```

## Preguntas de investigacion
1. Que categoria genera mayores ventas?
2. Que subcategoria es mas rentable y cual genera perdidas?
3. Que region produce mayor utilidad?
4. Que estados lideran las ventas?
5. Como afecta el descuento a la utilidad?

## Metodologia
1. Carga y exploracion inicial del dataset.
2. Limpieza de datos: normalizacion de columnas, textos y eliminacion de duplicados.
3. Ingenieria de caracteristicas: margen, venta promedio por unidad y fecha estimada.
4. Analisis descriptivo con `groupby` y `pivot_table`.
5. Visualizacion con Matplotlib.
6. Redaccion de conclusiones y recomendaciones de negocio.

## Como ejecutar
1. Abrir el archivo `notebook/proyecto_eda_superstore.ipynb` en Jupyter Notebook o Google Colab.
2. Verificar que el archivo `dataset/SampleSuperstore.csv` este en la carpeta correcta.
3. Ejecutar las celdas en orden.

## Principales resultados
- Ventas totales: $2,296,195.59
- Utilidad total: $286,241.42
- Margen total: 12.47%
- Registros procesados despues de limpieza: 9977

## Nota tecnica
La version del dataset utilizada no incluye una columna de fecha original. Para cubrir el componente temporal del proyecto academico, se genero una variable `Fecha_Estimada` basada en el orden de los registros.
