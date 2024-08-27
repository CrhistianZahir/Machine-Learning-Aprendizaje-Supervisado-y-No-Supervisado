# <h1 align="center"> Machine Learning, Aprendizaje Supervisado y No Supervisado</h1>

# <h1 align="center"> Satisfacción de usuarios de aerolíneas</h1>

# <h2 align="center"> Descripción del Proyecto</h2>
<p> 
Para abordar la predicción de satisfacción, se emplearon dos modelos distintos: el algoritmo de aprendizaje supervisado, Random Forest, y el algoritmo de agrupamiento no supervisado, K-means. Estos modelos ofrecen enfoques complementarios, uno centrado en la precisión de la predicción y otro en la identificación de patrones y segmentos de clientes con características similares.
Se usan herramientas como Pandas para manipular datos, junto con la aplicación de técnicas de preprocesamiento. se realiza también limpieza de datos (revisión de valores nulos y valores duplicados del dataframe, Completando los valores faltantes en la columna “Arrival Delay”,) y el análisis exploratorio de características por medio de gráficas y análisis de estos gráficos obtenidos, para identificar características que no se consideran relevantes para el estudio de caso.
</p>

# **Tabla de contenido**
**1. Objeto de estudio.**

**2. Introducción.**

**3. Descripción del problema.**

**4. Objetivos.**

**5. Descripción del conjunto de datos.**

**6. Implementación.**

**7. Importando librerías.**

**8. Limpieza de datos.**

**9. Análisis exproratorio de características.**

**10. Modelo de aprendizaje no supervisado.**

**11. Evaluación del modelo de aprendizaje no supervisado.**

**12. Modelo de aprendizaje supervisado.**

**13. Evaluación del modelo de aprendizaje supervisado**

**14. Optimización del modelo.**

**15. Conclusiones.**

**16. Referencias.**

## <p align="center">4. Objetivos</p>

**Objetivo general**

Desarrollar algoritmos de Machine Learning para analizar el nivel de satisfacción de usuarios de aerolíneas.

**Objetivos específicos**

1.Seleccionar las características del conjunto de datos que representan un impacto significativo en la satisfacción del pasajero.

2.Construir los modelos de Machine Learning a partir de las características seleccionadas con el fin de predecir la satisfacción del pasajero.

3.Evaluar el rendimiento de los modelos de Machine Learning por medio de las métricas de precisión, Recall y F1-Score.

## <p align="center">15. Conclusiones</p>

La correcta adquisición y limpieza del conjunto de datos demuestran un enfoque meticuloso en la preparación de datos para el Machine Learning. El uso de herramientas como Pandas para manipular y visualizar datos, junto con la aplicación de técnicas de preprocesamiento, garantiza la calidad y consistencia de los resultados, contribuyendo a la confiabilidad de los modelos construidos. La limpieza de datos (revisión de valores nulos y valores duplicados del dataframe, Completando los valores faltantes en la columna “Arrival Delay”,) y el análisis exploratorio de características por medio de gráficas y análisis de estos gráficos obtenidos, permitió identificar características que no se consideran relevantes para el estudio de caso, dichas características del dataframe fueron “ID, Gate Location, Gender, Flight Distance, Departure Delay y Arrival Delay”.

La implementación del algoritmo de agrupamiento K-means ofrece una perspectiva única al revelar patrones y segmentos con características similares, proporcionando insights valiosos para comprender los factores que influyen en la satisfacción del cliente. De esta implementación del modelo de aprendizaje no supervisado por medio del algoritmo de agrupamiento k-means, se observó qué, el cluster número 2 es el que tiene menor tamaño en comparación con los otros tres cluster. Se observó que, el cluster número 2 se encontró repetidamente en comparación con otras características para usuarios neutrales o insatisfechos, esto también permite concluir que hay más usuarios satisfechos a insatisfechos con los servicios prestados por las aerolíneas.

