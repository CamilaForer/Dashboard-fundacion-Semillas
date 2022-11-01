<h1 align="center">Dashboard Fundación Semillas
<p align="center">
 <img width="170" height="150" src="https://user-images.githubusercontent.com/86115727/199051290-83a2c79f-fcf4-4d98-bc4b-3991362cad80.png">
</p>
</h1> 
<hr>
<p>Para este proyecto la Fundación Semillas (que ofrece diplomados en sostenibilidad del medio ambiente) desea saber el estado de ánimo de sus alumnos, además de querer suministrarles una herramienta de fácil manejo. Para ello, plantea que se desarrolle una aplicación web con varios dashboard, que muestren indicadores sobre las emociones que un alumno puede llegar a sentir durante el desarrollo de la formación por cada actividad que realizan.
<br>
Nuestra propuesta ha sido realizada en HTML y CSS vanilla, para ello realizamos en primera instancia los <a href="https://www.figma.com/file/7UwR9BxDHxLrOEY1okEqdo/Semillas?node-id=0%3A1">wireframes</a>,<a href="https://www.figma.com/file/7UwR9BxDHxLrOEY1okEqdo/Semillas?node-id=2%3A3">mockups</a> y respectivos <a href="https://www.figma.com/proto/7UwR9BxDHxLrOEY1okEqdo/Semillas?node-id=91%3A105&scaling=scale-down&page-id=2%3A3&starting-point-node-id=91%3A24">prototipos</a> en figma, donde planteamos una primera pantalla que nos mostrara los diferentes diplomados que tiene la fundación y una gráfica de las emociones de sus alumnos de manera global para cada diplomado, al entrar al diplomado que se quiera visualizar, esta la opción de elegir a que alumno se quiere revisar. Una vez hecho esto podremos visualizar un dashboard que mostrará gráficos con el nivel de progreso de sus actividades,los niveles exactos de cada emoción y un promedio de la emoción que más predomina. Además se podrá visualizar un pop-up con la gráfica de promedio emocional por mes.
<br> 
Siguiendo los mockups previamente realizados iniciamos con la elaboración del header de la página para lo cual se hizo uso de clip-path, para dar la forma de la barra que contiene el logo y el menú.</p>
<p>Código</p>
<p align="center">
 <img src="https://user-images.githubusercontent.com/86115727/199053964-b7a4af0d-8c74-442c-8305-53f878dab4fc.png">
</p>
Vista
<p align="center"> 
 <img src="https://user-images.githubusercontent.com/86115727/199054333-68511823-6c47-4464-8835-4d8399aea773.png">
</p>
<p>Realizamos las tarjetas de información de los diplomados con sus respectivas graficas</p>
<p align="center"> 
 <img src="https://user-images.githubusercontent.com/86115727/199066331-f90bb584-03f5-4da8-a4e2-ba43a3c6b900.png">
</p>
Cada tarjeta tiene un hover que hace que se mueva un poco hacia arriba facilitando también la vista de la tarjeta a seleccionar.
<p>Código</p>
<p align="center"> 
 <img src="https://user-images.githubusercontent.com/86115727/199073939-055328de-52de-4689-86dd-4dde857adbc9.png">
</p>
Además se añade animación que simula la carga del contenido de las tarjetas
<p align="center"> 
 <img src="https://user-images.githubusercontent.com/86115727/199074290-294862f3-265f-48ec-913c-3c6a94e359d9.png">
</p>

