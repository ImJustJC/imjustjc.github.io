---
title: "Blue Prince"
lang: es
page_id: blue_prince
playtime: "21.2 horas"
date: 20/04/2025
---

<div class="quote-shadowbox">
Combinar puzles y roguelite es interesante, pero con sus defectos.
</div>

<!--content-->

<style>
.justified {
    text-align: justify;
    text-justify: inter-word;
}

ul {
    ::marker{
        content: "⚿ ";
    }

    .li-blue::marker {
        color:rgb(82, 82, 255);
    }

    .li-purple::marker {
        color: rgb(191, 67, 164);
    }

    .li-orange::marker {
        color:rgb(237, 171, 39);
    }

    .li-green::marker {
        color:rgb(10, 147, 13);
    }

    .li-red::marker {
        color:rgb(255, 25, 25);
    }

    .li-yellow::marker {
        color:rgb(250, 255, 95);
    }
}
</style>

Esta reseña compone la primera entrada de mi blog. ¿Saldrá bien? Es muy posible que no, pero llevo semanas con ganas de simplemente escribir mis opiniones sobre aquello a lo que juego.
Justamente, ha coincidido iniciar mi acercamiento a la redacción con terminar Blue Prince, un juego que, otra cosa no, pero da mucho de lo que hablar.

<h1>El misterio de Mt. Holly</h1>

<div style="display: flex; align-items: center; margin-bottom: 1.3em">
    <blockquote style="flex-grow: 1;" class="justified">
        Yo, Herbert S. Sinclair, de la Hacienda Mount Holly en Reddington, publico y declaro este instrumento, mi última voluntad y testamento, y por la presente revoco todos los testamentos y codicilos realizados hasta ahora.
    </blockquote>
    <img style="float: right; padding-left: 1em; width: 60vw; max-width: 650px;" src="/assets/images/games/blue_prince/mthollyestate.jpg" />
</div>

Como voluntad final, el Barón Sinclair otorga en herencia la Hacienda Mount Holly a su sobrino nieto, Simon P. Jones (controlado por el jugador). Junto a esta disposición, establece un desafío que probará digno al heredero de Sinclair: hallar la 46ª habitación de su hacienda de cuarenta y cinco salas. Pocos días después, Simon alcanza Mount Holly e inicia su incursión en esta misteriosa hacienda.

<div style="display: flex; align-items: center; justify-content: space-between; margin-bottom: 1.3em">
    <img style="width: 48.5%;" src="/assets/images/games/blue_prince/day1.jpg" />
    <img style="width: 48.5%;" src="/assets/images/games/blue_prince/entrance.jpg" />
</div>

Nada más adentrarse al recibidor, una de las últimas escrituras de Herbert yace en la mesita central, destinada al recién llegado Simon. En ella, queda claro que esta aventura transcurrirá a lo largo de días o incluso semanas, pues la mansión puede parecer <strong>diferente al regresar en la mañana siguiente</strong>. Además, establece varias normas que prohiben mantener hallazgos materiales entre días y pasar la noche dentro de la hacienda. Es con esta información que se presenta el enfoque <em>roguelite</em> del título, pero, ¿qué hace única cada run?

<h2>Un rompecabezas por construir</h2>

Junto a la carta de presentación se encuentra un plano de construcción de toda la hacienda, dividiendo el terreno en una cuadrícula de 5 columnas por 9 casillas vacías salvo por dos de ellas: el recibidor, situada en el centro al sur de la hacienda, y la <strong>antecámara</strong>, también en el centro pero en el extremo norte. Únicamente desde la antecámara puede conseguirse acceso a la ansiada habitación 46. Este plano también presenta las posesiones del personaje e información general sobre la run actual y, en general, el progreso de la partida.

<img style="width: 100%;" src="/assets/images/games/blue_prince/blueprint.jpg" />

