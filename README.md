### Propósito del análisis:

El notebook realiza un análisis de segmentación de clientes de un centro comercial. El objetivo principal es identificar grupos de clientes con características y comportamientos de gasto similares, lo cual puede ser útil para orientar estrategias de marketing y mejorar la atención al cliente.

### Datos utilizados:

Se utiliza un dataset llamado "Mall_Customers.csv" que contiene información sobre los clientes del centro comercial, incluyendo:

* `CustomerID`: Identificador único del cliente.
* `Gender`: Género del cliente.
* `Age`: Edad del cliente.
* `Annual Income (k$)`: Ingreso anual del cliente en miles de dólares.
* `Spending Score (1-100)`: Puntaje de gasto del cliente, que indica cuánto gasta en el centro comercial.

### Pasos del análisis:

1.  **Carga de datos:** Se carga el dataset en un DataFrame de pandas.
2.  **Análisis Exploratorio de Datos (EDA):** Se realiza un análisis descriptivo de los datos para entender su distribución y características principales. Esto incluye el uso de `df.describe()` para obtener estadísticas resumidas de las variables numéricas.
3.  **Visualización de datos:** Se generan histogramas y gráficos de dispersión para visualizar la distribución de las variables y las relaciones entre ellas.
4.  **Preprocesamiento de datos:** Se seleccionan las variables relevantes para la segmentación (Ingreso Anual y Puntaje de Gasto) y se estandarizan para que tengan la misma escala.
5.  **Aplicación de K-Means Clustering:** Se utiliza el algoritmo K-Means para agrupar a los clientes en diferentes clusters. Se determina el número óptimo de clusters utilizando el método del codo y el análisis del coeficiente de silueta.
6.  **Visualización de los clusters:** Se visualizan los clusters en un gráfico de dispersión para observar cómo se agrupan los clientes según su Ingreso Anual y Puntaje de Gasto.
7.  **Análisis de los clusters:** Se analizan las características de cada cluster y se les asignan etiquetas descriptivas.

### Principales clusters identificados:

* **Cluster 1:** Clientes con Ingreso Medio y Gasto Medio (40 años, ingreso medio, gasto medio).
* **Cluster 2:** Clientes con Ingreso Bajo y Gasto Alto (25 años, ingreso bajo, gasto alto).
* **Cluster 3:** Clientes con Ingreso Alto y Gasto Alto (32 años, ingreso alto, gasto alto).
* **Cluster 4:** Clientes con Ingreso Alto pero Gasto Bajo (44.4 años, ingreso alto, gasto muy bajo).

### Conclusiones y recomendaciones:

* La segmentación permite descubrir oportunidades de mejora y grupos prioritarios para diferentes estrategias de marketing.
* Los clusters 1 y 2 presentan el mayor valor potencial inmediato.
* Clusters como el 4 requieren análisis más profundo para convertirlos en clientes activos.
* Este análisis respalda decisiones más informadas en campañas publicitarias, diseño de productos y atención personalizada.
