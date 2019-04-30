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


## Bot de fitness y nutrición
- Tomando de partida los archivos .set y .map del anterior se crea una estructura más organizada, con un .aiml para cada función principal y derivados. Algunos fallos puntuales del video demostración se deben a archivos desactualizados que se emplearon del otro bot (fallan algunas palabras que se agregaron al otro a posteriori).
- El concepto de este bot es orientar a personas interesadas en el fitness. Emplea el elemento <reply> para facilitar la navegación dentro y entre las distintas funciones. También se puede interactuar únicamente por comandos.

> ### FUNCIONES:
>
> #### Asesoramiento
> - Guía al usuario estableciendo su objetivo, dirigiéndole a una calculadora de metabolismo basal y la web de myfitnesspal.
> - Se utilizan los datos obtenidos para realizar cálculos básicos gracias a la librería aimlstandardlibrery.aiml
> - Dada las limitaciones del sistema, es necesario establecer varias condiciones en dos categorías para sacar la conclusión final.
> - Una vez terminado el asesoramiento inicial, ofrece ir a otras categorías.
> 
> #### Profesionales
> - Da un listado de profesionales aconsejados en función del objetivo (si está aun en memoria, de lo contrario lo solicita).
> - Muestra a 8 hombres y 2 mujeres (enrenadores, preparadores, divulgadores, nutricionistas) aconsejados para cada caso y enlaza a sus páginas web.
>
> #### Mitos
> - Sección simple con 20 entradas distintas que desmiente falsas creencias sobre nutrición y entrenamiento.
> - Se puede interacuar mediante el botón de <reply> o por el chat
  >
> #### Quiz
> - Juego de 5 preguntas aleatorias (de 20) que establece puntuación y comenta el resultado.
> - Además, da la opción de explicar la pregunta haciendo referencia a su Id, vinculando en cada caso un enlace a un articulo relacionado.