<div style="margin-bottom: 1.3em">
    <img style="float: right; padding-left: 1em; width: 50vw; max-width: 600px;" src="/assets/images/games/blue_prince/drafting.jpg" />
    Con una mansión hueca al frente, es tarea del jugador maquetar qué salas ocupan cada casilla. Al intentar atravesar cualquier puerta que desemboque en una casilla vacía, se inicia un proceso de maquetación donde se muestran tres opciones con salas escogidas al azar. Es aquí donde queda presente el eje central de todas las runs y se expanden las posibilidades hasta un horizonte aparentemente interminable: día a día, este hogar será completamente distinto a instancias anteriores; en ocasiones, incluso con salas distintas que pueden tardar días en volver a presenciarse. Según este factor aleatorio y las decisiones realizadas al explorar la hacienda será establecida su estructura y las metas que podrán alcanzarse. A nivel individual, cada sala sí es constante y mantendrá sus atributos, como el número de salidas, efecto y distribución interior. Como todo <em>roguelite</em>, las primeras runs pueden no llegar muy lejos dada la falta de experiencia en la colocación de salidas estratégicamente para paliar la aleatoriedad, o simplemente al tratar de explorar las decenas de opciones que propone el sistema continuamente (las salas de mayor interés suelen tener un coste elevado o incluyen pocas salidas que acaben bloqueando la posibilidad de avanzar).
</div>

<h1>Aventurarse a la mansión cambiante</h1>

El objetivo queda claro nada más iniciar la partida: llegar a la antecámara y acabar entrando a la habitación 46 a base de generar salas alineando sus salidas avanzando hacia el norte. Esto no siempre será posible de una forma directa gracias a la aleatoriedad, pues se ofrecen salas con todo tipo de combinaciones (desde caminos sin salida, hasta pasillos con puertas hacia las cuatro direcciones cardinales). Mientras que en un día consigues alcanzar rangos altos de la hacienda, otros estarás restringido la sección inicial si la suerte no está de tu lado para maquetar las salidas correctas.

Aún con un objetivo global en mente, habrá que avanzar con precaución, pues cada día el jugador dispone de una <strong>cantidad limitada de recursos</strong>. El más importante y que debe controlarse con máxima precisión son los <strong>pasos</strong>, consumidos al atravesar una puerta y acceder a una sala diferente. Es importante considerar que se consume un paso cada vez que se atraviesa una puerta, ya sea al visitar nuevas salas o retrodecer a sitios anteriores ya vistos; desprevenir el consumo de pasos hará que los días sean mucho menos productivos y no puedan alcanzarse rangos superiores.

<h2>No todo lo que reluce es oro</h2>

Entre las normas establecidas al comenzar la aventura quedaba indicada la prohibición de mantener recursos y objetos de un día para otro. A lo largo y ancho de esta hacienda se encuentran distribuidos tres recursos básicos que serán necesarios durante la exploración: monedas de oro que podrán intercambiarse por otros objetos; llaves para abrir puertas cerradas o cofres; y gemas usadas como pago para generar las salas más raras y con mayor potencial útil.

<figure style="margin: 0 0 1.3em 0">
    <img style="width: 100%;" src="/assets/images/games/blue_prince/storeroom.jpg" />
    <figcaption>
        <p>Salas como la <em>Storeroom</em> (almacén) otorgan una gema, llave y moneda a cambio de ser un camino sin salida.</p>
    </figcaption>
</figure>

Además de esos recursos, en ocasiones pueden hallarse objetos con utilidades específicas, como una zapatillas que reducirán el consumo de pasos mientras exploramos las habitaciones, un martillo con el que romper las cerraduras de cofres pequeños y abrirlos sin gastar llave, o múltiples llaves especiales que influyen al resultado de abrir puertas cerrradas.

<blockquote class="quote-rule">
<p style="margin-top: 1.3em">Si bien disponer de recursos y objetos distribuidos por toda la casa conforme se expande, esto induce una necesidad de mantenerse pendiente a cada recoveco constantemente por el pensamiento de "¿Y si hay algo?". Aunque salas concretas siempre contienen los mismos puntos donde aparecen, es común encontrar monedas o llaves tiradas por el suelo o detrás de muebles, y acabas pasando de un sitio a otro con la cabeza agachada mirando al suelo.</p>

<p>No solo es un problema el tenerte mirando hacia abajo todo el rato, incluso cuando entras a una sala donde sabes que hay algún objeto, no hay nada que lo haga destacar del resto de la habitación. En mis más de 20 horas de juego, he tenido situaciones de no encontrar algo que tenía delante más veces de las que me gustaría admitir. Sumado a la necesidad de recoger o interactuar con elementos del escenario para resolver ciertos enigmas, no me extraña que haya perdido la oportunidad en más de una cosasión de completar algo que, en principio, debería ser casi trivial.</p>
</blockquote>

