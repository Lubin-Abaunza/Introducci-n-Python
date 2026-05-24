# 📊 Introducción a Python para Ciencia de Datos

Este repositorio contiene un Jupyter Notebook (`IntroduccionPython.ipynb`) que sirve como una guía práctica y completa para la manipulación, limpieza, análisis y visualización de datos utilizando el ecosistema de Python, con un enfoque especial en `pandas`.

El notebook fue desarrollado como material educativo, y es ideal para quienes quieran reforzar sus habilidades en **procesamiento de datos con Python**.

---

##  Contenido del Notebook

El cuaderno está estructurado en secciones que cubren desde la importación de datos hasta la creación de tablas de frecuencia y la generación de informes estadísticos. A continuación, los temas principales:

### 1. Configuración inicial
- Personalización del directorio de trabajo con `os`.
- Importación de librerías fundamentales (`pandas`, `numpy`, `duckdb`).

### 2. Importación de datos
- Lectura de archivos Excel (`.xls`, `.xlsx`) con `pd.read_excel()`.
- Selección de hojas, rangos de celdas, y personalización de nombres y tipos de columnas.
- Lectura de archivos delimitados (`.dlm`, `.csv`, `.txt`) con `pd.read_table()`.
- Manejo de formatos de fecha, decimales (`decimal`, `thousands`), y errores comunes.

### 3. Limpieza de datos
- Eliminación de caracteres especiales en variables categóricas usando expresiones regulares.
- Normalización de texto (minúsculas, título, eliminación de espacios).
- Manejo de valores perdidos (missings) y creación de funciones para identificarlos.

### 4. Creación y transformación de variables
- Creación de nuevas columnas mediante operaciones aritméticas (`denspobl` = población / superficie).
- Clasificación de variables (`Tipo`, `Zona`) usando `apply()` y `loc`.
- Uso de `pd.cut()` para discretizar variables numéricas.

### 5. Estadísticas descriptivas
- Uso de `describe()` para variables numéricas y categóricas.
- Creación de un resumen estadístico personalizado (media, desviación, coeficiente de variación, asimetría, curtosis, percentiles, etc.).
- Cálculo de estadísticas agrupadas con `groupby()` y `agg()`.

### 6. Tablas de frecuencia
- Tablas de una y dos vías con `pd.crosstab()`.
- Funciones personalizadas (`onewayfreq`, `twowayfreq`) para mostrar frecuencias y porcentajes.
- Uso de ponderadores (`weight`) para calcular porcentajes sobre población o superficie.

### 7. Consultas y transformaciones avanzadas
- Uso de **duckdb** para realizar consultas estilo SQL directamente sobre DataFrames.
- Manipulación avanzada con `query()`, `merge()`, `concat()`, `groupby()` y `agg()`.
- Ejemplos prácticos de agregación, filtrado, ordenamiento y creación de subconjuntos.

### 8. Unión de datos
- Unión horizontal (`concat(axis=1)`) y vertical (`concat(axis=0)`).
- Comparación de resultados entre distintas formas de implementación.

### 9. Ejercicio práctico final (Datos de Brasil)
Se trabajó con una base de datos de municipios brasileños para responder preguntas como:
- ¿Cuál región tiene más/menos municipios?
- ¿Cuál es la región más homogénea/heterogénea en términos de población y superficie?
- ¿Cuáles estados tienen mayor población o superficie en municipios costeros?
- Proporción de superficie y población en municipios costeros por estado.

---

## 🛠️ Requisitos

Para ejecutar el notebook necesitas tener instalados los siguientes paquetes:

```bash
pip install pandas numpy openpyxl duckdb
