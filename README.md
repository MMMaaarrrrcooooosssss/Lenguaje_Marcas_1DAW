Guía de Estudio: Programación, Estructuración y Elementos Contenedores en HTML
Esta guía de estudio recopila y organiza todos los elementos, estructuras, tipos de control de formularios y propiedades asociadas que se pueden programar y definir dentro del lenguaje HTML y su interacción con CSS, en base al material del curso.
1. Resumen de Contenidos: Elementos Programables en HTML
En HTML se pueden programar dos categorías principales de elementos según su comportamiento de visualización: elementos en bloque y elementos en línea.
A. Elementos Contenedores y de Estructura
Elementos en Bloque: Introducen automáticamente un salto de línea antes y después del elemento.
Ejemplos especificados: <h1>, <p>, <ul>, <table>.
Contenedor genérico de bloque: <div>.
Uso de <div>: Se utiliza como contenedor para agrupar otros elementos HTML (párrafos, encabezados, listas). No aporta significado semántico por sí solo, pero combinado con CSS permite aplicar atributos de estilo a grandes bloques de contenido y estructurar el diseño de la página (sustituyendo el antiguo método basado en tablas).
Elementos en Línea: Se colocan a continuación del elemento anterior en el flujo de texto, sin introducir saltos de línea.
Ejemplos especificados: <b>, <i>, <a>.
Contenedor genérico en línea: <span>.
Uso de <span>: Funciona como un contenedor de texto sin significado especial. Junto con CSS, permite aplicar atributos de estilo a partes específicas de un texto.
B. Elementos y Controles de Formularios
A través de la etiqueta <input> y elementos complementarios de agrupación, se pueden programar los siguientes controles de interacción:
Tipos de campos <input>:
Texto (type="text"): Campo donde el usuario puede escribir una línea de texto.
Contraseña (type="password"): Campo donde el usuario puede escribir texto que se oculta a la vista (no se lee lo que se escribe).
Casilla de verificación (type="checkbox"): Permite al usuario marcar o desmarcar valores de su interés.
Fichero (type="file"): Permite explorar el sistema de archivos del ordenador y seleccionar un archivo para enviarlo.
Agrupación de controles:
<fieldset>: Agrupa un conjunto de campos o controles relacionados en un formulario.
<legend>: Establece el título o descripción del grupo representado por un <fieldset>.
Comportamiento de botones (type):
submit: Envia la información del formulario.
reset: Reinicia todos los campos del formulario a sus valores iniciales.
button: Define una función personalizada ejecutada mediante un script.
Atributos de los controles:
name: Obligatorio. Es el nombre único del campo dentro del formulario.
value: Representa el valor que se enviará cuando se procese el formulario.
disabled: Deshabilita el control para impedir que el usuario pueda interactuar con él o pulsarlo.
tabindex: Define la posición del control en el orden o índice de tabulación de la página.
C. Modelo de Caja (Box Model) y Dimensiones
Cualquier elemento programado en HTML que se renderice en pantalla posee una estructura de caja conformada por 6 componentes principales y capas de visualización:
Componente / Capa
Descripción y Propiedades
Contenido (content)
El texto, imagen, tabla o caja div interna del elemento. Su tamaño se define con width (ancho) y height (alto). No admiten valores negativos. Se pueden definir en píxeles (px) o porcentaje (%) sobre la anchura del elemento padre.
Relleno (padding)
Espacio libre entre el contenido y el borde. Es transparente y deja ver el color o la imagen de fondo del elemento.
Borde (border)
Línea que encierra el contenido y su relleno. Se define mediante su anchura (border-width), color (border-color) y estilo (border-style).
Imagen de Fondo (background-image)
Imagen de fondo situada detrás del contenido y del relleno. Se encuentra en una capa superior al color de fondo, por lo que prevalece sobre este.
Color de Fondo (background-color)
Color que se muestra por detrás del contenido y del espacio de relleno.
Margen (margin)
Espacio transparente entre el borde del elemento y las cajas adyacentes. Muestra el fondo del elemento padre.

