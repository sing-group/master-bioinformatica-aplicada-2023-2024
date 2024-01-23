# Machine Learning en Bioinformática

> Máster en Bioinformática Aplicada a Medicina Personalizada y Salud (Curso 2023-2024)

## Proyecto de Machine Learning

Objectivos principales y pasos a seguir:

1- Búsqueda de un conjunto de datos relacionados con la bioinformática/biomedicina/medicina.

- Buscador de conjuntos de datos [Google Dataset Search](https://datasetsearch.research.google.com/).
- Herramientas para buscar conjuntos de datos como [Kaagle](https://www.kaggle.com/datasets).
- Iniciativa de datos abiertos del [Gobierno de España](https://datos.gob.es/es).
- Repositorio [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets.php).

2- Identificación de la/s tarea/s de Machine Learning a abordar (regresión o clasificación) con el conjunto de datos seleccionado.

3- Análisis exploratorio de los datos para observar si es necesario:

- Reducción del conjunto de datos, por ejemplo, eliminando columnas innecesarias.
- Eliminación de valores nulos y/o repetidos.
- Identificación de datos adicionales.
- Transformación o descomposición de datos.

**HITO-1**: Presentación en la clase del día **14 de febrero** explicando el tipo de problema que se pretende abordar junto el conjunto de datos seleccionado, así como un pequeño estudio de los atributos de ese conjunto de datos. Cada grupo tendrá como **máximo 8 minutos**.

4- Preparación de los datos, por ejemplo, entre otras muchas técnicas:

- Limpieza de datos (*outliers* o *missing values*, etc).
- Integración de datos, en el caso de tener que unir diferentes base de datos para la creación del conjunto de datos.
- Balanceo de datos.
- Selección de características.
- Discretización de variables continuas.
- Estudio de correlaciones entre variables.
  
5- Elección del(os) modelo(s) de aprendizaje. Investigar cuál es el modelo más apropiado para el problema planteado, teniendo en cuenta parámetros como *(i)* tiempos de procesamiento para su ejecución en tiempo real o no, *(ii)*  rendimiento predictivo del modelo, *(iii)* requisitos de memoria durante el entrenamiento, etc. También es posible seleccionar varios modelos o algoritmos para hacer comparativas tanto en métricas de rendimiento como en tiempos de ejecución, incluso, teniendo como referencia una publicación existente.

6- Entrenamiento y validación del(os) modelo(s). Consiste en dividir el conjunto de datos, asegurándose de que los datos de entrenamiento, validación y test no se mezclen entre las particiones, para llevar a cabo el entrenamiento del(os) modelo(s) y obtener las métricas de validación. Dependiendo del volumen de datos, quizás hay que emplear una validación cruzada de los datos.

7- Interpretación de los resultados y ajustar o modificar el modelo de aprendizaje. Hay que asegurarse de que el modelo ha aprendido algún patrón teniendo en cuenta los datos de entrada y que es capaz de generalizar, es decir, que no se produzca *overfitting*. Si esto sucediera, se debe analizar el problema y plantear una posible solución.

**HITO-2**: Presentación en la clase del día **28 de febrero** de los resultados obtenidos, explicando brevemente el trabajo realizado para la consecución de los mismos, incluyendo problemas detectados y estrategias empleadas. Cada grupo tendrá **máximo 15 minutos**.


### **Composición de grupos de trabajo**

Los grupos estarán formados por 3 o 4 personas.

### **Exposiciones de trabajo**

Los requisitos a tener en cuenta durante las exposiciones son:

- Ajustarse al tiempo disponible. En caso de exceder la duración, se detendrá la presentación.
- Elaborar diapositivas que apoyen el discurso para facilitar la comprensión del problema planteado.
- No es necesario que expongan todos los miembros del grupo, pero no puede repetir la presentación la misma persona, es decir, si un miembro ya ha realizado la primera presentación, no podrá realizar la segunda.
- Pueden efectuarse preguntas a la finalización de cada exposición.

### **Rúbrica de evaluación**


| **Ítem**                                    | **Descripción**                                                                                                                                                                            | **Valoración** |
| ------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------- |
| Presentación del trabajo                    | Exponer el trabajo realizado. En caso de partir de código existente (de Kaggle, del notebook de prácticas, etc.) se debe aclarar las contribuciones o adaptaciones aportadas.              | 3 puntos        |
| Aplicación de técnicas y algoritmos         | Emplear diferentes técnicas de preprocesamiento de datos, ejecución/selección de diferente/s model/os y uso correcto de métricas de evaluación.                                            | 1 punto        |
| Justificación de las decisiones             | Explicación razonada de los motivos que llevaron a tomar ciertas decisiones (p. ej.: no tener en cuenta algunas columnas o *features*, la conversión de los valores de una columna, etc.) y respuesta adecuada en posibles preguntas. | 2 puntos        |
| Interpretación de los resultados            | Ser capaces de transmitir e interpretar los resultados obtenidos (sean estos buenos o malos). Análisis adecuado de los resultados obtenidos y respuesta adecuada en posibles preguntas.                                             | 2 puntos        |
| Identificación de trabajo futuro            | Exposición de posibles vías de trabajo futuras (p. ej.: tareas interesantes que no dio tiempo a hacer, etc.).                                                                              | 1 punto        |
| Contribución individual de cada miembro del grupo                      | Valoración individual de cada miembro del grupo según la aportación, sin perjuicio de que la ausencia total de participación implique la expulsión automática de ese individuo.                                                                                 | 1 punto        |