Además, de la visualización de los clusters obtenidos y de su distribución con respecto a las características del dataframe se determino que: Se observa que los cluster "3 y 2" en su mayoría están insatisfechos y tienen una edad que va desde 10 a los 28 años, y desde los 50 a los 56 años. Mientras que los usuarios satisfechos no presentan un rango de edad en específico con respecto a la distribución de los clusters. Se observa que los usuarios insatisfechos están compuestos por los clusters "2 y 3" y se encuentran distribuidos en el nivel de satisfacción con el servicio"On-board Service". El cluster "0 y 1" se encuentran en los usuarios satisfechos con el servicio de la aerolínea y el servicio "On-board Service". Se observa que el cluster "2" en su mayoría están insatisfechos y tienen un nivel de satisfacción con el servicio "Cleanliness" que oscila entre 0 y 3. Mientras que los usuarios satisfechos se presentan en los cluster "0 y 3" y tienen un nivel de satisfacción con el servicio "Cleanliness" que oscila entre 0 y 3. Se observa que el cluster "2" en su mayoría están insatisfechos y tienen un nivel de satisfacción con el servicio "Ease of Online Booking" que oscila entre 1 y 3. Mientras que los usuarios satisfechos se presentan en los cluster "0 y 1" y tienen un nivel de satisfacción con el servicio "Cleanliness" que oscila entre 0 y 5. Se observa que los cluster "2 y 3" se presentan insatisfechos y están distribuidos en el nivel de satis facción con el servicio de Check-in. Mientras que los usuarios satisfechos se presentan en los cluster "0, 1 y 3". Se observa que el cluster "2" se presenta insatisfecho y tienen un nivel de satisfacción con el servicio "Online Boarding" que oscila entre 1 a 3 y 5. Mientras que los usuarios satisfechos se presentan en el cluster "0" y tienen un nivel de satisfacción con el servicio "Online Boarding" que oscila entre 1 y 5. Se observa que el cluster "2" se presenta tanto satisfecho como insatisfecho y tienen un nivel de satisfacción con el servicio "Seat Comfort" que oscila entre 0 a 3. Se observa que el cluster "2 y 3" se presenta tanto satisfecho como insatisfecho, pero cuando esta insatisfecho tienen un nivel de satisfacción con el servicio "Leg Room Service" que oscila entre 0 a 5. Se observa que el cluster "2" se presenta como insatisfecho para el nivel de 0 a 3 con respecto al servicio "Food and Drink", y el cluster "3" se presenta como satisfecho e insatisfecho para un nivel de 4 a 5 con respecto al servicio "Food and Drink". Se observa que el cluster "2 y 3" se presenta como insatisfecho para el nivel de 0 a 4 con respecto al servicio "In-flight Service". Se observa que el cluster "2" se presenta como insatisfecho para el nivel de 0 a 3 con respecto al servicio "In-flight wifi Service". Se observa que el cluster "2" se presenta como insatisfecho para el nivel de 1 a 3 con respecto al servicio "In-flight Entertainment". Se observa que el cluster "2 y 3" se presenta como insatisfecho para el nivel de 1 a 3 y 5 con respecto al servicio "Baggage Handling".

De la implementación del algoritmo de aprendizaje supervisado por medio del algoritmo Random Forest, se obtuvo una precisión general con un valor de 96,26%, una precisión por clase de 95,61% y 97,17%, también se obtuvo un valor de Recall por clase con valor de 97,9% y 94,12%, obteniendo finalmente un F1 Score de 96,74% y 95,62%. Finalmente se realizó una optimización del modelo de aprendizaje supervisado encontrando mejores hiperparámetros y utilizando los datos de validación cruzada se alcanzó una nueva precisión con un valor de 96,44%.

Del presente estudio de caso sobre la satisfacción de usuarios de aerolíneas, se pudo observar la importancia del análisis exploratorio de características para determinar que características se pueden considerar irrelevantes o que puedan entorpecer la construcción de los modelos de machine learning. Además, se observó que, aunque, la visualización de los resultados de evaluar el rendimiento del modelo de aprendizaje no supervisado sea un proceso más largo en comparación con el modelo supervisado, se logró obtener más información que describía el comportamiento de las características del dataframe con respecto al nivel de satisfacción de los usuarios al usar los servicios de aerolíneas.

**Nota:** Dentro del Notebook "ML_Satisfaccio_Usuarios_Aerolineas.ipynb" se encuentra todo el desarrollo que se presenta en la tabla de contenido.
