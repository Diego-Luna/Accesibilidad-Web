# Accesibilidad-Web

## ¿Qué es WCAG?

En inglés son las Web Content Accessibility Guidelines o en español las Pautas de Accesibilidad para el Contenido Web. Un rango de recomendaciones para crear contenido web más accesible.

### Historia de WCAG
* W3C - World Wide Web Consortium : Creadores de los estándares que usamos para construir la web.

* WAI - Web Accessibility Initiative : Iniciativa dentro de W3C cuya meta es asegurar la accesibilidad web.

## 12 criterios de conformidad

Aunque las pautas (referidas también por su nombre en inglés WCAG) son muy completas y siguen creciendo a medida que nuestras tecnologías crecen, es importante conocer los 4 principios que nos guían para poder tomar decisiones puntuales a nivel de nuestros productos. Dentro de cada principio encontramos los criterios de conformidad que se pueden interpretar acorde al nivel de WCAG que le quieres o debes aplicar a tu sitio web. Recuerda que los 3 niveles son:

* A - nivel basico

* AA - nivel intermedio

* AAA - nivel avanzado al cual debemos apuntar si trabajamos en servicios del gobierno, universidades o servicios esenciales de la vida cotidiana.

En esta lectura vamos a profundizar sobre los criterios de conformidad para tener una idea más clara de que podemos encontrar dentro de WCAG. Podemos empezar por el primer principio:

### 1. Perceptible

Los criterios de conformidad bajo este principio se enfocan en asegurar que todo el contenido que es importante se pueda interpretar de varias maneras. Aqui nos queremos

* 1.1 Asegurar que estamos proporcionando alternativas textuales para todo contenido no textual.

* 1.2 Proporcionar alternativas para los medios tempodependientes (como videos o audios, queremos ofrecer opciones como subtítulos o guiones).

* 1.3 Crear contenido que se pueda presentar de diferentes formas sin perder información o estructura.

* 1.4 Facilitar a los usuarios ver y oír el contenido, incluyendo la separación entre el primer plano y el fondo


### 2. Operable

Cuando hablamos de ser operable, queremos asegurarnos que nuestro sitio es fácil de usar y navegar, que se puede navegar de diferentes maneras y con mouse y/o teclado

* 2.1 Proporcionar acceso a toda la funcionalidad mediante del teclado

* 2.2 Darle a las usuarias suficiente tiempo para leer y usar el contenido (tener esto en cuenta cuando hacemos time outs, comunicarlos y dar opciones para pedir más tiempo si es necesario)

* 2.3 Tener mucho cuidado de no usar elementos que brillan o se mueven muy rápido ya que pueden provocar ataques, espasmos o convulsiones

* 2.4 Asegurarnos que nuestros usuarios pueden navegar, encontrar contenido y determinar dónde se encuentran en nuestros sitios


### 3. Comprensible

Hacer que nuestro sitio web sea comprensible nos asegura que un rango de personas lo pueden usar desde la persona que vive con una discapacidad mental que necesita patrones comunes para saber cómo usar la web hasta la persona que va de carrera y necesita consultar algo rápido

* 3.1 Tener en cuenta los tamaños de texto y contraste de colores para que los textos resulten legibles y comprensibles

* 3.2 Hacer que las páginas web aparezcan y operen de manera predecible.

* 3.3 Dar instrucciones para evitar errores y oportunidades para corregirlos cuando ocurren

### 4. Robusto

Cuando hacemos productos que funcionan en muchos lados, abrimos las posibilidades que cualquier persona los use sin importar su ubicación, máquina, navegador y mucho más

* 4.1 Maximizar la compatibilidad con las aplicaciones de usuario actuales y futuras, incluyendo las tecnologías asistivas

Los demas: http://www.sidar.org/traducciones/wcag20/es/

## Tecnología Asistivas - cuáles son y cómo funcionan

Las tecnologías asistivas ayudan a las personas con alguna de sus capacidades mermadas, sean visuales, auditivas o motoras, a consumir la web de la misma forma que lo hacen los demás.

Un ejemplo muy simple y común de este tipo de tecnologías son los lentes 👓. Estos permiten que personas con defectos en la visión puedan percibir el mundo igual que los demás.

Tecnologías asistivas:
1. Visuales:
* Lectores de pantalla.
* Extensiones que manipulan el CSS.

1. Motoras:
* Varilla bucal.
* Switch


## Pruebas manuales con tu teclado

El teclado es muy importante en la accesibilidad web porque las tecnologías asistivas tienden a conectarse con el teclado para darle a sus usuarios diferentes maneras de navegar cuando no tienen acceso a un mouse o un teclado como nosotros.
Los elementos que reciben foco de teclado son elementos interacctivos:

* Enlaces: nos llevan a otra página, son para la navegación.
* Botones: nos ayudan a interactuar con la página de alguna manera.
* Formularios: requieren nuestra interacción para llenar nuestros datos.

