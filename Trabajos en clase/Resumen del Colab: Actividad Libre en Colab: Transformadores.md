🧁 Resumen de la Actividad Libre en Colab: Aplicaciones con Hugging Face (Postres y Cocina)

En esta actividad exploratoria, se utilizan distintos pipelines de Hugging Face aplicados a textos con temática gastronómica (especialmente postres), para probar capacidades y límites de modelos de PLN en español. Las pruebas se organizan en cuatro mini-experimentos:

1. Análisis de Sentimiento con sarcasmo y jerga
Se prueban frases coloquiales y sarcásticas relacionadas con postres, como:

“Riquísimo el flan, si te gusta el gusto a cartón mojado.”

El modelo BETO analiza el sentimiento. Resultado: la mayoría de las frases se clasifican como positivas, incluso las sarcásticas, lo que evidencia que el modelo no siempre detecta la ironía con precisión.

2. Resumen de un artículo de Wikipedia
Se resume un texto sobre la chocotorta argentina usando un modelo mT5 multilingüe.
Resultado: el modelo genera un resumen claro y conciso que captura la esencia del texto original (ingredientes, historia y facilidad de preparación del postre).

3. Traducción de frases técnicas y poéticas
Se traduce del español al inglés una frase técnica (“emulsión de mayonesa”) y otra poética (“el merengue debe sostener tus sueños”).
Resultado: el modelo Helsinki-NLP/opus-mt-es-en mantiene el estilo de cada frase, mostrando buena adaptación tanto a registros técnicos como metafóricos.

4. Generación de texto formal vs. informal
Se le pide a un modelo GPT-2 en español completar frases con tono formal (“Para lograr una mousse perfecta…”) e informal (“Si querés que la mousse te quede piola…”).
Resultado: el modelo genera salidas que diferencian el tono, aunque no siempre son coherentes con el tema cocina (por ejemplo, “es fundamental contar con un buen calzado”).

-- Conclusión general:
Esta actividad demuestra cómo los modelos pueden adaptarse a distintos estilos y tareas, pero también revela limitaciones, como dificultades con el sarcasmo o coherencia temática. Ideal para explorar creativamente las capacidades del PLN en español.
