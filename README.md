# Evaluación Prospectiva del Riesgo Operacional

## Descripción del proyecto

Este proyecto desarrolla una evaluación prospectiva del riesgo operacional mediante el análisis de eventos históricos y la aplicación de técnicas de analítica de datos.

El análisis parte de información relacionada con la frecuencia y severidad de eventos operacionales y busca identificar diferentes niveles de exposición al riesgo. Para ello, se integran herramientas de análisis de pérdidas operacionales, gestión del riesgo y técnicas de agrupamiento no supervisado.

El proyecto incorpora un enfoque prospectivo mediante la aplicación de un modelo de distribución de pérdidas (LDA), una estimación de la pérdida gestionada y posteriormente una segmentación de los eventos mediante K-Means.

---

## Objetivo

Evaluar de manera prospectiva la exposición al riesgo operacional a partir del comportamiento histórico de los eventos, utilizando modelos de distribución de pérdidas y técnicas de agrupamiento para identificar diferentes niveles de riesgo.

### Objetivos específicos

- Analizar el comportamiento de los eventos de riesgo operacional.
- Estimar la pérdida asociada a los eventos mediante un modelo LDA.
- Incorporar una gestión de la pérdida estimada dentro del análisis prospectivo.
- Identificar grupos de eventos con características similares.
- Clasificar los eventos de acuerdo con diferentes niveles de exposición al riesgo.
- Analizar el valor financiero asociado a la gestión del riesgo.
- Estimar el valor de captura relacionado con gases de efecto invernadero (GEI).

---

## Base de datos

El proyecto utiliza información histórica de eventos de riesgo operacional, incluyendo variables relacionadas con el comportamiento transaccional, la frecuencia de ocurrencia y las pérdidas asociadas a los eventos.

Entre las variables utilizadas durante el análisis se encuentran:

- Transacciones Diarias
- Valor Transado (millones)
- Frecuencia de eventos
- LDA
- LDA Gestionada

La información permite analizar conjuntamente la frecuencia y la severidad de los eventos para construir una evaluación de exposición al riesgo.

---

## Metodología

El desarrollo del proyecto se realizó mediante las siguientes etapas:

### 1. Preparación de los datos

Se organizó la información histórica de los eventos operacionales y se prepararon las variables necesarias para desarrollar el análisis de riesgo.

### 2. Modelación de pérdidas operacionales

Se utilizó el **Loss Distribution Approach (LDA)** para estimar la pérdida asociada al comportamiento de los eventos de riesgo operacional.

El modelo considera elementos relacionados con la frecuencia y la severidad de las pérdidas para obtener una estimación de la exposición al riesgo.

### 3. Gestión de la pérdida

A partir de la pérdida estimada mediante LDA se incorporó un componente de gestión del riesgo, permitiendo analizar el comportamiento de la pérdida después de aplicar medidas de gestión.

### 4. Análisis prospectivo

Se desarrolló una evaluación prospectiva orientada a analizar cómo podría comportarse la exposición al riesgo bajo el escenario de gestión planteado.

Este análisis permite comparar la clasificación del riesgo antes y después de considerar la gestión de las pérdidas.

### 5. Agrupamiento mediante K-Means

Se aplicó el algoritmo **K-Means** para identificar grupos de eventos con características similares.

Las variables utilizadas para el agrupamiento fueron:

- Transacciones Diarias
- Valor Transado (millones)
- Frecuencia
- LDA
- LDA Gestionada

Para el proceso de agrupamiento se realizó previamente la estandarización de las variables y se evaluó el número de clusters mediante el método del codo.

### 6. Clasificación del riesgo

Los grupos obtenidos mediante K-Means fueron utilizados para caracterizar diferentes niveles de exposición al riesgo operacional.

Posteriormente, se comparó la clasificación de los eventos antes y después de incorporar la gestión de la pérdida.

### 7. Valor financiero y captura de GEI

Finalmente, se estimó el valor financiero asociado a la gestión de los eventos y se incorporó una estimación de captura de gases de efecto invernadero (GEI) asociada al escenario analizado.

---

## Herramientas utilizadas

- **Python**
- **Google Colab**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Scikit-learn**
- **K-Means**
- **Loss Distribution Approach (LDA)**

---

## Estructura del repositorio

```text
operational-risk-prospectivity/
│
├── README.md
├── Reto_6.ipynb
│
└── data/
    └── 5. Riesgo Operacional FallasTecnológicas.xlsx
