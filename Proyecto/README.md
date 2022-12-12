# Proyecto <br>

![Texto alternativo](01%20Logotipo.png) <br>

***Autores***: <br>
Ayoub Fehri Boulaadas <br>
Cristian Gil García. <br>
Pedro Sánchez Fernández. <br>
Sarai Besada Pino. <br>


## Hoja de revision

| ***Fecha*** | ***Version*** | ***Descripcion*** | ***Autor*** |
| ----------- | --- | --- | --- |
| 29/11/2022 | 1.0 | Proyecto para el desarrollo de un software de un sistema de informacion interactivo al viajero del transporte público regular de viajeros para la isla de Gran Canaria (Portal web de servicios) mediante procedimiento abierto | FehriGilFernandezBesada | <br>

<br>

## Introducción
En el siguiente documento se especifica los procesos llevados a cabo para el desarrollo de un proyecto software centrado en la implementación de un sistema de información y un portal web para una aplicación sobre el transporte público regular de viajeros para la isla de Gran Canaria. <br>
Además, se aporta información de la Autoridad de Transporte Público de Gran Canaria para facilitar el diseño del portal y sus funcionalidades.Por otra parte, se añaden los requisitos, diagramas, casos de uso e información necesaria para la implementación de todas las partes de la aplicación.

<br>

### Organigrama
![Texto alternativo](Organigrama.drawio.svg) <br>


## Glosario de términos

| ***Fecha*** | ***Versión*** | ***Descripción*** | ***Autor*** |
| --- | --- | --- | --- |
| 29/11/2022 | 1.0 | Diccionario de palabras técnicas que permite disponer de toda la información que pueda crear dudas sobre el proyecto en orden alfabético.| FehriGilFernandezBesada | <br>

| ***Fecha*** | ***Versión*** | ***Término*** |***Descripción*** |***Autor*** |
| --- | --- | --- | --- | --- |
| 29/11/2022 | 1.0 | Alarma | Notificación acerca de los cortes en carreteras, colapso tras algún evento o el retraso de un transporte siendo un usuario registrado. | FehriGilFernandezBesada | <br>
| 02/12/2022 | 1.0 | Operador de transporte | El conductor de cada medio de transporte. | FehriGilFernandezBesada | <br>
| 03/12/2022 | 1.0 | Operador adjudicatario | Los revisores y/o personal de asistencia que añaden información en el vehículo. | FehriGilFernandezBesada | <br>
| 03/12/2022 | 1.0 | Eventos | Monumentos, ocio, competencias deportivas, acontecimientos culturales autonónimos y nacionales. | FehriGilFernandezBesada | <br> 
| 03/12/2022 | 1.0 | Medios de transporte | Atobuses, taxis, barcos y carros tirados por caballos. | FehriGilFernandezBesada | <br> 
| 03/12/2022 | 1.0 | Tiempo de saltos | El tiempo que una incidencia hace que se retrase nuestro medio de transporte,el retrasado generado. | FehriGilFernandezBesada | <br> 
| 03/12/2022 | 1.0 | Medio magnético | Un registro en un disco duro. | FehriGilFernandezBesada | <br> 


# Necesidades del negocio.
## Objetivos del negocio
## Tareas.

# Requisitos del sistema a desarrollar.
En el siguiente apartado se desarrollan los requisitos funcionales y no funcionales necesarios para llevar a cabo el cumpliento del pliego de condiciones del que se debe extraer toda la información necesario para el correcto funcionamiento del software a desarrollar. Además, se muestran también los diagramas de casos de uso, las tablas en detalle de los mismos y el listado de usuarios y casos de uso.

## Requisitos
### Requisitos del portal (A1)

| ***Requisito*** | ***Descripcion*** | ***Tipo*** |
|---|---|---|
| Obtención información Gestor de transporte. | Función la cual se podrá realizar mediante método magnético o soporte a papel, así como el trabajo de campo para la obtención de la información no recogida en otras fuentes. En el caso de que se necesiten medios la AUTGC los facilitará para el mejor desarrollo de las tareas. | Requisito funcional | <br>


### Requisitos del sistema de información (A2)

