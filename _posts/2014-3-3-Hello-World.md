---
layout: post
title: INF3863-1 - Sistemas Recomendadores
---

Clase 6 - Justicia, Explicabilidad y Transparencia en Sistemas de Recomendación

Es un hecho que estamos viviendo días increíbles, con potentes avances en la inteligencia artificial. Así podemos verlo en grandes hitos como los primeros autos que lograron conducirse de manera autónoma, una IA que ha logrado vencer al campeón mundial de Go o la generación de escenas desde una imagen, por nombrar solo algunos de estos sorprendentes avances.

Si bien, estos avances son muy positivos para el desarrollo tecnológico, al mismo tiempo también nos presentan ciertos desafíos, los cuales estaremos describiendo en este resumen.

Es así como el caso de COMPAS, un sistema usado en EE. UU. para predecir la probabilidad de reincidencia de personas condenadas por delitos, han demostrado presentar ciertos sesgos raciales. De una forma similar, tenemos el caso de estudio de Joy Buolamwini, investigadora de MIT MediaLab, donde también se evidencia un peor rendimiento detectando rostros de mujeres de tez más oscura. Ciertamente en cualquier caso como estos, donde se pueda perjudicar a algún grupo de personas de manera discriminatoria, siempre será un tema delicado en este tipo de sistemas que finalmente progresan a pasos agigantados, o al menos más rápido de lo que podemos encontrar acuerdos para regular su uso y aplicaciones.

Este tipo de comportamientos no deseados en los sistemas, se pueden explicar desde el hecho en el que su rendimiento se mide por métricas, pero nadie asegura que esas métricas sean justas.

Por el mismo motivo y muchos más, grandes sistemas de recomendación como lo es el caso de YouTube han tenido que cambiar la arquitectura de su sistema varias veces durante los últimos años, para mejorar esos distintos aspectos. Dentro de sus principales desafíos tienen el hecho de no lograr diferenciar fácilmente contenido como violento o fake news de manera automática. Generalmente este tipo de problemas se resuelven con otro sistema satélite que se encarga del filtrado de contenido, que no se encuentra dentro del mismo sistema de recomendación, y compañías como Facebook, gastan millones de dólares al año intentando lidiar con estos contenidos no aptos para la plataforma, donde han tenido que solucionar muchos de esos problemas de manera manual, con personas que revisen los contenidos reportados como no aptos.

Continuando con el caso de YouTube, otro tema muy relevante es la transparencia en el contenido que se está recomendando. Entonces un ingeniero de YouTube creó un sistema que logra medir cuales son los contenidos que se están recomendando en base a una pregunta inicial utilizando un robot que realiza distintas caminatas aleatorias por el contenido, saltando de recomendación en recomendación. También existía la preocupación de si los usuarios de la plataforma realmente estaban utilizando las recomendaciones hechas por el sistema, a lo que estudios han demostrado que al menos un 75% de los usuarios en distintos rangos etarios, si lo realizan al menos de manera ocasional.

Ahora que hemos visto los casos mencionados en los párrafos anteriores. Debería importarnos la correcta evaluación de estos sistemas. Personalmente no tengo duda de que, si debería importarnos, dado que estos sistemas cada vez se utilizan para fines más relevantes en nuestras vidas.
Esta preocupación no es algo nuevo, y de hecho en algunos lugares del mundo se ha avanzado bastante en esta discusión sobre como regular en particular, el uso de los datos. En el año 2018, la Unión Europea generó una normativa llamada General Data Protection on Regulation (GDPR) que se encarga de proteger los datos de los ciudadanos y residentes de la Unión Europea y todas las compañías que allí residan o bien trabajen con datos de personas, deben garantizar su correcto uso en base a dicha legislación.

Por otra parte, el año 2019 se creó la FACCT, una conferencia donde se reúnen profesionales de distintas disciplinas para hablar sobre los impactos de estos sistemas socio-técnicos en la sociedad y realizaron un documento de principios para Accountable Algorithms, para el impacto social de estos algoritmos.

¿Cómo medir, estudiar y prevenir el sesgo en Sistemas Recomendadores? Existen algunas definiciones para tener en cuenta para lidiar con estos aspectos tales como:

•	Fairness: La propiedad de ser justo o equitativo vs. Sesgo: inclinación hacia algo; predisposición, parcialidad, prejuicio, preferencia, predilección, discriminación.
•	Accountability: Ser responsable significa ser
•	sujeto a dar cuenta o tener la obligación de informar, explicar o justificar algo -> IA explicable (XAI).
•	Transparency: Es el principio de que los factores que influir en las decisiones tomadas por los algoritmos debe ser visible, o transparente, para las personas que usan, regulan y se ven afectadas por los sistemas que emplean esos algoritmos.

Todas ellas se denominan “FAT Definitions”, un acrónimo de esas tres definiciones anteriores.

Clase 8 – Sistemas Recomendares Conversacionales

Recomendación basada en críticas 

En este tipo de sistemas, la recomendación se inicia con una propuesta inicial que es refinada a través de críticas del usuario.

¿Qué es un sistema conversacional?

Un sistema recomendador que da sugerencias personalizadas a través de diálogos en lenguaje natural con un sistema.

Una forma natural de recibir recomendaciones: 
•	Descubrir las necesidades del usuario mediante diálogos. 
•	Dar orientación en una situación particular. 

Es importante mencionar que La IA Conversacional le da más poder a los chatbots, pero no todos los chatbots están basados en IA Conversacional, por lo tanto son dos conceptos distintos que podrían estar o no relacionados.

Test de Turing

Estos sistemas se pueden medir con el Test de Turing que básicamente evalúa la capacidad de una computadora de imitar a un humano.

Framework general de un sistema conversacional 

La manera en la que tenemos más chances de conocer a un usuario es a través de su personalidad, desde lo cual estos sistemas pueden resultar de mucha ayuda para capturar dicha información.

¿Por qué́ son importantes los sistemas recomendadores conversacionales? 

•	Uso de técnicas de reinforcement learning y deep learning han permitido que estos sistemas conversacionales sean usables (no perfectos) por usuarios finales. (Alexa, Siri, etc..) 
•	Sirve para extraer de manera dinámica más feedback del usuario y patrones de uso. 
•	Más datos nos permiten mejorar más aún estos modelos conversacionales.

Formalización básica del problema Sistema recomendador conversacional

INPUT 
•	Historial de diálogos: últimas N interacciones con el sistema. 
•	[opcional] Preferencias del usuario (clicks, compras, etc..) 
•	[opcional] Información adicional de ítems (categoría, metadata) 

OUTPUT 
•	Próxima respuesta del sistema para interactuar (en turnos) 
•	Items recomendados para el usuario (una o múltiples veces) 
•	 [opcional] Una explicación de porqué está recomendando algo.

Diferentes tipos de diálogo con un sistema conversacional
 
Evaluación de la calidad de la conversación 
•	Turn-level metrics 
•	Calidad de las oraciones generadas por el chatbot (BLEU, ROUGE, legibilidad) 
•	Relevancia de preguntas generadas por el chatbot (ground truth de preguntas, accuracy, recall) 
•	Frecuencia y distribución de acciones tomadas por el chatbot (recomendar, chatear, preguntar) 
•	Nivel de cooperación del usuario (cuanto responde el usuario a las preguntas del chatbot) 
•	Dialogue-level metrics 
•	largo de los diálogos 
•	ratio diálogo satisfactorio y cumplimiento de tareas (recomendar, preguntar) 
•	Business-level metrics 
•	conversion-rate (% usuarios que hacen una acción específica) por sesión de chats 
•	incremento en ventas 
•	satisfacción del usuario, ratings, retención de clientes, lealtad de clientes, etc. 

Arquitectura modular

5 grandes módulos:
1.	Natural Language Understanding / Generation (entiende y genera diálogos) 
2.	Dialogue State Management (controla quién habla y qué acciones toma) 
3.	Sistema Recomendador 
4.	Explicación [opcional] 
5.	Knowledge (conocimiento externo)
  
Natural language understanding 

Entender lo que quiere el usuario dado el contexto e información del texto. (un área más específica de NLP) 
Dentro de los principales objetivos están: 

•	Detección de categorías de ítems 
•	Detección de atributos/aspectos de ítems 
•	Detección de intenciones del usuario 
•	Análisis de sentimientos
Estas tareas pueden ser abordadas por RNNs o Transformers.