Los div no reciben foco porque son un elemento presentacional, no esperan ninguna interacción a menos de que tú lo programes.

## [42 Browser Extensions to Perform Accessibility Testing Effectively](https://www.digitala11y.com/accessibility-plug-ins-ie-chrome-firefox-browsers/)

## Lectores de Pantalla

Los lectores de pantalla han abierto a la web a diversas personas que antes no podían usar los sitios web

Combinaciones de lectores de pantalla y navegadores:

* NVDA - Mozilla Firefox
* JAWS - Internet Explorer
* VoiceOver - Safari
* ChromeVox - Google 
* Apartado de Chorme DevTools → En Elements → Accessibility → Accessibility Tree

## VoiceOver

Para activarlo: "fin" + "cmd" + "f5"

Para pausar: "cmd"

Mover adelante: "ctr" + "alt" + flecha derecha

Mover atras:  "ctr" + "alt" + flecha izquierda


## ¿Qué es el HTML semántico?

El HTML semántico es una de las herramientas más poderosas a la mano a la hora de implementar la accesibilidad web

### ¿Qué es?

No solo nos ayuda con algunos aspectos de presentación pero le agrega significado a nuestro contenido. Es decir agregarle significado al navegador

* Sin HTML semántico: Se puede crear una estructura visual buena con CSS pero realmente difícilmente los navegadores entenderán la semántica del sitio web construido

```html
<div></div>
	<div></div><div></div>
<div></div>
```

* Con HTML semántico:
    * Usamos una variedad de elementos con significado que el navegador lee e implementa la presentación y alguna interacción.
    * El navegador incluye esto en el árbol de accesibilidad, este lo usan los lectores de pantalla

```html
<header></header>
	<article></article>
<footer></footer>
```

## ARIA - Accessible Rich Internet Applications
ARIA es un conjunto de atributos especiales para accesibilidad que pueden añadirse a cualquier etiqueta, pero especialmente adaptado a HTML

ARIA ⇒ Fue creado por la W3C a través de WAI (web accessibility initiative)

Atributos de ARIA:
* Roles
* Propiedades
* Estados

### ARIA - Roles

Roles de ARIA: Define el tipo general del objeto ( como un artículo, una alerta o un deslizador)

Los roles le comunican al navegadores cuales son las interacciones que debería esperar y cómo se va a usar este objeto en nuestro proyecto. Se usan en situaciones muy especificas, es mejor depender del HTML semántico para comunicar los roles.

### ARIA properties

Las propiedades ARIA la vamos a usar más seguido.

Comunican atributos que son esenciales para el comportamiento o significado de un elemento pero que se suelen comunicar visualmente

### ARIA label
Podemos usar para agregar un string para describir un elemento de nuestro código
Ejemplo:

```html
<form class="form-container">
        Nombre<input type="text" aria-label="nombre"/> <br />
        Correo<input type="text" aria-label="correo"/> <br />
        <div class="message-input">Mensaje<input type="text" /> <br /></div>
        <button class="send-button">Enviar</button>
      </form>
```

### ARIA states

Estados de ARIA comunican estados y cambios de estados en elementos que se suelen comunicar visualmente

Existen veces que mostramos casos que solo pasan cuando algo cambia en la pantalla
* Impidiendo que personas con discapacidades visuales no podrán notar ese cambio

* Debemos dar una experiencia del sitio a personas discapacitadas al igual que damos importancia a personas sin ningún problema

Si tenemos un checkbox
*   Sabemos que esta seleccionado por que está marcado
*   Alguien con discapacidad quizás no pueda ver eso

Un lector de pantalla no se dará cuenta que algunas cosas no se están mostrando.
Podemos usar el atributo aria-hidden para ocultar algunas cosas de los lectores de pantalla,


```html
<li aria-hidden="true">...</li>
```

## Contrastes de color

El contraste de color es la diferencia existente entre dos o más colores que interactúan en un diseño de forma que afectan al modo en el cual se percibe. El color según sus diferentes características influye en el efecto que causa en las personas

* Los contrastes de color se refieren a la diferencia del color de fondo y color del texto

* Normalmente es tarea del diseñador encargarse de este aspecto, pero como desarrolladores podemos encargarnos de detectar problemas de contraste para posteriormente comunicar el problema

* Si el contraste es muy bajo no se puede ver el texto correctamente

* Podemos usar Chrome Dev Tools para revisar el contraste de los colores de los textos
    * Nos indicaran a que nivel de WCAG estaremos llegando

## Skip links
Son botones que a simple vista no se ven pero al momento que un software de lectura de texto los detecta aparecene

Se crean poniendo un botón común y corriente

```html
<button id="skip-link">Saltar al contenido</button>

```

Y en css le pondremos lo siguiente

```css
.skip-link{
weight: 0; /* desaparecemos el botón a simple vista*/
}
.skip-link:focus,
.skip-link:active{
background..
font ...
} /* de esta forma cuando navegen con un teclado este aparecerá*/
```