Reglas de Asignación de Valores Simplificados (Short-hand)
Las propiedades margin, padding, border-width y border-color pueden recibir entre 1 y 4 valores con el siguiente orden de aplicación:
1 valor: Válido/común para los 4 lados (superior, derecho, inferior, izquierdo).
2 valores: 1º valor para superior e inferior; 2º valor para izquierdo y derecho.
3 valores: 1º valor para superior; 2º valor para izquierdo y derecho; 3º valor para inferior.
4 valores: Orden de las agujas del reloj: 1º superior, 2º derecho, 3º inferior, 4º izquierdo.
Peculiaridades de Márgenes y Posicionamiento
Márgenes Verticales vs Laterales:
margin-top y margin-bottom (verticales) solo se pueden aplicar a elementos en bloque e imágenes.
margin-left y margin-right (laterales) se aplican a cualquier elemento.
Fusión de Márgenes Verticales: Cuando dos cajas verticales se encuentran adyacentes o una está contenida dentro de otra, sus márgenes verticales no se suman, sino que se fusionan tomando el valor del margen más grande.
Cálculo del Ancho Total de un Elemento: \text{Ancho Total} = \text{Margen Izq.} + \text{Borde Izq.} + \text{Relleno Izq.} + \text{Ancho Contenido} + \text{Relleno Dcho.} + \text{Borde Dcho.} + \text{Margen Dcho.} Ejemplo de cálculo: 30\text{px} + 10\text{px} + 50\text{px} + 300\text{px} + 50\text{px} + 10\text{px} + 30\text{px} = 480\text{px}.
Posicionamiento de Imagen de Fondo (background-position): Por defecto se ubica en la posición superior izquierda (0,0). Se especifica mediante:
Posición Horizontal: Palabras clave (left, right, middle), coordenadas fijas (ej. 12px) o relativas (ej. 5%).
Posición Vertical: Palabras clave (top, bottom, center), coordenadas fijas (ej. 20px) o relativas (ej. 15%).
2. Cuestionario de Evaluación (Quiz)
¿Qué diferencia principal existe entre un elemento en bloque y un elemento en línea en cuanto al salto de línea?
Indique cuáles son los elementos contenedores genéricos para bloque y para línea, y qué función cumplen cuando se combinan con CSS.
Mencione cuatro tipos de control <input> que se pueden programar en un formulario y la función de cada uno.
¿Qué papel desempeñan las etiquetas <fieldset> y <legend> en la programación de un formulario?
¿Qué diferencia de comportamiento existe entre asignar los valores submit, reset y button al atributo type de un botón?
¿Para qué se utilizan los atributos disabled y tabindex en un control de formulario?
Ordene las capas de visualización de una caja desde la capa más profunda hasta la más superficial.
Si un elemento div tiene un contenido de 300px de ancho, rellenos laterales de 50px cada uno, bordes laterales de 10px cada uno y márgenes laterales de 30px cada uno, ¿cuál es su anchura total ocupada?
¿Cómo se interpretan los valores si se define la propiedad CSS margin: 5px 33% 50px 0;?
¿A qué elementos se pueden aplicar los márgenes verticales (margin-top y margin-bottom) y qué ocurre cuando dos márgenes verticales coinciden?
Si se define width: 80% para un elemento div cuya caja contenedora padre tiene una anchura de 600px, ¿cuál es el ancho resultante en píxeles del elemento hijo?
¿Cuáles son las palabras clave posibles para configurar las posiciones horizontal y vertical del fondo mediante CSS?
3. Clave de Respuestas (Answer Key)
Diferencia de comportamiento: El elemento en bloque incorpora automáticamente un salto de línea antes y después del mismo. El elemento en línea se coloca a continuación del elemento anterior sin introducir ningún salto de línea.
Contenedores genéricos:
Bloque: <div>. Agrupa otros elementos (párrafos, listas, etc.) y se usa para el diseño/maquetación del documento y la aplicación de estilos a grandes bloques de contenido.
Línea: <span>. Sirve como contenedor de texto sin significado especial para aplicar estilos a partes específicas de un texto.
Tipos de <input>:
text: Permite escribir una línea de texto.
password: Permite escribir texto ocultando los caracteres introducidos.
checkbox: Permite marcar o desmarcar opciones.
file: Permite explorar el equipo del usuario y adjuntar un archivo.
<fieldset> y <legend>: <fieldset> agrupa controles relacionados dentro de un formulario, mientras que <legend> asigna un título o cabecera explicativa a dicho grupo.
Comportamiento del atributo type en botones:
submit: Envía la información del formulario.
reset: Borra los datos y restablece el formulario a su estado inicial.
button: No realiza una acción por defecto; su función debe programarse mediante un script.
Atributos disabled y tabindex:
disabled: Deshabilita el botón o campo impidiendo su activación o pulsación.
tabindex: Define el índice u orden de tabulación del control al navegar con el teclado.
Orden de capas (de más profunda a más superficial):
Color de fondo (background-color).
Imagen de fondo (background-image).
Relleno (padding) / Margen (margin) (ambos son transparentes).
Borde (border).
Contenido (content).
Cálculo de anchura total: \text{Ancho Total} = 30\text{px} (\text{margen}) + 10\text{px} (\text{borde}) + 50\text{px} (\text{relleno}) + 300\text{px} (\text{contenido}) + 50\text{px} (\text{relleno}) + 10\text{px} (\text{borde}) + 30\text{px} (\text{margen}) = 480\text{px}
Interpretación de 4 valores en margin: Se aplican en el orden superior, derecho, inferior e izquierdo. Superior: 5px, Derecho: 33%, Inferior: 50px, Izquierdo: 0.
Márgenes verticales y fusión: Solo se pueden aplicar a elementos en bloque e imágenes. Cuando dos cajas verticales se juntan o anidan, sus márgenes se fusionan tomando como valor único el margen más grande.
Cálculo de ancho en porcentaje: El porcentaje se calcula sobre el ancho del padre. 80\% \times 600\text{px} = 480\text{px}.
Palabras clave de posicionamiento de fondo:
Posición horizontal: left, right o middle.
Posición vertical: top, bottom o center.
4. Glosario de Términos
<div>: Elemento contenedor genérico a nivel de bloque. No aporta significado semántico y se utiliza principalmente para estructurar secciones de la página o agrupar elementos a los que aplicar estilos CSS.
<span>: Elemento contenedor genérico a nivel de línea. Se emplea para delimitar porciones de texto o contenido en línea con el fin de aplicarles reglas de estilo específicas mediante CSS.
<fieldset>: Etiqueta HTML de formulario utilizada para agrupar visual y lógicamente un conjunto de controles o campos relacionados.
<legend>: Elemento que define el título o etiqueta descriptiva para un contenedor <fieldset>.
disabled: Atributo booleano que deshabilita un control de formulario impidiendo que el usuario pueda interactuar con él o pulsarlo.
tabindex: Atributo que especifica el orden de tabulación de un elemento cuando el usuario navega por los controles mediante la tecla Tab.
Contenido (content): Región central de la caja de un elemento HTML donde se sitúa el texto, imagen u otros elementos contenidos. Sus dimensiones se controlan con width y height.
Relleno (padding): Espacio transparente comprendido entre el contenido de un elemento y su borde.
Borde (border): Línea que rodea el relleno y el contenido de un elemento. Se define por su anchura, color y estilo.
Margen (margin): Espacio libre exterior y transparente que separa el borde de un elemento respecto a las cajas de los elementos adyacentes.
Fusión de márgenes verticales: Comportamiento del renderizado por el cual los márgenes superiores e inferiores de dos cajas adyacentes o anidadas se combinan en un único margen cuyo valor es el mayor de los dos.
border-width: Propiedad CSS que establece el grosor de los bordes. Acepta valores numéricos con unidad (ej. px) o las palabras clave thin, medium (valor inicial) y thick.


