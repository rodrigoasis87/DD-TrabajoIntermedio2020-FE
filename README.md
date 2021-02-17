# Trabajo intermedio de Curso de Frontend 2020

Este es el punto de partida del trabaj intermedio del curso de Frontend 2020-2021 de DoctaDevs. Revisá el detalle completo de la actividad en [Notion](https://www.notion.so/joelalejandro/Proyecto-Intermedio-GitHub-5bcbbceb34e94c2abc2da09a9699914c).

Para comenzar el trabajo, realizá un [fork](https://github.com//DoctaDevs/DD-TrabajoIntermedio2020-FE/fork) de este repositorio.

Tendrás tiempo hasta el 15 de febrero de 2021 para entregar la actividad.

--------------------------------------------------------------------------------------------------------------------------

Fecha redacción del proceso: hoy 17/02

Proceso del trabajo intermedio: Maqueta de la página Github.

Todo comenzó... algún tiempo atrás en la isl-- no, mentira.

Bueno, voy a intentar hacer una breve reconstrucción cronológica de mi proceso:

Lo primero, bastante tiempo atrás, en diciembre, fue leer detalladamente la consigna y, acto seguido, realizar un análisis
en papel, dibujando lo que sería la estructura en HTML. Hasta ahí todo bien. Paréntesis:

(Una vez realizado ese incipiente análisis, esto no es excusa, me pasaron cosas muy complicadas a nivel personal que literalmente no me dejaron volver a poner cabeza a esto. Muy brevemente, y perdón por comentar cuestiones extracurriculares, pero es para que me entiendas, quedé envuelto en un enriedo amoroso con una piba que viajó a resolver su situación con su pareja a EEUU, y un día parecía que se volvía, otro que se quedaba, y así durante varias semanas. Sinceramente el nivel de incertidumbre no me dejaba pensar en otra cosa y la angustia vencía a la voluntad de codear. Ya está todo bastante encaminado por suerte, pero fue bastante complicado. No me hubiese imaginado jamás encontrarme en una situación así, pero bueno, a veces nos pasan cosas que no elegimos y que nos exceden, ia tú sabe. Ah, y también estuve estas últimas dos semanas con covid, como para terminar de pasarla joya, je.)

Retomo lo curricular.

Luego de armar la estructura en HTML, ya tiempo después de haber leído la consigna, directamente empecé a poner clases y diseñar los estilos. Acá los primeros aprendizajes (que vinieron unas semanas después): por un lado, que la etapa de análisis no se reduce exclusivamente a diagramar la hoja en HTML, sino que tendría que haber hecho un análisis integral de todo, incluyendo CSS y también las consignas, porque tiempo después de empezar a codear en CSS, retomé las consignas y me dí cuenta de que estaba omitiendo muchas cosas. Codeando en CSS llegué hasta el <nav> (donde se encuentra el listado de opciones en horizontal), y hasta ahí me concentré más que nada en realizar una réplica lo más estéticamente idéntica posible. Tal vez no era eso lo más importante, sino la reutilización de clases, las hojas de estilo bien separadas, e incluso haber forkeado, je. Empecé creando un repositorio sin haber forkeado, por eso hay varios commits que no vas a poder ver. Luego sí, hice el fork y copié los archivos en el nuevo repo. Borré los archivos en la pc, no sé si aún así quedan en el repo, creo que sí, por las dudas te paso el link. Tampoco fui realizando esta redacción a medida que tomaba decisiones. Me hubiese gustado hacerlo así porque eso también te va alertando sobre las decisiones que vas tomando. Queda para la próxima.

Una vez terminada esa "primera sección" (porque subdividí la estructura del <main> en varias <section>) hice un repaso de las consignas para poder acomodarme a los requerimientos establecidos.

Realicé el fork, creé un archivo buttons.css para separar las propiedades de los botones, creé variables para los colores que más se repetían, y fui realizando anotaciones tanto en HTML y CSS sobre la forma de aplicar las etiquetas y las clases.

De ahí en adelante, empecé a trabajar con esa lógica más ordenada.

Reutilicé cuanta clase pude reutilizar. Algo que también me surgió fue lo siguiente: pensando en la posibilidad de crear clases con poquitas variables para reutilizarlas la mayor cantidad de veces, noté que también podía ocurrir que una etiqueta se me llenara de clases. Ahí encontré un nuevo criterio para tener en cuenta en el análisis inicial.

En esta nueva línea de trabajo más ordenada y criteriosa, busqué terminar de maquetar el MobileFirst, sabiendo que luego tendría que aplicar MediaQueries para llevar los elementos a la configuración Desktop. 

Una vez terminado, comencé a implementar los menú expandibles. Sé que eran 4, pero me concentré en dos, por el tiempo que me quedaba (cronológicamente ya estamos en este fin de semana largo). Me hubiese gustado dedicar tiempo a explorar animaciones como transition, pero no llegué. 

En el primero, que se desprende del header, traté de encontrar opciones de posicionamiento que desplazaran el resto de la hoja, pero no encontré o no me funcionaron. Por eso acudí a position:absolute, entendiendo que no es la mejor opción. Dentro de este menú, incorporé un <input> como cuadro de búsqueda. Las demás propiedades aplicadas cumplen las funciones de dar al menú la apariencia apropiada, con fondo gris oscuro y las separaciones correspondientes entre líneas.

En este tramo del trabajo, tanto en los menú expandibles como al momento de reacomodar elementos para la versión Desktop, apelé al uso de position absolute y relative, tal vez haciendo uso y abuso, pero fueron las únicas opciones que logré aplicar y que me dieran una cierta solución.

Para el paso de Mobilie a Desktop, apliqué la clase @media (min-width:770px), y dentro de ella utilicé nuevas clases para redefinir la ubicación de los contenedores, nuevamente con position absolute y relative, manejando el ancho de los mismos con un valor porcentual, y ubicándolos desde los márgenes aplicando right, left, top y bottom. Intenté poner clases en etiquetas contenedoras para agrupar los divs utilizando flex y grid, pero no tuve éxito.

En cuanto a la visión oscura del fondo de la página, estoy por hacerlo ahora, así que te debo la explicación detallada del caso.

Como conclusión, este trabajo me sirvió para incorporar un montón de aprendizajes. Primero que nada, familiarizarme bastante con el código. Es la primera vez que le puedo dedicar tantas horas (aunque no fueran todas las que habría querido y lo terminé a las apuradas), lo que me permitió ver en tiempo real los cambios que iba realizando, aprendiendo qué cosas se pueden hacer, qué cosas no, qué cosas me conviene hacer primero, qué después, etc. También me dio una noción de cuánto me lleva hacer esto, qué implicancias tiene, cuánto lleva aprender. Me llevó a indagar bastante en Google y Youtube sobre distintas propiedades como display, position y otras.

Le dí bastante importancia a la apariencia, a los detalles, a la ortografía (yo creo que la ortografía debería valer 50 puntos =P). En ese sentido me sentí cómodo y confiado.

Y bueno, sobre todo, sí me quedaron bastantes dudas que espero poder ir puliendo en lo que se viene.

Eso creo que es todo hasta aquí. El hecho de elaborar esta suerte de informe habiendo terminado el trabajo y no durante el mismo seguramente me hace dejar unos cuantos detalles en el camino. También es cierto que cuando no se tiene un análisis exhaustivo desde el comienzo del trabajo y se empieza directamente a codear, se recurre demasiado a la metodología de prueba y error, que pasados los días hace que uno no recuerde exactamente por qué eligió tal o cual opción. Pero bueno, todos aprendizajes que quedan.