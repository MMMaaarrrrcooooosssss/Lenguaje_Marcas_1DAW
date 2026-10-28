Prefiero el flex porque parece más compacto

Si pongo display none desaparece

padding (relleno): Es el espacio interno comprendido entre el contenido del elemento y su propio borde. Es un espacio transparente en el que se muestra el color o la imagen de fondo definidos para el propio elemento.
margin (margen): Es el espacio libre externo situado fuera del borde, encargado de separar la caja de los elementos vecinos adyacentes o de las paredes de su contenedor. Es transparente y deja ver el fondo del elemento padre.

Por defecto, la etiqueta <div> es un elemento a nivel de bloque (display: block) y, por naturaleza, introduce un salto de línea antes y después, impidiendo que otros elementos se situen a su lado.
Si las tarjetas se alinearon en horizontal usando display: inline-block o float, la causa del salto se debe a que el tamaño real de cada caja en el documento comprende la suma total de width + padding + border + margin. Si la suma acumulada de las tres tarjetas excede los 800 px de ancho del contenedor padre, la tercera caja no tiene espacio para encajar y salta a la fila inferior.

El elemento <span> es un contenedor genérico que se comporta por defecto como un elemento en línea (display: inline).
Propiedades que ignora: márgenes verticales, ancho y alto
Las ignora porque la función de los elementos en línea es adaptarse y fluir dentro de una línea de texto de forma continua sin romperla, ocupando únicamente el espacio estricto que requiere la visualización de sus contenidos.

Al asignar display: none; a un elemento, este queda oculto junto con sus hijos y el espacio que ocupaba la caja se retira completamente de la página.
A diferencia de otras propiedades de ocultación (como visibility: hidden, que mantiene el hueco reservado), los demás elementos de la estructura web se desplazan para ocupar el lugar libre que ha dejado la caja eliminada.
