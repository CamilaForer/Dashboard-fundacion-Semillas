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



Para la grafica de barras se hicieron caritas con ayuda de CSS y un hover que las hce cambiar de color
<p align="center"> 
 <img src="https://user-images.githubusercontent.com/86115727/199075694-e2a91016-a48d-4825-a5c4-14b7c6184937.png">
</p>

