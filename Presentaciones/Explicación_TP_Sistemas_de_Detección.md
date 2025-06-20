Análisis Inteligente de Tickets de Soporte en E-commerce

Este proyecto aplica procesamiento de lenguaje natural (PLN), modelos LLM y visualización interactiva para automatizar el análisis de quejas, elogios y consultas en e-commerce.


-----+ Parte 1: Clasificación Automática de Tickets +-----

🔹 1. Análisis de Sentimiento (BETO)
Se usa el modelo beto-sentiment-analysis para detectar si el tono del ticket es positivo, negativo o neutral.
Resultado: 53.3% de coincidencia con las etiquetas manuales.


🔹 2. Clasificación Zero-Shot
Se emplea Recognai/zeroshot_selectra_medium para predecir la categoría del ticket sin necesidad de reentrenamiento.
Resultado: 46.7% de coincidencia con las categorías reales.


🔹 3. Comparación Manual vs. Modelo
Se analizan discrepancias entre etiquetas humanas y las predicciones automáticas para detectar áreas de mejora.


-----+ Parte 2: Extracción de Información Clave con PLN +-----

🔹 4. NER (Reconocimiento de Entidades)
Se detectan automáticamente nombres de clientes, ubicaciones y productos mencionados en los tickets usando bert-spanish-cased-finetuned-ner.


🔹 5. QA (Pregunta-Respuesta)
Con roberta-large-bne-sqac, se formulan preguntas específicas a cada ticket:
"¿Qué producto se menciona?", "¿Cuál es el problema?", etc.


🔹 6. Filtro de Ruido y Validación
Las respuestas de QA se limpian con reglas por campo (ej: validar que una ubicación no sea un verbo) y se combinan con los resultados de NER para mayor precisión.


-----+ Parte 3: Generación de Respuestas Automáticas +-----

🔹 7. Respuestas Personalizadas (LLM via Gemini)
Se generan respuestas empáticas o de agradecimiento, según el caso, usando prompts custom y el modelo gemini-2.0-flash.


🔹 8. Aplicación Gradio Interactiva
Se arma una interfaz web donde cualquier usuario puede ingresar un ticket nuevo y recibir análisis + respuesta automática.


--Conclusión General--
Este sistema demuestra cómo combinar múltiples técnicas de PLN para cubrir el ciclo completo del soporte al cliente:
- detectar emociones,
- clasificar la intención,
- extraer información clave,
- y responder con lenguaje natural.
  

https://colab.research.google.com/drive/1x-yRHcYpOqz4b18_vGpLBFHTczePgfpc#scrollTo=1synQtNNAzP_