| ***Requisito*** | ***Descripcion*** | ***Tipo*** |
|---|---|---|
| Obtención información Gestor de transporte. | Función la cual se podrá realizar mediante método magnético o soporte a papel, así como el trabajo de campo para la obtención de la información no recogida en otras fuentes. En el caso de que se necesiten medios la AUTGC los facilitará para el mejor desarrollo de las tareas. | Requisito funcional | <br>
| Obtención información de las Guaguas. | Obtención de datos como las líneas de guaguas, sus recorridos, paradas, horarios planificados de los itinerarios según tipos de día y períodos definidos, las tarifas, restricciones de tráfico, incidencias notificadas, etc. El modelo de datos debe corresponderse con alguno de los estándares europeos definidos por el CEN (comité europeo de normalización). | Requisito funcional | <br>
| Ayuda en línea. | Ayudas en línea para cada proceso | Requisito funcional | <br>
| Calcular distancia entre paradas | Distancia entre dos paradas diferentes. | Requisito funcional | <br>
| Cálculo de tiempos de recorrido | Tiempo que tarda el bus en recorrer desde la parada de inicio hasta la parada final | Requisito funcional | <br>
| Definir transbordo | Indicar las líneas a realizar el transbordo | Requisito funcional | <br>
| Identificación de zonas no transitables | Zonas donde la guagua no puede acceder | Requisito funcional | <br>
| Definir barrios | Definición de cada uno de los barrios de la isla. | Requisito funcional | <br>
| Definir zonas | Definición de cada una de las zonas de la isla. | Requisito funcional | <br>
| Definir municipios | Definición de cada uno de los municipios de la isla. | Requisito funcional | <br>
| Presentación del recorrido. | Mostrar el recorrido de las diferentes líneas. | Requisito funcional | <br>
| Presentación del itinerario recomendación. | Se indicarán entre otros datos, los diferentes tramos que debería recorrer el usuario, el tiempo empleado en recorrer cada uno de ellos, la línea, su descripción y el destino de la línea en la que viajará y, finalmente, el tiempo total del trayecto hasta alcanzar el destino. | Requisito funcional | <br>
| Mostrar paradas y datos asociados. | Conjunto de paradas que conforman la red de transporte incluido datos como localización… | Requisito funcional | <br>
| Ubicar sitios de interés, eventos culturales y turísticos. | Ubicación de los sitios de interés, eventos que puedan haber durante el periodo establecido y sitios turísticos. | Requisito funcional | <br>
| Información adicional paradas. | Se ampliará la información indicando las líneas que pasan por cada una de ellas, su dirección postal, la foto, etc. | Requisito funcional | <br>
| Información adicional a una línea. | Se presentarán sus tarifas, horarios, empresa gestora, incidencias, etc | Requisito funcional | <br>
| Información adicional a itinerario. | Por cada tramo se mostrará el inicio y el fin del mismo. | Requisito funcional | <br>
| Selección de origen y destino. | Se puede obtener según la calle, paradas, barrio, zona, municipio, desde el mapa, evento cultural o sitio de interés turístico. | Requisito funcional | <br>
| Operaciones del mapa. | Operaciones del mapa como acercar, alejar, desplazar, ir al mapa base y centrar. | Requisito no funcional | <br>
| Calculo del itinerario. | Con los datos obtenidos se calcula el itinerario recomendado. | Requisito no funcional | <br>




### Requisitos del sistema del sistema de monitorización de la explotación del transporte (SMET)

| ***Requisito*** | ***Descripcion*** | ***Tipo*** |
|---|---|---|
| Mostrar sobre la cartografia en pantalla la actividad de los peradores |Se debe mostrar en pantalla (que a su vez muestra un mapa), la actividad de los operadores en tiempo real, teniendo la capacidad de registrar situaciones puntuales (fotos de estado) y periodos contínuos de tiempo (películas de estado). | Requisito funcional | <br>
| Visualizar las alarmas de los distintos proyectos de la autoridad | Se deben mostrar las alarmas (notificaciones) de los diversos proyectos de la autoridad de transporte (proyecto de monitorización y venta) que contenga información del sistema de ventas, gestión del título único del transporte (gestión de billetes únicos y su información que no permita la generación de dos iguales), información de adelanto o atraso del paso por parada, el estado de los sistemas (líneas no disponibles o buses fuera de servicio) y otros que se quieran integrar. | Requisito funcional | <br>
| Recibir avisos. | Se debe permitir definir eventos con base en variables y con unas condiciones que permitan generar avisos. | Requisito funcional | <br>
| Examinar el estado de la explotación en tiempo real. | Se debe poder examinar el estado de la explotación en tiempo real para el/los operador/es que prefiera el usuario. | Requisito funcional | <br>
| Visualización y monitorización del sistema | Se debe poder realizar la visualización y monitorización del sistema  en base a los datos que se reciban. Y también, desde los datos que puedan estar almacenados previamente, y que podrían enviarse al sistema para ser visualizados a posteriori, especificando un rango de fecha, hora, operador y tiempo de salto. Debe ser posible redefinir todas las notificaciones y validar los eventos recibidos y procesados. | Requisito funcional | <br>
| Claridad en contraste de la información. |En particular el sistema debe poner de manifiesto de modo claro y sin complejidad el nivel de cumplimiento de lo planificado respecto a lo realizado.   | Requisito no funcional | <br>
| Visualización de alarmas (notificaciones) simultáneas |Las alarmas (notificaciones) deben ser simultáneas en los distintos proyectos y se deben manifestar mediante avisos acústicos, visuales y mediante notificaciones a móviles aparte de otras a considerar. | Requisito no funcional | <br>


