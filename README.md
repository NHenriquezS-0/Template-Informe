## Template de informe en latex
Este corresponde a un template para confeccionar [geniales informes en latex](https://github.com/ppizarror/Template-Informe/blob/master/Informe.pdf), contiene funciones básicas para agregar imágenes, fórmulas, etc.

<p align="center">
  <img src="https://raw.githubusercontent.com/ppizarror/ppizarror.github.io/master/resources/images/informe/informe_data.png" alt="Informe" width="800px" height="800px"/>
</p>

## Configurando el documento
Para modificar el documento (Título, nombre de la universidad, curso, etc.) se deben modificar las variables definidas en el bloque de *%INFORMACIÓN DEL DOCUMENTO* al principio del documento, estas son del estilo _\newcommand{_**\nombreVariable**_}{_ **Valor**}, entre las cuales se encuentran:
+ **\nombredelinformetitulo**: Título del informe.
+ **\temaatratar**: Tema a tratar.
+ **\fecharealizacion**: Fecha en que se realizó el experimento / informe.
+ **\fechaentrega**: Fecha en que se entregó el informe.
+ **\nombreuniversidad**: Universidad, Instituto, etc.
+ **\nombrefacultad**: Facultad relacionada a la Universidad, Instituto, etc.
+ **\departamentouniversidad**: Departamento de la Universidad.
+ **\imagendeldepartamento**: Imagen del departamento o universidad a usar en la portada, estos se pueden encontrar en la carpeta _/images/departamentos/_. Actualmente existen las siguientes imágenes:
  - **das**: Departamento de Astronomía.
  - **dcc**: Departamento de Ciencias de la Computación.
  - **dfi**: Departamento de Física.
  - **dgf**: Departamento de Geofísica.
  - **dic**: Departamento de Ingeniería Civil.
  - **die**: Departamento de Ingeniería Eléctrica.
  - **dii**: Departamnto de Ingeniería Industrial.
  - **dim**: Departamento de Ingeniería Matemática.
  - **dimec**: Departamento de Ingeniería Mecánica.
  - **diqbt**: Departamento de Ingeniería Química y Biotecnología.
  - **fcfm**: Facultad de Ciencias Físicas y Matemáticas.
  - **geo**: Departamento de Geología.
  - **humanidades**: Área de Humanidades.
  - **minas**: Departamento de Ingeniería en Minas.
+ **\imagendeldepartamentoescl**: Escala de la imagen a usar.
+ **\localizacionuniversidad**: Ciudad o región en donde se ubica la universidad / instituto.
+ **\nombredelcurso**: Curso - Ramo referido al informe.
+ **\codigodelcurso**: Código del curso.

## Configurando otros elementos del documento
También se pueden modificar los márgenes de los títulos de tablas y figuras _(caption)_, el tamaño de los títulos de las secciones, etc. Estas se encuentran en el bloque de *% CONFIGURACIONES*, entre las cuales se encuentran:
+ **\defaultimagefolder**: Directorio de las imágenes, sólo utilizado por las funciones que insertan figuras.
+ **\tipofuentetitulo**: Tamaño por defecto de los títulos.
+ **\tipofuentetitulo**: Tamaño por defecto de los títulos.
+ **\tipofuentesubtitulo**: Tamaño por defecto de los subtítulos.
+ **\tipofuentetituloi**: Tamaño por defecto de los títulos en el índice.
+ **\tipofuentesubtituloi**: Tamaño por defecto de los subtítulos en el índice.
+ **\tiporeferencias**: Tipo de referencias, por defecto se usa la norma APA.
+ **\nombltformulas**: Nombre de la lista de fórmulas.
+ **\nomblttablas**: Nombre de la lista de tablas.
+ **\nombltfiguras**: Nombre de la lista de figuras.
+ **\nombltcontend**: Nombre del índice de contenidos.
+ **\nombltwtablas**: Nombre de las tablas.
+ **\nombltwfigura**: Nombre de las figuras.
+ **\defaultcaptionmargin**: Márgenes de las leyendas por defecto.
+ **\defaultpagemarginleft**: Margen izquierdo de las páginas en centímetros.
+ **\defaultpagemarginright**: Margen derecho de las páginas en centímetros.
+ **\defaultpagemargintop**: Margen superior de las páginas en centímetros.
+ **\defaultpagemarginbottom**: Margen inferior de las páginas en centímetros.
+ **\defaultfirstpagemargintop**: Margen superior de la portada en centímetros.
+ **\defaultmarginfloatimages**: Margen superior de las figuras flotantes en pt.
+ **\defaultmargintopimages**: Margen superior de las figuras en centímetros.
+ **\defaultmarginbottomimages**: Margen inferior de las figuras en centímetros.

## Añadiendo librerías
Las librerías se cargan en la sección *%LIBRERÍAS INDEPENDIENTES* y *%LIBRERÍAS DEPENDIENTES*, en librerías independientes se cargan las librerías que, como bien dice su nombre, no dependen de la previa importación de otras, o que su importación no genera algún error. Las librerías utilizadas son:
+ **amsmath**: Fórmulas matemáticas.
+ **amssymb**: Símbolos matemáticos.
+ **amsthm**: Teoremas matemáticos.
+ **cancel**: Cancelar términos en fórmulas.
+ **caption**: Leyendas (o títulos de objetos).
+ **chngcntr**: Agrega números de secciones a las leyendas *[dependiente]*.
+ **color**: Colores.
+ **easylist**: Listas.
+ **enumitem**: Enumeraciones avanzadas.
+ **fancyhdr**: Encabezados y pié de páginas.
+ **float**: Administrador de posiciones de objetos.
+ **geometry**: Dimensiones y geometría del documento.
+ **graphicx**: Propiedades extra para los gráficos.
+ **hyperref**: Permite añadir enlaces y referencias.
+ **mhchem**:	Fórmulas químicas [versión 4].
+ **multicol**: Múltiples columnas.
+ **multirow**: Añade nuevas opciones a las tablas *[dependiente]*.
+ **lipsum**: Permite crear textos dummy.
+ **longtable**: Permite utilizar tablas en varias hojas.
+ **listings**: Permite añadir código fuente.
+ **setspace**: Cambia el espacio entre líneas.
+ **subfig**: Permite agrupar imágenes.
+ **tikz**: Permite dibujar.
+ **titlesec**: Cambia el estilo de los títulos.
+ **url**: Permite añadir enlaces.
+ **wrapfig**: Permite comprimir imágenes.

## Añadiendo integrantes, profesores, auxiliares y fechas
Esta información de la portada se encuentra en la sección *%INTEGRANTES, PROFESORES Y FECHAS*, en esta se pueden agregar integrantes, profesores, auxiliares, auxiliar de laboratorio, fecha de entrega y realización, etc.

## Insertando figuras, fórmulas, citas y otros
También es posible añadir fórmulas, citas, figuras y otros elementos de forma sencilla, para ello existen las siguientes funciones:
+ **Insertar párrafos y citas**: Para esto existen las siguientes funciones:
  - **\newpar**{*Párrafo*}: Inserta un nuevo párrafo con un salto de linea al terminar.
  - **\newparnl**{*Párrafo*}: Inserta un nuevo párrafo sin un salto de linea al terminar.
  - **\quotes**{*Texto*}: Función simplificada para insertar "citas" sin lidiar con carácteres.
  - **\quotesit**{*Texto*}: Función simplificada para insertar _"citas en itálico"_ sin lidiar con carácteres.
+ **Añadir una imagen**: Las funciones para añadir imágenes requieren del nombre de la imagen (el archivo almacenado en el directorio definido por la variable **\defaultimagefolder**), su escala y su correspondiente título (caption, o leyenda), la syntax para cada una de ellas es:
  - **\insertimage**{*Archivo*}{*Escala*}{*Leyenda*}: Inserta una simple imagen.
  - **\insertimageboxed**{*Archivo*}{*Escala*}{*Leyenda*}: Inserta una imagen recuadrada.
  - **\insertdoubleimage**{*Archivo*}{*Escala 1*}{*Leyenda 1*}{*Dirección de la imagen 2*}{*Escala 2*}{*Leyenda 2*}{*Leyenda general*}: Inserta dos imagenes en un sólo elemento.
  - **\insertimageleft**{*Archivo*}{*Escala*}{*Leyenda*}{*Número de columnas a usar*}: Inserta una imagen alineada a la izquierda, flotante.
  - **\insertimageright**{*Archivo*}{*Escala*}{*Leyenda*}{*Número de columnas a usar*}: Inserta una imagen alineada a la derecha, flotante.
+ **Insertar una fórmula**: Existen dos funciones para añadir fórmulas: _\insertequation_ y _\insertequationcaptioned_, las cuales consideran la fórmula en sí (escrita en forma bruta, sin los $) y la leyenda para la segunda.
    - **\insertequation**{*Fórmula*}: Inserta una fórmula.
    - **\insertequationcaptioned**{*Fórmula*}{*Leyenda*}: Inserta una fórmula con leyenda.
    - **\pow**{*a*}{*b*}: Forma simplificada de añadir una potencia del tipo a^b.
    - **\lpow**{*a*}{*b*}: Forma simplificada de añadir una sub potencia del tipo a_b.
    - **\fracpartial**{*a*}{*b*}: Crea una fracción de derivadas parciales del estilo ∂a/∂b.
    - **\fracdpartial**{*a*}{*b*}: Crea una fracción de derivadas parciales al cuadrado al estilo ∂^2 a/∂b^2.
    - **\fracnpartial**{*a*}{*b*}{*c*}: Crea una fracción de derivadas parciales a la n al estilo ∂^c a/∂b^2.
+ **Insertar títulos sin número, y títulos sin aparecer en el índice**: También pueden añadirse títulos sin que estos se numeren automáticamente, o títulos sin que estos aparezcan en el índice, para ello existen las siguientes funciones:
  - **\newtitleanum**{*Título*}: Inserta un título sin número.
  - **\newsubtitleanum**{*Título*}: Inserta un subtítulo sin número.
  - **\newtitleanumnoi**{*Título*}: Inserta un título sin número sin que aparezca en el índice.
  - **\newsubtitleanumnoi**{*Título*}: Inserta un subtítulo sin número sin que aparezca en el índice.

## Autor
Pablo Pizarro, 2016.

Si tienes alguna sugerencia envíame un correo a: [pablopizarro9@gmail.com](mailto:pablopizarro9@gmail.com), o sencillamente ten la libertad de enviar un _pull request_.
