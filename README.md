# Aprendizaje_Automatico_Parcial_2026

##  Predicción de Precios de Alquileres en Río Grande

### Autor

**Lionel Alfredo Martínez**
Tecnicatura Superior en Ciencias de Datos e Inteligencia Artificial

Link del video presentacion: https://youtu.be/I9ejc0LsFcc

---

# Descripción del Proyecto

Este proyecto tiene como objetivo desarrollar un modelo de Aprendizaje Automático capaz de estimar el precio mensual de alquiler de propiedades ubicadas en la ciudad de Río Grande, Tierra del Fuego.

Para ello se construyó un dataset propio a partir de publicaciones inmobiliarias reales obtenidas de diferentes portales y sitios web locales.

El problema fue abordado como una tarea de **Aprendizaje Supervisado de tipo Regresión**, utilizando diferentes algoritmos para comparar su desempeño y seleccionar el modelo más preciso.

---

# Objetivos

## Objetivo General

Desarrollar un modelo predictivo capaz de estimar el precio de alquiler de una propiedad en Río Grande utilizando características relevantes del inmueble.

## Objetivos Específicos

* Construir un dataset representativo del mercado inmobiliario local.
* Realizar tareas de limpieza y normalización de datos.
* Desarrollar un análisis exploratorio de datos (EDA).
* Entrenar modelos de regresión utilizando Scikit-Learn.
* Comparar el desempeño de los modelos mediante métricas estadísticas.
* Identificar las variables con mayor influencia sobre el precio de alquiler.

---

# Origen de los Datos

Los datos fueron obtenidos mediante relevamiento manual de publicaciones inmobiliarias de Río Grande.

Fuentes consultadas:

* Mercado Libre Inmuebles
* Argenprop
* Inmobiliaria Latitud
* Mac Rae Propiedades
* Grupo Inversión

Los registros fueron recopilados entre mayo y junio de 2026.

---

# Dataset

El conjunto de datos final contiene:

* **167 registros**
* **20 variables**

Variables principales:

* Barrio
* Ambientes
* Metros²
* Tipo_propiedad
* Amoblado
* Antigüedad
* Baños
* Cochera
* Mascotas_permitidas
* Expensas_incluidas
* Latitud
* Longitud
* Precio (variable objetivo)

---

# Análisis Exploratorio de Datos (EDA)

Durante el análisis exploratorio se estudiaron:

* Distribución de precios de alquiler.
* Precio según tipo de propiedad.
* Relación entre superficie y precio.
* Precio promedio por barrio.
* Estadísticas descriptivas generales.

Principales hallazgos:

* Existe una relación positiva entre superficie y precio.
* Las casas presentan los alquileres promedio más elevados.
* Los barrios Barrancas, Mutual y Profesional registran algunos de los valores promedio más altos.
* Los precios presentan una distribución asimétrica positiva.

---

# Modelos Implementados

Se evaluaron tres modelos de regresión:

## 1. Regresión Lineal

Modelo base utilizado para establecer una referencia inicial.

## 2. Árbol de Decisión

Permite capturar relaciones no lineales entre variables.

## 3. Random Forest

Modelo basado en múltiples árboles de decisión que mejora la precisión y reduce el sobreajuste.

---

# Resultados

| Modelo            | MAE     | RMSE    | R²    |
| ----------------- | ------- | ------- | ----- |
| Regresión Lineal  | 127.095 | 186.998 | 0.757 |
| Árbol de Decisión | 75.588  | 148.492 | 0.847 |
| Random Forest     | 74.630  | 109.781 | 0.916 |

---

# Mejor Modelo

### Random Forest

Resultados obtenidos:

* MAE = 74.630
* RMSE = 109.781
* R² = 0.916

El modelo logró explicar aproximadamente el 91,6% de la variabilidad observada en los precios de alquiler, obteniendo el mejor desempeño general del estudio.

---

# Tecnologías Utilizadas

* Python 3
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Google Colab
* GitHub

---

# Estructura del Repositorio

Aprendizaje_Automatico_Parcial_2026/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   ├── Alquileres_RioGrande.ipynb
│   └── Alquileres_RioGrande_Final.ipynb
│
├── reports/
│   ├── Informe Tecnico.docx
│   ├── Diccionario de Datos.docx
│   └── Presentacion_proyecto.md
│
├── references/
│   ├── Programa Aprendizaje Automático 2026.pdf
│   ├── Rúbrica de Evaluación.pdf
│   └── Lineamientos generales.pdf
│
├── src/
│   └── .gitkeep
│
├── requirements.txt
└── README.md

---

# Conclusiones

Los resultados obtenidos demuestran que es posible construir modelos predictivos confiables para estimar precios de alquiler a partir de variables inmobiliarias relevantes.

El modelo Random Forest presentó el mejor desempeño, alcanzando un coeficiente de determinación de 0.916 y los menores errores de predicción.

Estos resultados permiten disponer de una herramienta de apoyo para la toma de decisiones dentro del mercado inmobiliario local.

Una limitación importante del proyecto es el tamaño del conjunto de datos. Al contar con 167 registros, los resultados obtenidos deben interpretarse con cautela, ya que una muestra más amplia podría mejorar la capacidad de generalización de los modelos.
---

# Trabajo Futuro

Como posibles mejoras futuras se propone:

* Incrementar el tamaño del dataset.
* Incorporar nuevas variables relacionadas con servicios y ubicación.
* Automatizar la actualización de datos.
* Evaluar modelos avanzados como Gradient Boosting y XGBoost.

---

# Repositorio GitHub

Proyecto desarrollado para la materia **Aprendizaje Automático 2026** utilizando la metodología de trabajo propuesta por la cátedra y la estructura basada en Cookiecutter Data Science.


