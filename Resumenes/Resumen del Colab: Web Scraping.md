Proyecto de Web Scraping y Procesamiento de Texto
Este proyecto tiene como objetivo aplicar técnicas de web scraping y procesamiento de lenguaje natural (PLN) en dos casos diferentes. Utiliza BeautifulSoup, requests, NLTK, WordCloud, entre otras librerías de Python, para extraer datos de páginas web, analizarlos y visualizarlos.

Caso 1: Análisis de una Receta de Empanadas Santiagueñas
Presentación:
Este caso se centra en la extracción y análisis del texto de una receta de empanadas santiagueñas obtenida desde un blog de cocina. El objetivo es explorar el contenido de la receta, identificar palabras clave, visualizar ingredientes importantes y realizar una limpieza de texto orientada al análisis semántico y nutricional básico.

¿Qué se logró con este código?
Web Scraping: Se extrajo automáticamente el contenido HTML desde la página de una receta de empanadas santiagueñas.

Procesamiento de texto: Se limpió el texto, eliminando puntuación, palabras vacías (stopwords) y términos irrelevantes.

Exploración semántica: Se contaron menciones de palabras clave como “empanada”, “carne”, “cebolla”, etc., lo que permite una primera lectura de los ingredientes o ideas más importantes.

Visualización: Se generaron tres nubes de palabras:

Un general.
Una con colores personalizados.
Una filtrada con solo palabras significativas.
Análisis nutricional básico: Se agregó una sección que cuenta menciones de ingredientes clave, útiles para análisis alimentario o enfoque en contenido.

Caso 2: Extracción de Contenido desde StackOverflow
Presentación:
Este caso demuestra cómo automatizar la extracción de contenido útil desde una página de preguntas y respuestas técnicas como StackOverflow. El objetivo es capturar tanto la pregunta principal como la primera respuesta, lo cual puede servir para bases de datos de conocimiento o para análisis de patrones en respuestas.

¿Qué se logró con este código?
Scraping de StackOverflow: Vea el contenido de una pregunta específica y su primera respuesta desde la versión en español de StackOverflow.

Limpieza básica: Se limpiaron espacios innecesarios y se mostró el contenido en forma clara y directa.

Extracción dirigida: Se utilizaron selectores HTML específicos para localizar el cuerpo de la pregunta y la respuesta.

Requisitos
Python 3.x
solicitudes
beautifulsoup4
nltk
nube de palabras
matplotlib
Almohada
