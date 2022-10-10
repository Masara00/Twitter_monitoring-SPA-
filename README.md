# prueba_tecnica

Con este programa queremos hacer un monitoreo de la red social twitter para predecir los sentimientos de los tweets respecto a la cuenta @TheBridge_Tech.
Para ellos hemos utilizado varias herramientas y seguido varios procesos que paso a enumerar:

1- Optención de tweets:
  - Para el minado de los datos hemos utilizado la librería de python 'twint'.
  - Estos datos han sido recopilados filtrando la busqueda por los comentarios con la palabra '@TheBridge_Tech' en las fechas comprendidas entre el 13 de Junio de 2002 y el 5 de Octubre de 2022.
    
2- Realizar un Analisis Exploratorio de Datos para ver y comprender lo datos que hemos obtenido.
    
3- Crear una base de datos SQL con dos tablas: tweets y usuarios.

4- Antes de utilizar el modelo hemos aplicado una serie de cambios a los textos para obtener una mejor eficiencia y resultado. Estos cambios han sido:
  - Quitar signos de puntuación.
  - Quitar links.
  - Quitar StopWords en español (artículos, conjunciones, preposiciones, etc...)
  - Quitar emojis.
  - Aplicar SnowballStemmer para quedarnos con la raíz de las palabras y ayudar al modelo en cuanto a eficiencia.

5- Utilizar un modelo pre entrenado para ver qué sentimientos tienen los tweets. Su clasificación es: 
  - Sentimiento positivo = 0
  - Sentimiento negativo o neutro = 1
  
6- Crear una aplicación con un endpoit al que le podamos pasar nuevos textos para que nos prediga su sentimiento.

7- Despliegue de la aplicación en 'pythoneverywhere' enlazado con nuestro repositorio de GitHub para poder acceder a ella de forma remota. 
