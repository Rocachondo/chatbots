# chatbots

## Bot de información turística 
- Laurita es el primer bot desarrollado en base al tutorial de Steve Worwick. 
- Es con el que fui aprendiendo y probando posibles opciones de desarrollo.
- En principio se desarrolló todo el contenido en el udc.aiml, pero se fueron empleando otros archivos para los sinónimos y otras opciones.
- En cada .aiml hay un pequeño índice para darles una estructura, así como comentarios que explican las diferentes funciones.
- El bot tiene personalidad propia, alegre y simpática, así como un par de filtros de lenguaje.
- El bot estuvo unos cuantos días desplegado de forma pública en pandorabots, por lo que pude hacer mejoras sustanciales en su comprensión del lenguaje.
- Es capaz de entender correctamente los contextos con el uso de las etiquetas that e it: para resolver el problema que representaba la reducción que hace el inglés a it creé la tabla advervios temporales. Esto resuelve en la mayoría de casos los problemas de referirse de distinto modo a una localización-
- Viendo su gran utilidad, se han empleado multitud de archivos .set para definir los grupos de palabras relacionados, cosa que ha ahorrado escribir muchas lineas de código.
- En el video demostración he mostrado alguna de sus posibilidades, pero es capaz de entender un planteamiento de muchas formas diferentes. En la parte final ocurre un fallo de recursión AIML debido a un contexto inadecuado por estar la sentencia condicionada por un that. Decidí dejarlo así, ya que el video duraba ya 7 minutos.
