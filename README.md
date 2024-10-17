## Hi there 👋

<!--
**Franklinj900/Franklinj900** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
# Proyecto de Ciencia de Datos: Análisis de Sentimientos en Reseñas de Películas

**Descripción:**

Este proyecto tiene como objetivo analizar el sentimiento de las reseñas de películas utilizando técnicas de procesamiento de lenguaje natural (NLP) y aprendizaje automático. Se emplearán modelos de clasificación para determinar si una reseña es positiva, negativa o neutral.

**Tecnologías Utilizadas:**

* **Python:** Lenguaje de programación principal.
* **NLTK:** Kit de herramientas para el procesamiento de lenguaje natural.
* **Pandas:** Biblioteca para manipulación y análisis de datos.
* **Scikit-learn:** Biblioteca para aprendizaje automático.
* **TensorFlow/Keras:** Framework para aprendizaje profundo (opcional, si se utilizan modelos más complejos).

**Estructura del Proyecto:**

* **data:** Contiene los datos crudos y preprocesados.
* **notebooks:** Jupyter Notebooks con el código para cada etapa del proyecto.
* **models:** Modelos entrenados.
* **src:** Código fuente de las funciones y clases personalizadas.

**Ejemplo de Código:**

```python
import pandas as pd
import nltk
from nltk.sentiment.vader import SentimentIntensityAnalyzer

# Cargar los datos
df = pd.read_csv('data/reviews.csv')

# Crear un analizador de sentimientos
sia = SentimentIntensityAnalyzer()

# Calcular el sentimiento compuesto para cada reseña
df['sentiment'] = df['review'].apply(lambda x: sia.polarity_scores(x)['compound'])

# Visualizar los resultados
print(df.head())