<h3>Vista Diplomado</h3> 
    <h4>Maqueta</h4> 
    <p>Para posicionar el contenido y darle margin se utilizó las clases <b>container</b> y <b>contenido</b>. Internamente se dividio el contenido en dos partes: la primera corresponde a la información del estudiante y la segunda comprende las información gráfica de las emociones por actividad.</p> 
    <p align="center">Código</p> 
    <p align="center"> 
      <img 
        src="https://user-images.githubusercontent.com/92338030/199116824-79b8dbf6-a3f8-443f-a775-43b893f296fc.png" 
      /> 
    </p> 
 <h4>Información del estudiante</h4> 
    <p>Para realizar la gráfica <b>Promedio Emocional 2022</b> se utilizó el formato vectorial <b>SVG</b>. El motivo de esta elección fueron los inconvenientes presentados para crear y posicionar las lineas interiores con los elementos <b>clip-path</b> y la técnica de <b>triángulos con un solo borde</b>.</p> 
    <p align="center">Problema</p> 
    <p align="center"> 
      <img 
        src="https://user-images.githubusercontent.com/92338030/199121173-fa72fba7-bb73-4e43-b568-e450855425b9.PNG" 
        width="470" 
      /> 
    </p>Dentro del elemento SVG se utlizaron dos <b>polyline</b> para los ejes de la gráfica y cinco más para las líneas que representan las emociones. Para la leyenda de los ejes se utilizaron etiquetas se utlizarón las etiquetas <b>g</b> y <b>text</b>. 
    <p align="center">Código</p> 
    <p align="center"> 
      <img 
        src="https://user-images.githubusercontent.com/92338030/199124482-04e7a854-7606-4ba2-92ad-24e6ce5e894a.png" 
        width="470px" 
      /> 
    </p> 
    <p align="center">Vista</p> 
    <p align="center"> 
      <img 
        src="https://user-images.githubusercontent.com/92338030/199127097-03e89f6c-66f0-4480-8f3f-a98ce2207ed3.png" 
        width="470px" 
      /> 
    </p> 
    <h4>Actividades</h4> 
    <p> 
      Para realizar la gráfica de <b>Entregas</b>  se utilizarón las clases : <b>circle-wrap</b> para dar dimensiones y forma al elemento padre (circulo exterior); las clase <b>mask full-1</b> y <b>fill-1</b> para dar la animación de que el circulo se rellena cuando la página se carga y; la clase <b>inside-circle</b> para dar la forma de anillo. 
    </p> 
    <p align="center">Código</p> 
    <p align="center"> 
      <img 
        src="https://user-images.githubusercontent.com/92338030/199245265-33d2af6d-8078-4f9d-b287-2e9b0d607cf4.png" 
        width="470px" 
      /> 
    </p> 
    <p align="center">Vista</p> 
    <p align="center"> 
      <img 
        src="https://user-images.githubusercontent.com/92338030/199245420-d9d51c2f-c44a-4c8f-8679-de05d9643944.png" 
        width="470px" 
      /> 
    </p> 
    <p> 
      Para realizar el <b>Diagrama de Barras de Emociones</b> se crearon las clases <b>board</b> y <b>sub_board</b> para dar dimensiones al contenido. Dentro se ubicaron las barras y la leyenda del eje vertical con las clases <b>graf_board</b>, <b>barra</b>, <b>tag_board</b>, <b>sub_tag_board</b>, entre otras. 
    </p> 
    <p align="center">Código</p> 
    <p align="center"> 
      <img 
        src="https://user-images.githubusercontent.com/92338030/199248499-1c8a195d-c64a-42b3-8639-826c6d84b3e8.png" 
        width="470px" 
      /> 
    </p> 
    <p align="center">Vista</p> 
    <p align="center"> 
      <img 
        src="https://user-images.githubusercontent.com/92338030/199248643-0b183428-8683-4f54-b977-f414cbbd9b35.png" 
        width="470px" 
      /> 
    </p>

Para la grafica de barras se hicieron caritas con ayuda de CSS y un hover que las hace cambiar de color
<p align="center"> 
 <img src="https://user-images.githubusercontent.com/86115727/199075694-e2a91016-a48d-4825-a5c4-14b7c6184937.png">
</p>
<p align="center"> 
 <img src="https://user-images.githubusercontent.com/86115727/199252908-9235de3e-ffe3-45f7-8be8-8b9fb072eb91.png">
</p>


