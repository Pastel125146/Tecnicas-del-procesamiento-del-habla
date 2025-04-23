# Tecnicas-del-procesamiento-del-habla

Trabajo 1: Web Scraping de recetas y página de preguntas

+ En el primer trabajo escrapeé una receta de empanadas santigueñas para extraer el titulo y los ingredientes. (herramientas usadas: requests y BeautifulSoup)
+ Luego limpié el texto, sacando símbolos innecesarios y espacios de más.
+ Después conté la frecuencia de palabras clave (ingredientes) que aparecían en la receta y generé una nube de palabras como visualización. Esto me ayudó a ver qué términos eran más importantes en el texto.
  
**Este trabajo no aplica todavía técnicas de PLN, pero fue el primer paso para conseguir el texto con el que después sí vamos a trabajar.**

+ También practiqué con otra página, esta vez de preguntas y respuestas. Hice Web Scraping para extraer la pregunta principal y la primera respuesta de la página.
  
**Este ejercicio sirvió para aprender cómo está estructurado el HTML, cómo buscar etiquetas específicas y cómo navegar por el contenido de una web.**

----------------------------------------------------------------------

Trabajo 2: spaCy con receta de pizza

En el segundo trabajo seguí trayendo una receta (esta vez de pizza), pero ahora sí usé herramientas del PLN.
Trabajé con spaCy, que no es una técnica, sino una herramienta de Python que entiende el lenguaje humano para analizar textos

Vimos varias cosas que podemos hacer con SpaCy:

+ Dividir el texto en oraciones

+ Separar cada palabra (tokenización)

+ Cambiar las palabras a su forma base (lematización)

+ Saber qué tipo de palabra es cada una (sustantivo, verbo, adjetivo, etc.)

+ Detectar nombres de cosas como cantidades o ingredientes (entidades nombradas)

**Este ejercicio sirvió para aprender a mirar un texto no solo como palabras, sino entender cómo está formado y qué información tiene.**