<h2>Habitáculos ingeniosos</h2>

Dentro de esta amalgama pseudoaleatoria, conocer el uso de cada habitación maquetada será el punto clave para tener <em>mejores</em> runs y gestionar correctamente los recursos que proporciona este hogar. Una característica común a cada sala es un código de color que define su propósito principal:

<ul>
    <li class="li-blue">Azul: planos generales con utilidad variada o esencial para el avance.</li>
    <li class="li-purple">Púrpura: dormitorios, con sinergias relativas a la obtención de pasos.</li>
    <li class="li-orange">Naranja: salones y pasillos, generalmente sin utilidad específica pero con mayor número de salidas.</li>
    <li class="li-red">Rojo: salas con varias salidas pero efectos negativos que afectan al resto del día.</li>
    <li class="li-green">Verde: salas relativas a la naturaleza, caras de construir pero con efectos muy llamativos</li>
    <li class="li-yellow">Amarillo: tiendas en las que intercambiar monedas por objetos variados.</li>
</ul>

Todas las salas tienen una utilidad, que quizá destaque más en ciertas situaciones o empeore la situación de la partida. Entre todo el conjunto, al cabo de poco tiempo de juego hay dos habitaciones que resultan mucho más llamativas a nivel general por su utilidad en cualquier momento: <em>Billiard room</em> (sala de billar) y <em>Parlor</em> (salón). Ambas contienen un puzle individual que puede ser completados sin ayuda externa (aunque ciertos documentos explican su funcionamiento o dan consejos), y ofrecen una recompensa más o menos conocida.

<div style="display: flex; flex-direction: row; align-items: center; margin-bottom: 1.3em; gap: 1.5em">
    <div style="flex: 1 1 40%">
        <p>La sala de billar incluye un tablero de dardos con el que interactuar. Al hacerlo, se verá iluminado uno de los paneles indicando el primer paso del acertijo. No desvelaré aquí la metodología en detalle, pero este puzle captará enseguida la atención de cualquiera interesado en rompecabezas matemáticos, ya que tiene unas normas establecidas y solo se alteran los valores, operadores y orden a seguir. Como recompensa, la diana oculta un premio en forma de llaves comunes o una llave especial, de ahí el gran interés por esta habitación.</p>
    </div>
    <div style="flex: 1 1 60%">
        <img src="/assets/images/games/blue_prince/billiard.jpg" />
    </div>
</div>
<div style="display: flex; align-items: center; margin-bottom: 1.3em; gap: 1.5em">
    <div style="flex: 1 1 60%">
        <img src="/assets/images/games/blue_prince/parlor.jpg" />
    </div>
    <div style="flex: 1 1 40%">
        <p>Nada más entrar al <em>Parlor</em>, destacan tres cajas de distinto color sobre pedestales y una frase en su tapa. En una mesita cercana se encuentra una carta definiendo las reglas del puzle: al menos una caja es cierta; al menos una caja es falsa; y solo una caja contiene gemas. Evaluando la frase indicada en cada caja, habrá que determinar dónde se encuentran las gemas, conociendo estas reglas.</p>
    </div>
</div>

<blockquote class="quote-rule">
<p style="margin-top: 1.3em">
    Tanto el puzle de dardos como el <em>Parlor</em> son muy buenas propuestas de acertijos menores, pensados para solucionarse en un momento. A medida que resuelves más y más veces cada uno, su dificultad aumenta e introducen situaciones más complejas; en el caso de los dardos, también añaden variaciones sobre las reglas que establecían en un inicio, una situación compleja de encajar de primeras. Repetir una y otra vez estas salas acaba resultando monótono, ya que, además, es una necesidad conseguir sus recompensas si quieres avanzar en la run.
</p>
</blockquote>

<h2>Siempre hay otro secreto</h2>

Ya hemos visto cómo cada habitación propone un reto interesante, normalmente corto pero con llamativas recompensas para continuar con el día. Sin embargo, siendo esperable de un juego de este estilo, todo su contenido está cubierto por uno o varios misterios de gran escala, que requieren varios intentos hasta completarse. El primer obstáculo con el que uno se topa relativamente pronto sucede una vez alcanzas <span class="quote-spoiler" tabindex="0">la antecámara, pues sus accesos están bloqueados y no es posible entrar simplemente alcanzado la sala</span>.

