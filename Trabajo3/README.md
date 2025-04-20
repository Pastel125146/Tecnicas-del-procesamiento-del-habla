Análisis de Texto y Datos de un Artículo de Economipedia

Este proyecto combina Web Scraping, procesamiento de texto (NLP) y análisis visual para estudiar un artículo de Economipedia sobre las empresas más grandes del mundo en 2024.

¿Qué se hizo?
+ Extracción del artículo y tabla desde Economipedia (con requests, BeautifulSoup y pandas).
+ Limpieza y análisis del texto narrativo: eliminación de caracteres especiales, lematización, tokenización y eliminación de stopwords.
+ Vectorización para análisis de frecuencias.
+ Visualización: nube de palabras, gráficos por país, sector y distribución de empresas.

--Objetivo--
Analizar tanto el contenido narrativo como los datos estructurados del artículo como para cosas del tipo:

¿Qué palabras son más frecuentes en el texto?

¿Qué países dominan el ranking?

¿Qué sectores están más representados?

¿Cómo se distribuyen las empresas en el top 100?



-----+ Parte 1: Análisis del Texto Narrativo +-----
🔹 1. Web Scraping
Se extrae el texto principal del artículo desde una página web mediante requests y BeautifulSoup.

🔹 2. Preprocesamiento del texto
Se limpia el texto eliminando signos de puntuación, stopwords, etc.

🔹 3. Lematización
Se usa spaCy para reducir las palabras a su forma base y unificar términos.

🔹 4. Vectorización
Se transforma el texto lematizado en una representación numérica (TF-IDF o Bag of Words).

🔹 5. Visualización
Gráfico de barras con las palabras más frecuentes.

WordCloud para ver los conceptos clave visualmente.

-----+ Parte 2: Extracción y Análisis de la Tabla de Empresas +-----

🔹 6. Extracción de tabla
Se detecta y extrae la tabla del ranking desde el mismo artículo web utilizando BeautifulSoup y pandas.read_html().

🔹 7. Limpieza de datos
Se renombran columnas.

Se corrigen tipos de datos (por ejemplo, convertir capitalización bursátil a números).

Se eliminan valores nulos o inconsistentes.

🔹 8. Análisis exploratorio
Se realizan distintos análisis sobre la tabla:

Empresas con mayor capitalización.

Distribución por país.

Distribución por sector.

Comparación entre continentes o regiones.

Promedios y estadísticas generales.

🔹 9. Visualización de datos
Gráficos de barras y torta (pie charts) para mostrar:

Qué países tienen más empresas en el ranking.

Qué sectores dominan el top 10.

Comparaciones entre capitalizaciones.

--Conclusión General--
+ Este trabajo demuestra cómo se pueden unir datos no estructurados (texto) y datos estructurados (tabla) para generar un análisis integral.
+ A través del texto, entendemos el contexto global del ranking y los temas más mencionados.
+ Con los datos estructurados, obtenemos información precisa, visual y comparativa entre empresas, países y sectores.
+ En conjunto, ofrecen una visión completa del panorama económico empresarial mundial en 2024.



