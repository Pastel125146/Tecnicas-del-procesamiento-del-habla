En este Colab se desarrolla un micro-laboratorio práctico sobre representación vectorial de texto usando dos técnicas clave: Bolsa de Palabras (BoW) y TF-IDF. Se trabaja con un pequeño conjunto de reseñas sobre películas/documentales en español, que se procesan y analizan paso a paso.

- ¿Qué se hace?
Preprocesamiento de texto
Se limpia y normaliza cada reseña aplicando minúsculas, eliminación de signos, stopwords y stemming. El resultado son versiones simplificadas listas para vectorizar.

Creación de la Matriz BoW
Se construye una matriz donde cada fila representa una reseña y cada columna una palabra del vocabulario. Las celdas indican cuántas veces aparece cada palabra en cada reseña.

Creación de la Matriz TF-IDF
Usando el mismo vocabulario, se crea una matriz TF-IDF que no solo cuenta palabras, sino que calcula su peso informativo. Las palabras comunes entre reseñas tienen menor valor.

Análisis comparativo

Se examinan las palabras con mayor peso TF-IDF en una reseña específica para detectar las más representativas.

Se identifican palabras que aparecen mucho en BoW pero tienen bajo peso TF-IDF, lo que indica que no aportan valor diferencial al texto (por ejemplo, términos genéricos o repetidos).

- Conclusión
BoW muestra qué tan frecuentemente aparecen las palabras.

TF-IDF destaca cuáles son realmente importantes y distintivas en cada reseña.

La práctica permite ver cómo TF-IDF mejora el análisis semántico, ayudando a identificar los conceptos clave dentro de un conjunto de textos.