## Casos de uso
### Diagramas de casos de uso
#### Diagrama del portal.
#### Diagrama del  sistema interactivo de información del transporte. SIIT (A2).
| ***UC-01*** |  |
| --- | --- |
| ***Nombre:***  | Realizar Consulta |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 12/12/22 |
| ***Descripcion:*** | Realizar una consulta del trayecto a realizar. |
| ***Relaciones*** | UC-00 |
| ***Actores:***  |  Usuario Logueado y Usuario Invitado. |
| ***Precondicion:*** | <br> |
| ***Flujo Normal:*** | 1. Acceso a la realizacion de la consulta. |
|***Flujo Alternativo:*** | <br> |
| ***Poscondiciones :*** | <br>  |
<br>

| ***UC-02*** |  |
| --- | --- |
| ***Nombre:***  | Introducir Parametros |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 12/12/22 |
| ***Descripcion:*** | Introducir los parametros necesarios para que el sistema pueda ofrecer la ruta optima. |
| ***Relaciones*** | UC-00 |
| ***Actores:***  |  Usuario Logueado y Usuario Invitado. |
| ***Precondicion:*** | <br> |
| ***Flujo Normal:*** | 1. Introduccion origen y destino. <br>2. Introduccion de fecha y hora.<br> 3. Actor pulsa un boton para guardar los parametros |
|***Flujo Alternativo:*** | 1.A. El sistema comprueba que los datos corresponde con lo esperado<br> 
2.A. El sistema comprueba que la fecha introducida es correcta|
| ***Poscondiciones :*** | <br>  |
<br>

| ***UC-02*** |  |
| --- | --- |
| ***Nombre:***  | Introducir Parametros |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 12/12/22 |
| ***Descripcion:*** | Introducir los parametros necesarios para que el sistema pueda ofrecer la ruta optima. |
| ***Relaciones*** | UC-00 |
| ***Actores:***  |  Usuario Logueado y Usuario Invitado. |
| ***Precondicion:*** | <br> |
| ***Flujo Normal:*** | 1. Introduccion origen y destino. <br>2. Introduccion de fecha y hora.<br> 3. Actor pulsa un boton para guardar los parametros |
|***Flujo Alternativo:*** | 1.A. El sistema comprueba que los datos corresponde con lo esperado<br> 
2.A. El sistema comprueba que la fecha introducida es correcta|
| ***Poscondiciones :*** | <br>  |
<br>

| ***UC-03*** |  |
| --- | --- |
| ***Nombre:***  | Introducir origen y destino |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 12/12/22 |
| ***Descripcion:*** | Introduccion del origen y del destino por medio de las diferentes opciones ofertadas: calle y numero, detalle paradas, barrio, zona, municipio, desde el mapa o a partir de un evento cultural |
| ***Relaciones*** | UC-00 |
| ***Actores:***  |  Usuario Logueado y Usuario Invitado. |
| ***Precondicion:*** | <br> |
| ***Flujo Normal:*** | 1. Eleccion del metodo de introduccion de los datos. <br>2. Seleccion del origen y destino. |
|***Flujo Alternativo:*** | 2.A. El sistema comprueba que los datos se encuentran en el territorio contemplado |
| ***Poscondiciones :*** | <br> |
<br>

| ***Código*** | ***Actor*** | ***Descripción*** |
|---|---|---|
| ACT-01 | Usuario invitado | Usuario que no se encuentra registrado en el sistema y hace uso de las funcionalidades de la app que no requieren de estar logueado. |<br>
| ACT-02 | Usuario logueado | Usuario cuyas credenciales ya se encuentran dentro del sistema y, por lo tanto, tiene la posibilidad de loguearse podiendo así hacer uso de ciertas funcionalidades que lo requieren y disfrutan de otros beneficios. |<br>
| ACT-03 | Subcontratado | Trabajador de una empresa externa expresamente contratado para el ofrecimiento de ayudas en linea a los usuarios. |<br>


