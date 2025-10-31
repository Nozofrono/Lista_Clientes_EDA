# 📊 Análisis Exploratorio de Datos (EDA) - Perfil Demográfico y Económico de Clientes
por: Juan Guillermo Marulanda Mesa
Este documento resume los hallazgos esenciales obtenidos del análisis de las variables demográficas (`Age`, `Educ`) y la variable económica (`Income`) de la clientela, buscando la estructura de los segmentos y sus relaciones.

### Objetivo del Análisis

El objetivo principal fue determinar si las variables demográficas básicas tienen una **correlación lineal** con el ingreso, y si las **distribuciones multimodales** de las variables pueden servir como base para una segmentación efectiva.

## 1. Distribuciones Univariadas: Estructura y Segmentos Naturales

La exploración de la forma de las distribuciones (Gráficos de Densidad) reveló una base de clientes internamente compleja.

| Variable | Característica Principal | Implicación de Segmentación | Imagen de Referencia |
| :--- | :--- | :--- | :--- |
| **Ingreso** | **Bimodal** (Dos picos claros: ~5M y ~10M) | Se recomienda segmentar en **dos grupos de valor** distintos. |  |
| **Edad** | **Multimodal y Ancha** (Picos en ~30 y ~45-50 años) | Éxito en atraer **múltiples generaciones**; estrategias deben ser cohortes específicas. |  |
| **Educación** | Multimodal | Base de clientes con diversidad de niveles de formación. |  |

---

## 2. Hallazgo Clave: Diferencias Educativas por Género

Al desagregar los años de educación por género (Histogramas), se identificaron concentraciones específicas que definen segmentos demográficos fuertes:

* **Clientes Masculinos:** La mayor concentración se encuentra en **12 años de educación**, representando un segmento de **Secundaria Completa**.
* **Clientes Femeninos:** La distribución es más dispersa, pero con una concentración más fuerte que los hombres en los **niveles educativos inferiores** (e.g., 1, 7 y 8 años).

---

## 3. Conclusión de Correlación: Independencia entre Variables

El análisis bivariado (Diagramas de Dispersión) y el resumen estadístico (Mapa de Calor) establecieron el hallazgo más crítico para el modelado:

| Relación entre Variables | Coeficiente de Correlación | Implicación Analítica |
| :--- | :--- | :--- |
| **Ingreso** vs. **Edad** | **-0.04** | **No hay correlación lineal.** Edad no predice ingreso. |
| **Ingreso** vs. **Educación** | **-0.01** | **No hay correlación lineal.** Educación no predice ingreso. |

### Implicación Estratégica

La falta de correlación lineal entre Ingreso, Edad y Educación significa que **las variables demográficas por sí solas no sirven para predecir el nivel de ingreso o valor del cliente**. La segmentación debe basarse en la **estructura de las distribuciones** (los picos identificados) y en la **composición por género**, no en una tendencia lineal simple.

---

## 4. Librerías Utilizadas

Para llevar a cabo la limpieza, el análisis estadístico y la visualización de datos, se utilizaron las siguientes librerías de Python:

* `pandas`
* `numpy`
* `seaborn`
* `matplotlib.pyplot`