A la vez, simplemente jugar y explorar más y más salas hace que poco a poco empiecen a destacar ciertos elementos del escenario, en especial <span class="quote-spoiler" tabindex="0">las parejas de cuadros</span> que se hallan en casi todas las salas que pueden generarse en la hacienda. Es aquí donde, tras un tiempo de juego variable según el factor aleatorio de cada partida, se desvela que no son simplemente decoración y, en efecto, forman parte de un acertijo a mayor escala que será resuelto a lo largo de múltiples días.

<blockquote class="quote-rule">
<p style="margin-top: 1.3em">
    Algo común a los juegos de este estilo es el proporcionar ese momento clave, que dura escasos segundos, pero te hace sentir un cosquilleo característico al ver que, efectivamente, llevas horas de juego ignorando una cosa esencial que puede llevarte a resolver muchas de las preguntas que has ido formulando. Pese a solo completar el final básico del juego, me hico sentir esto varias veces durante la aventura; todas ellas igual de espectaculares, daba la impresión de que nunca iban a acabar los secretos.
</p>
<p>
    El siguiente párrafo contiene spoilers sobre uno de los principales misterios que presenta el juego y, aunque es más bien secundario, merece completamente la pena descubrirlo por uno mismo. A modo de resumen, es una idea increíble con una implementación sobresaliente que se integra perfectamente con el resto del juego.
</p>
<p class="quote-spoiler" tabindex="0">
    No cabe duda que uno de los elementos que más llaman la atención durante una partida es la presencia de parejas de cuadros en las habitaciones visitadas. A priori, muestran dibujos cualesquiera, sin mucha relación entre sí. Nada más encontrar y acceder a una sala concreta, el estudio, se revela que todo el mapa de hacienda contiene 44 letras formando un mensaje. Cada letra corresponde a cada hueco, sin contar la antecámara, y se obtiene a través de una pareja de palabras que únicamente difieren en la letra en cuestión. Es aquí donde todo conecta: las parejas de cuadros representan las dos palabras clave que dan lugar a una letra de diferencia. Como ejemplo, el recibidor siempre incluye un cuadro con una carta de reina de diamantes y un as de picas, <em>face</em> y <em>ace</em> respectivamente, distanciadas por la letra <strong>F</strong>.
</p>
<p>
    Pese a la genialidad tras el diseño de estos misterios, cuentan con un gran defecto que puede llegar a complicarlos en exceso: resulta imposible de localizar a otros idiomas fuera del inglés las soluciones obtenidas, el procedimiento de ciertos puzles, o directamente las instrucciones básicas para siquiera entender lo que proponen. Esto también afecta al transfondo que muestra el juego mediante escritos, pues tener que leer decenas de páginas con ingentes cantidades de información y, encima, buscando cualquier indicio de pista o solución, es un reto que rápidamente se vuelve tedioso para cualquiera con menor fluencia en el idioma.
</p>
</blockquote>

<h1>Mañana será un nuevo día</h1>

Hasta ahora, Blue Prince encaja sin duda en el género de puzles y ofrece aquello que se espera de él, pero incorpora un conjunto de mecánicas <em>roguelite</em> a la fórmula establecida. Al acabar un día, ya sea voluntariamente desde el menú o forzado al agotar los pasos disponibles, la hacienda vuelve a su estado original sin habitaciones distribuidas. Al principio, no parece encajar mucho la mezcla de ambos géneros ya que no están realmente relacionados; ¿qué motivación hay para repetir una y otra vez el proceso de explorar? La respuesta que da el juego es, sin duda, prometedora, donde no solo te exige mantenerte atento a los muchos enigmas que incluye, sino que acopla un sistema estratégico con el que construir el contenido del mapa a explorar.

En concreto, la idea tras enfocar el progreso en la división por días distintos es extender la duración del juego gracias a este sistema de construcción, sobre el que las propias decisiones del jugador y la aleatoriedad influyen directamente en el resultado al final del día. Además, volver a generar la hacienda cada vez fomenta visitar la mayoría de salas, ya sea en busca de algo concreto o por su utilidad estructural o funcional.

<h2>El <em>una más y me voy</em> y el <em>no puedo avanzar más</em></h2>