#### Diagrama del sistema del sistema de monitorización de la explotación del transporte (SMET).
![Texto alternativo](/out/Proyecto/source/Sistema%20de%20Informacion/Sistema%20de%20infirmacion.svg) <br>
### Lista general de casos de uso y actores.
| ***Caso de uso*** | ***Descripción*** |
|---|---|
<br>

| ***Código*** | ***Actor*** | ***Descripción*** |
|---|---|---|
| ACT-01 | Usuario invitado | Usuario que no se encuentra registrado en el sistema y hace uso de las funcionalidades de la app que no requieren de estar logueado. |<br>
| ACT-02 | Usuario logueado | Usuario cuyas credenciales ya se encuentran dentro del sistema y, por lo tanto, tiene la posibilidad de loguearse podiendo así hacer uso de ciertas funcionalidades que lo requieren y disfrutan de otros beneficios. |<br>
| ACT-03 | Administrador | Usuario con beneficios especiales que desempeñan la administración del sistema interacitivo de información del transporte y del portal. |<br>
| ACT-04 | Operador adjudicatario | Usuario con beneficios especiales que desempeñan la administración del sistema de monitorización de la explotación del transporte. |<br>
| ACT-05 | Operador de transporte | Usuario o usuarios encargados de operar los distintos transportes disponibles pertenecientes a la Autoridad Única de Transporte de Gran Canaria. |<br>

<br>

### Detalles de los casos de uso
<br>

## Diagramas de clase asociados a los requisitos de información

<br>

# Apéndices
## Entrevista
| ***Ficha de entrevista*** | |
|---| --- |
| ***Desarrollo de la entrevista*** | Técnico Rafa Bravo |
| ***Tiempo seg/min*** | ***Pregunta/tema tratado*** |
|  | P:¿Es necesario registrarse?¿Es una opción? <br> R: Depende de la funcionalidad que estemos hablando. Para ver la noticias no hace falta loguearse, pero para subir noticias sí. |
|  | P:¿De qué medios de transporte se podrá ver horarios y demás información? Medios por carretera, pero ¿cuáles? <br> R: Hoy estamos usando solo buses, pero van a entrar buses como los taxis y unos inter barcos que tenemos entre las distintas islas. Tiempo parada por donde van, por donde están circulando. También tenemos carros tirados por caballos y no estoy seguro de si eso está controlado o no, tenéis que preguntar a otra persona. |
|  | P:¿Qué tipo de eventos estamos tratando? <br> R: En principio, eventos y monumentos, por donde se pasa por las rutas. En el portal web solamente, las noticias que se pongan se van a estar relacionadas con cosas de ocio, eventos de un partido de fútbol, todo relacionado con las Islas Canarias. |
|  | P:¿Las notificaciones de qué nos deben avisar? <br> R: Cuando haces búsquedas de rutas, os debe avisar de cortes en la carretera, o por culpa de algún evento hay un colapso y los transporte sufren un retraso. En el momento en el que selecciones esa ruta se te avisará si eres un usuario registrado y tienes puesto un número de teléfono. |
|  | “Deberá ser posible examinar el estado de la explotación en tiempo real para cada operador por separado o en conjunto o en la combinación de operadores que se prefiera por el usuario-.” <br> P:¿A qué se refiere exactamente con la explotación en tiempo real de operadores? <br> R: Los operadores son los conductores de cada medio de transporte, o revisores, o personal de asistencia. |
|  | “Se debe poder examinar el estado de la explotación en tiempo real para el/los operador/es que prefiera el usuario.” <br> P:¿Puede el usuario ver qué operadores están disponibles en todo momento y acaso tienen una valoración o algo similar ? <br> R: Pues no lo habíamos pensado, pero sería interesante que los usuarios pudieran puntuar a los operadores. |
|  | “Calcular distancias entre paradas, definir transbordos, calcular tiempos de recorrido, -identificar zonas por las que no se puede transitar y deben ser rodeadas-” <br> P: ¿Este tipo de información será visible también para el usuario normal o sólo para el gestor de transporte? <br> R: Hay que avisar al conductor para que no pase por esa calle, y se debe avisar a los usuarios por si quieren bajar en una parada que está cortada la calle. |