Guía de Estudio: Programación y Estilizado con CSS
Esta guía de estudio ofrece una síntesis exhaustiva y detallada de los elementos, propiedades y comportamientos de maquetación y diseño que se pueden programar utilizando hojas de estilo en cascada (CSS) y su interacción con la estructura HTML, a partir del material docente analizado.
1. Inventario General de Elementos y Propiedades Programables en CSS
A continuación se detalla todo lo que es posible programar y configurar en CSS de acuerdo con las especificaciones del material:
1.1. Propiedades del Modelo de Caja (Box Model)
El modelo de caja define la estructura tridimensional y bidimensional de los elementos en pantalla. Se compone de varias capas con un orden de visualización concreto:
Contenido (content): Espacio central ocupado por texto, imágenes, tablas o div contenedores.
Relleno (padding): Espacio transparente entre el contenido y el borde. Muestra el color o imagen de fondo del elemento.
Propiedades individuales: padding-top, padding-bottom, padding-left, padding-right.
Propiedad abreviada: padding (acepta de 1 a 4 valores).
Borde (border): Línea que envuelve perimetralmente el contenido y el relleno.
Dimensiones: border-width, border-top-width, border-bottom-width, border-left-width, border-right-width. Valores aceptados: thin, medium (valor inicial), thick o valores numéricos específicos (ej. 2px).
Color: border-color, border-top-color, border-bottom-color, border-left-color, border-right-color. Valores aceptados: un color específico (ej. darkred, deeppink) o transparent.
Estilo: border-style (ej. solid).
Esquinas redondeadas: border-top-left-radius, border-bottom-right-radius (ej. 20px).
Sintaxis abreviada: border (ej. 2px solid darkred).
Fondo (Background):
background-color: Color de fondo que se muestra tras el contenido y el relleno (ej. lightpink).
background-image: Imagen que se muestra por detrás del contenido y del relleno. Prevalece sobre el color de fondo por situarse en una capa superior a este.
background-position: Define la posición inicial de la imagen de fondo (que por defecto se coloca en la esquina superior izquierda 0,0). Admite:
Coordenada horizontal: Palabras clave (left, right, middle), valores concretos (ej. 12px) o relativos (ej. 5%).
Coordenada vertical: Palabras clave (top, bottom, center), valores concretos (ej. 20px) o relativos (ej. 15%).
Margen (margin): Espacio libre exterior y transparente entre la caja y sus cajas adyacentes. Deja ver el color o imagen del elemento padre.
Propiedades individuales: margin-top, margin-bottom, margin-left, margin-right.
Propiedad abreviada: margin (acepta de 1 a 4 valores).
1.2. Reglas de Sintaxis para Propiedades Abreviadas de 1 a 4 Valores (margin, padding, border-width, border-color)
Las propiedades que definen los cuatro lados de una caja admiten de uno a cuatro valores bajo el siguiente esquema:
Nº de Valores
Regla de Asignación
1 Valor
Valor común para los cuatro lados (superior, derecho, inferior, izquierdo).
2 Valores
El 1º se asigna al lado superior e inferior; el 2º al lado izquierdo y derecho.
3 Valores
El 1º al lado superior; el 2º a los lados izquierdo y derecho; el 3º al lado inferior.
4 Valores
Se asigna en el sentido de las agujas del reloj: 1º superior, 2º derecho, 3º inferior, 4º izquierdo.

