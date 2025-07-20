Sentiment Analysis System

Autores:

José Daniel Moreno

Juan Felipe Murriel

Asigantura: Aprendizaje Automático


Este proyecto implementa varios sistemas de análisis de sentimientos en inglés. Se utiliza un conjunto de reseñas etiquetadas como positivas (+) o negativas (-), y los sistemas aprende a clasificar nuevas reseñas con base en la información aprendida.

🧠 Descripción
El flujo del proyecto es el siguiente:

Carga y preprocesamiento de datos
Se leen archivos CSV con reseñas y etiquetas, se realiza limpieza básica del texto, y se tokeniza.
Clasificador Meme
Un punto de partida

Clasificador de vocabulario
Se implementa desde cero un clasificador que asigna una etiqueta a una reseña según los tokens que contiene, ponderando con un parámetro alpha.

-Evaluación del modelo
Se evalúa la precisión, exactitud, y F1-score, comparando contra un baseline (clasificador aleatorio).

-Optimización del hiperparámetro alpha
Se usa Optuna para encontrar el valor óptimo de alpha que maximiza el F1-score del clasificador.

Modelo de Naive Bayes
Implementando desde nltk

Modelo BERT
Un modelo muy robusto para el problema

Modelo de Regresión Logística
Un clasificador clásico, no tan robusto, idóneo para el problema

⚙️ Requisitos
Instala los siguientes paquetes para ejecutar el notebook correctamente:

numpy pandas scikit-learn matplotlib seaborn optuna plotly
Requiere además:

Python 3.8+

Jupyter Notebook o entorno compatible (por ejemplo, VS Code)

🚀 Cómo ejecutar
Clona o descarga el proyecto.

Asegúrate de tener los archivos train.csv y test.csv en el mismo directorio.

Ejecuta el notebook Sentiment_Analysis.ipynb paso a paso. Algunas celdas de código pueden tomar varios minutos.

Visualiza métricas, gráficos y el mejor hiperparámetro encontrado (alpha).

📊 Análisis de resultados
F1-score optimizado para cada modelo.

Comparación de tiempo, dificultad y porcentaje de acierto de cada modelo

Una reflexión sobre el problema y su implementación.
