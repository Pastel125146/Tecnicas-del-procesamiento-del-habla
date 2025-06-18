Resumen del Colab: Ejercicios de NER con Transformers y Gemini (en contexto argentino) Este cuaderno propone una serie de ejercicios progresivos para trabajar con reconocimiento de entidades nombradas (NER), usando modelos locales de Transformers y la API de Gemini, aplicados al contexto argentino. Se abordan desde tareas básicas hasta funciones avanzadas y un proyecto integrador.

Ejercicio 1: Personalización (BÁSICO) Se adaptan textos de ejemplo con barrios porteños (Palermo, La Boca, Recoleta) y de otras regiones del país (Mendoza, Patagonia).
El objetivo es probar si los modelos reconocen correctamente nombres de personas, lugares y organizaciones en un contexto local.

Permite observar cómo reaccionan los modelos a distintas formas de nombrar entidades típicas del español rioplatense.

Ejercicio 2: Análisis Comparativo (INTERMEDIO) Se comparan dos enfoques: modelo local de Hugging Face vs Gemini API.
Se implementa:

Función para contar entidades por tipo.

Medición de tiempo de procesamiento por modelo.

Análisis de desempeño y cobertura en dos textos.

Hallazgo clave: Transformers detecta más entidades y ofrece mayor granularidad, pero Gemini entrega resultados más limpios y rápidos.

Ejercicio 3: Extensiones Avanzadas (AVANZADO) Se desarrolla una arquitectura más robusta para tareas a gran escala:
Procesamiento en lotes de textos.

Exportación a CSV con atributos como tipo de entidad, posición y puntuación.

Filtrado por tipo de entidad (ej., solo personas).

Resultados: exportación exitosa, detección precisa de nombres comunes, aunque con algunos falsos positivos.

Proyecto Integrador: "Analizador de noticias argentinas" Se construye un prototipo que extrae personas y lugares de textos periodísticos.
Resultado: buena detección de figuras políticas (Alberto Fernández, Martín Guzmán) y localizaciones (Casa Rosada), aunque con fragmentación por el tokenizador.

Se detectan nombres compuestos como subpalabras, mostrando una limitación común del modelo basado en WordPiece.

Preguntas de Reflexión Se discuten aspectos clave:
Ventajas y desventajas de modelos locales vs API.

Evaluación de precisión con métricas estándar.

Escalabilidad mediante procesamiento distribuido.

Ética en el uso de modelos que procesan datos personales.

Conclusión general Este cuaderno es un recorrido completo y práctico sobre NER aplicado a Argentina, con enfoque técnico y reflexivo. Muestra cómo combinar herramientas locales y nube para crear soluciones analíticas con conocimiento del contexto y sensibilidad a los datos.

https://colab.research.google.com/drive/1dwjBqnACkv1CTa8sn82ZgnK-VQDBb67V
