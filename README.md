# Práctica HTML-CSS
##### Bootcamp Web Developer Full Stack

## Por dónde empezar
La web no tiene por el momento una <i>home</i>, así que  **Bio** actúa como tal a través del archivo **index.html**. Para acceder al site, se puede cargar con Live Server ese fichero o cualquiera de los dos que hay en la carpeta vistas. La web también está **desplegada en GitHub**. Puedes verla [aquí][web].

[web]: https://adrianfsn.github.io/practica_HTML_CSS/index.html

## Mobile first y media queries
El proyecto está pensado <i> mobile first</i>, construido a partir de un tamaño de dispositivo de 425 px. Al no tener menú hamburguesa todavía para la versión móvil, tendrás que ampliar a una vista de al menos 768 px para poder navegar desde el inspector. Si no, puedes abrir con Live Server los tres archivos .html disponibles.

Las <i>media queries</i> que he añadido a los .css van desde:

* Por encima de...
    * 768 px: banner, bio, components, footer, header, porfolio
    * 1024 px: banner, bio, header, porfolio
    * 1440 px: banner, bio, porfolio

## Imágenes responsive
Dejando aparte el logo del <i>header</i> y el <i>footer</i>, hay imágenes en **Bio** y en **Porfolio**. He usado [Responsive Breakpoints][ResPo] para generar distintos tamaños y densidades de píxeles. Después, la web los "sirve" automáticamente, por lo que he podido testear en el inspector al bajar la densidad.

He limitado el tamaño de la foto más grande que se puede mostrar para cada dispositivo.

[ResPo]: https://www.responsivebreakpoints.com/

## Header
En la versión móvil, el logo se sitúa en el centro y los enlaces desaparecen. En el futuro, me gustaría poner un menú hanburguesa debajo del logo, que está enlazado con la página **Bio (index)**.

Al pasar a 768 px, aparecen los **enlaces**. El hover de todos ellos está suavizado con una transición para el color de la fuente y una animación para el borde inferior de la caja que los contiene. Los enlaces **Bio (en este caso solo cuando clicamos desde la propia página index)** y **Banner** tienen un ancla para llevar la vista a su sección correspondiente. El <i>scroll</i> que lleva hasta ellos también está suavizado.

El **botón** también tiene una transición suave tanto del fondo como del texto.

## Página Bio (index)
Con texto de introducción y barras para ilustrar las habilidades. Es posible que tengas que recargar la página para ver las barras moverse.

Esta página también lleva incrustado el **banner**. La imagen de fondo es diferente para la versión móvil de la de tamaños superiores.

## Página Porfolio
Comienza con un <i>fade-in</i> de un vídeo en bucle. Para reducir el tamaño de ese elemento, he utilizado [Online Convert][OConvert].

El vídeo es cuadrado, por lo que en el móvil ocupa toda la pantalla. Para mejorar su aspecto en dispositivos más grandes, he creado un fondo con un gradiente. Es un efecto sutil, puesto que la mayor parte del gradiente queda por detrás del vídeo, haciendo un leve halo a su alrededor.

El porfolio se basa en imágenes. Al superar los 768 px, su disposición pasa de un <i>grid</i> de una columna con una única foto, a dos columnas con dos elementos cada una.

Esas imágenes tienen una pequeña transición al pasar el cursor sobre cada una de ellas. Aparece un borde rojo a su derecha.

[OConvert]: https://video.online-convert.com/es/convertir-a-mp4#j=1c8bb88c-67c4-4875-a659-bf9aee907e25

## Página Contacto
El formulario está organizado en diferentes <i>fieldsets</i> que agrupan varias parejas de elementos. Creo que es útil tanto para el diseño como para agrupar temas: datos personales, forma de contactar...

Los botones del formulario tienen un aspecto diferente al del <i>header</i> y el <i>footer</i>, para no recargar demasiado el diseño. Sus <i>hover</i> están suavizados y estilizados.

Al pasar de móvil a pantallas más amplias, el formulario deja de ser un <i>block</i> y se convierte en una cuadrícula de dos columnas. Las parejas de elementos agrupadas en cada <i>fieldset</i> están en contenedores <i> flex</i>, que ocupan el tamaño de las dos columnas o solo de una, según sea necesario.

## Footer
Los iconos sociales los obtuve en [Font Awesome][FoAw]. Están enlazados a mi Linkedin y mi Instagram (este último hace siglos que no lo uso).

El logo está enlazado con la página **Bio (index)**.

[FoAw]: https://fontawesome.com/

## Colores y fuentes
He usado una paleta de tres colores. Puedes encontrarla en la carpeta **Tools** con el nombre Paleta 2.

Las fuentes son de [Google Fonts][GoFo], pasadas por [Google-webfonts-helper][GoFoHe]. Para los títulos, uso **Bebas Neue**. En el resto de textos empleo **Inconsolata**.

[GoFo]: https://fonts.google.com/
[GoFoHe]: https://gwfh.mranftl.com/fonts

## Diseño en general
He tratado de dar a la web un estilo retro, por la elección de los colores negro y sepia, las fotos en escala de grises y la fuente Inconsolata. También, algo llamativo o atrevido, con el rojo, la alineación de los h1 a la derecha y el tono irónico del contenido del porfolio; pero sin quitarle seriedad y (espero) elegancia.