1.3. Dimensionamiento y Comportamiento de Flujo
Propiedades de dimensión:
width: Ancho del contenido.
height: Alto del contenido.
Unidades: Valores fijos en píxeles (px) o porcentajes (%). Los porcentajes se calculan a partir de la anchura del elemento padre (ejemplo: un elemento con width: 80% dentro de un contenedor padre de 600px tendrá un ancho de 480px).
Restricción: No admiten valores negativos. Se redimensionan dinámicamente según el tamaño de la ventana.
Cálculo del Tamaño Total de un Elemento (Ancho Total): \text{Ancho Total} = \text{margin-left} + \text{border-left} + \text{padding-left} + \text{width} + \text{padding-right} + \text{border-right} + \text{margin-right}
Visualización y Alineación:
display: Modifica el tipo de visualización del contenedor. El valor inline-block permite disponer elementos en línea manteniendo propiedades de bloque.
vertical-align: Alineación vertical de elementos (ej. top).
1.4. Reglas Especiales de Comportamiento CSS
Restricción de Márgenes Verticales vs. Laterales:
Los márgenes verticales (margin-top y margin-bottom) solo se pueden aplicar a elementos de bloque y a imágenes.
Los márgenes laterales (margin-left y margin-right) se pueden aplicar a cualquier elemento.
Fusión de Márgenes Verticales (Margin Collapsing):
Cuando existen varias cajas adyacentes en vertical o cajas contenidas una dentro de otra, sus márgenes verticales no se suman, sino que se fusionan tomando como valor final el más grande de los implicados.
1.5. Tipos de Elementos HTML sobre los que se aplica CSS
Elementos en bloque: Incorporan un salto de línea antes y después (ej. <h1>, <p>, <ul>, <table> y la etiqueta genérica <div>). <div> se utiliza como contenedor para agrupar otros elementos o para diseñar la estructura/layout de la página sustituyendo al uso antiguo de tablas.
Elementos en línea: Se colocan a continuación del elemento anterior sin salto de línea (ej. <b>, <i>, <a> y la etiqueta genérica <span>). <span> se usa para aplicar estilos CSS a partes concretas dentro de un texto.
Formularios y sus Controles:
Agrupaciones: <fieldset> (agrupa controles) y <legend> (título del grupo).
Entradas (<input>): Campos de texto (text), contraseña (password), casilla de verificación (checkbox), fichero (file).
Botones: submit (enviar), reset (reiniciar), button (ejecuta script).
Atributos de control asociados: name (identificador único), value (valor enviado), disabled (deshabilita el control), tabindex (orden de tabulación).
2. Glosario de Términos
Background-position: Propiedad CSS que establece la posición inicial de una imagen de fondo mediante coordenadas o palabras clave horizontales (left, right, middle) y verticales (top, bottom, center).
Border (Borde): Parte del modelo de caja que consiste en una línea que encierra completamente el contenido y su relleno.
Border-radius: Propiedad CSS utilizada para definir esquinas redondeadas en una caja (ej. border-top-left-radius, border-bottom-right-radius).
Box Model (Modelo de Caja): Concepto de diseño web según el cual todo elemento HTML se representa como una caja rectangular compuesta por contenido, relleno, borde y margen.
Display: inline-block: Valor de la propiedad display que permite que un elemento se comporten en línea con respecto a los demás elementos pero conservando las capacidades de dimensionado de un elemento en bloque.
Div: Elemento contenedor genérico a nivel de bloque en HTML. Sin significado semántico especial, se utiliza habitualmente junto a CSS para la maquetación de la página y la aplicación de estilo a grandes bloques de contenido.
Fusión de márgenes (Margin Collapsing): Comportamiento por el cual dos o más márgenes verticales adyacentes o anidados se combinan en un único margen con el tamaño equivalente al margen de mayor valor.
Margin (Margen): Espacio transparente situado en la zona más exterior de la caja que separa el elemento de sus vecinos. Muestra el fondo del elemento padre.
Padding (Relleno): Espacio transparente comprendido entre el contenido de un elemento y su borde.
Span: Elemento contenedor genérico a nivel de línea en HTML, ideal para aislar partes de un texto y aplicarles reglas de estilo con CSS.
Width / Height: Propiedades de CSS que definen la anchura y la altura de la zona del contenido de una caja. No aceptan valores negativos.
3. Cuestionario de Evaluación (Quiz)
Pregunta 1
¿Cuál es la diferencia fundamental en el comportamiento visual entre un elemento en bloque y un elemento en línea en HTML?
Pregunta 2
Mencione el orden de las capas de visualización en el Modelo de Caja desde la más profunda hasta la más externa. ¿Qué elemento prevalece entre el color de fondo y la imagen de fondo?
Pregunta 3
Si se declara la regla CSS margin: 5px 33% 50px 0;, ¿qué valor corresponde a cada lado del elemento?
Pregunta 4
Si un elemento <div> padre tiene una anchura (width) de 600px y su elemento hijo tiene configurado un width: 80%, ¿cuál es el ancho exacto del elemento hijo en píxeles?
Pregunta 5
Dado un elemento con las siguientes propiedades CSS:
width: 300px
padding: 50px (aplica a todos los lados)
border-width: 10px (aplica a todos los lados)
margin: 30px (aplica a todos los lados)
¿Cuál es el tamaño total del ancho que ocupa dicho elemento en el documento?
Pregunta 6
¿A qué tipo de elementos HTML se pueden aplicar los márgenes verticales (margin-top y margin-bottom)?
Pregunta 7
Explique el fenómeno de la "fusión de márgenes verticales" cuando dos cajas verticales adyacentes entran en contacto.
Pregunta 8
¿Cuáles son los valores posibles que se pueden asignar a la propiedad border-width además de una medida concreta en píxeles? ¿Cuál es su valor inicial?
Pregunta 9
¿Cómo se posiciona por defecto una imagen de fondo (background-image) en una página y qué coordenadas/palabras clave se pueden utilizar para modificar su posición horizontal y vertical?
Pregunta 10
Mencione cuatro tipos de control que se pueden crear mediante la etiqueta <input> en un formulario HTML y explique la función de los atributos disabled y tabindex.
4. Clave de Respuestas Explicada
Respuesta 1
Un elemento en bloque introduce automáticamente un salto de línea antes y después del mismo, ocupando el ancho disponible. Un elemento en línea se coloca a continuación del elemento anterior en la misma línea, sin introducir saltos de línea.
Respuesta 2
De abajo a arriba (capas de fondo a superficie):
Color de fondo (background-color)
Imagen de fondo (background-image)
Relleno (padding - transparente)
Contenido (content)
Borde (border)
Margen (margin - transparente)
La imagen de fondo prevalece sobre el color de fondo porque está situada en una capa superior a este.
Respuesta 3
Al incluir 4 valores, la asignación sigue el orden: superior, derecho, inferior, izquierdo.
Margen superior: 5px
Margen derecho: 33%
Margen inferior: 50px
Margen izquierdo: 0
Respuesta 4
El ancho exacto es 480px. Los valores en porcentaje se calculan sobre la anchura del elemento padre (600\text{px} \times 0.80 = 480\text{px}).
Respuesta 5
El ancho total ocupado es 480px. Cálculo: \text{Margin-left (30px)} + \text{Border-left (10px)} + \text{Padding-left (50px)} + \text{Width (300px)} + \text{Padding-right (50px)} + \text{Border-right (10px)} + \text{Margin-right (30px)} = 480\text{px}
Respuesta 6
Los márgenes verticales únicamente se pueden aplicar a los elementos de bloque y a las imágenes. (A diferencia de los laterales, que se aplican a cualquier elemento).
Respuesta 7
Cuando dos cajas se encuentran en vertical o una está contenida dentro de otra, los márgenes no se suman. En su lugar, se fusionan prevaleciendo un único margen cuyo valor es el más grande de los márgenes implicados.
Respuesta 8
Los valores posibles para border-width son:
Un valor de medida concreto.
thin
medium (que es el valor inicial)
thick
Respuesta 9
Por defecto, la imagen de fondo se coloca desde la esquina superior izquierda de la página (posición 0,0).
Posición Horizontal: Palabras clave (left, right, middle), coordenada concreta (ej. 12px) o relativa (ej. 5%).
Posición Vertical: Palabras clave (top, bottom, center), coordenada concreta (ej. 20px) o relativa (ej. 15%).
Respuesta 10
Tipos de <input>:
text: Campo de texto de una línea.
password: Campo de texto donde los caracteres no son leíbles al escribir.
checkbox: Casilla de verificación para seleccionar/marcar valores.
file: Campo para explorar el ordenador y seleccionar un fichero a enviar.
Atributos:
disabled: Deshabilita el botón o control impidiendo que el usuario pueda pulsar sobre él.
tabindex: Establece el índice de orden de tabulación dentro del formulario.