Otro aspecto común a los <em>roguelite</em> son las dos frases que componen el título de esta sección. Separar la experiencia jugable en fragmentos de un tiempo medible y aproximable con la experiencia previa de juego facilita a cualquiera medir sus sesiones de juego y si puede permitirse un intento más. Por supuesto, diseñar una progresión y acabar por ofrecer su totalidad directamente al empezar el juego haría que se consuma enseguida, de ahí que se implementen barreras, caminos secundarios o secretos que requieran varias partidas. La maquetación de salas en Blue Prince contenta ambas cuestiones: conociendo el número limitado de salas posibles en la hacienda y la curiosidad e intención de explorar de cada uno, el día promedio duraría entre 30 minutos hasta una hora; parejo a ello, ese factor aleatorio de generar una habitación tras una puerta se limita a únicamente 3 opciones (existen formas de alterar este proceso, pero la base aleatoria sigue influyendo igual).

Entre esas 3 opciones deben considerarse múltiples factores para elegir: ¿necesito el efecto o contenido de la sala para poder avanzar?; ¿tiene salidas suficientes para que pueda seguir explorando?; ¿puedo permitirme el riesgo de su efecto?. La situación más común que rápidamente cualquiera se enfrenta es el generar habitaciones sin pensar en sus salidas, originando un bloqueo en rangos iniciales de la mansión.

<figure style="margin: 0 0 1.3em 0">
    <img style="width: 100%;" src="/assets/images/games/blue_prince/results.jpg" />
    <figcaption>
        <p>Algunos días, ya sea intencionado o por culpa de la aleatoriedad, no será posible alcanzar ciertos objetivos al estar restringidos a una subsección del espacio disponible. En la imagen de arriba, toda la mitad norte es inaccesible dada la selección de habitaciones y, por tanto, imposibilita el avance hasta la antecámara.</p>
    </figcaption>
</figure>

<blockquote class="quote-rule">
<p style="margin-top: 1.3em">
    Desde el plano teórico, la idea de mezclar un juego de puzles con mecánicas <em>roguelite</em> no llega a armonizar, pero tampoco desentona drásticamente. Durante las primeras horas de juego es un añadido muy curioso, que incluso motiva a continuar explorando en busca de nuevas posibilidades que no aparecieron antes. Al cabo de pocos días, el sentimiento de satisfacción del sistema empieza a desmoronarse cuando surgen situaciones extremadamente negativas. Es común tener un objetivo claro en mente, la solución a uno de esos grandes enigmas, y no poder completarlo porque la sala necesaria no aparece en días.
</p>
<p>
    Esto mismo ha sido mi experiencia, con dos picos de desesperación al estar extremadamente cerca de resolver los puzles <span class="quote-spoiler" tabindex="0">del laboratorio</span> y <span class="quote-spoiler" tabindex="0">del depósito de agua</span>; ambos requieren <span class="quote-spoiler" tabindex="0">activar la energía en salas concretas desde la caldera, pero ésta solo manda energia a salas contiguas</span>. De mis 21 horas de juego, con casi 40 días completados, solo en uno de ellos pude cumplir las condiciones que pedían esos puzles.
</p>
</blockquote>

<h1>Conclusiones</h1>

En definitiva, Blue Prince ha sido toda una sorpresa, para bien y para mal, pero tras varios días de meditarlo y repasar el juego con esta review, puedo decir sin miedo que la experiencia general ha sido buena. Por supuesto, los momentos malos son muy agudos y es facil que impacten a la percepción de cualquiera, pero la capacidad del título por ocultar misterios tan densos en cada esquina y el cúmulo de grandes ideas opacan en gran medida a los claros errores que presenta. Simplemente retocando un poco el factor aleatorio, quizá dando alguna alternativa para facilitar la búsqueda de habitaciones concretas, creo que se acercaría mucho a algo perfecto jugablemente. Pocos días después de su salida, ya han sido publicados un par de parches con correcciones a errores menores o concretos y pequeños ajustes a varias mecánicas.

Sin duda, <strong>recomendaría Blue Prince a cualquiera interesado en juegos de puzles</strong>, aunque con un gran aviso del factor aleatorio que incorpora el juego y extiende artificialmente el tiempo necesario hasta cumplir objetivos. Buena suerte a todo aquel con intención de abordar el misterio de Mount Holly, es sin duda una experiencia única :)

