# Horarios
En una universidad, el personal del PDI, el personal del PAS y los estudiantes pueden consultar horarios. Por su parte, el personal del PAS puede modificar horarios y dar de alta estudiantes. El personal de PDI puede proponer cambios en los horarios y dar de alta estudiantes. La funcionalidad de dar de alta estudiantes del PAS realiza una verificación de los datos del estudiante. Sin embargo, la funcionalidad de dar de alta estudiantes del PDI, además de verificar los datos también permite de forma excepcional realizar la búsqueda en las listas de clase de sus asignaturas.

## Diagrama de Horarios
![Texto alternativo](../../out/lab0/source/Horarios/Horarios.svg)

## Digrama entidad relación de horarios
![Texto alternativo](../../out/lab1/source/HorariosEntidadRelacion/Horarios.svg)

## Tablas de casos de uso de Horarios.

| ***UC-01*** |  |
| --- | --- |
| ***Nombre:***  | Proponer cambios en el horario. |
| ***Autor:***  | Fehri Gil Fernandez Besada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El personal PDI puede proponer cambios en el horario. |
| ***Relaciones*** | INF-01,INF-03 |
| ***Actores:***  | <br>  PersonalPDI. |
| ***Precondicion:*** |  <br>  El personal PDI debe estar logueado. |
| ***Flujo Normal:***  | <br>  1. El personal PDI debe pulsar un boton para modificar el horario. <br> 2. El actor rellena un formulario con los cambios realizados. <br> 3. El actor pulsa un botón para confirmar los cambios. |
| ***Flujo Alternativo:*** | <br>  1. Si al confirmar no se actualiza el horario vuelve a mostrar el formulario. <br> 2. Si no se rellena el formulario se mostrará un mensaje de error. |
| ***Poscondiciones*** | <br>   |


| ***UC-02*** |  |
| --- | --- |
| ***Nombre:***  | Consultar horarios. |
| ***Autor:***  | Fehri Gil Fernandez Besada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El usuario puede comprobar el horario correspondiente |
| ***Relaciones*** | INF-01 |
| ***Actores:***  | <br>  Estudiantes. |
| ***Precondicion:*** |  <br>  El estudiante debe de tener sus datos personales en la universidad y por tanto estar dado de alta. |
| ***Flujo Normal:***  | <br>  1. El estudiante accede a la pestaña de horario. <br> 2. El estudiante debe de elegir el dia y el mes. <br> 3. El actor pulsa un botón para el envio del formulario. <br> 4. El sistema comprueba que los datos introducidos. <br> 5. Visualizacion del horario. |
|***Flujo Alternativo:*** | <br> 4.A.- El sistema comprueba que los datos introducidos son correctos, en caso de que en el dia no haya ninguna clase se enviara un mensaje de error.<br>4.B.- El sistema comprueba que los datos introducidos son correctos, en caso de que los datos no lo sean, se avisara al usuario que los corrija.|
|***Postcondiciones*** | <br>  |
<br>

| ***UC-03*** |  |
| --- | --- |
| ***Nombre:***  | Modificar horarios. |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El personal PAS puede modificar los horarios. |
| ***Actores:***  | <br>  PersonalPAS. |
| ***Precondicion:*** | <br>  El personal PAS debe estar logueado como PAS. |
| ***Relaciones*** | INF-03 |
| ***Flujo Normal:*** | <br>  1. El personal PAS debe pulsar un boton para modificar el horario. <br> 2. El actor rellena un formulario con cajas de texto para los nuevos cambios realizados. <br> 3. El actor pulsa un botón para confirmar los cambios. |
|***Flujo Alternativo:*** | <br> 2A. El sistema comprueba los datos del formulario y si no son correctos pide corrección |
| ***Poscondiciones :*** | <br> El horario se ha modificado |

| ***UC-04*** |  |
| --- | --- |
| ***Nombre:***  | Dar alta estudiantes (PDI) |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El personal PDI puede dar de alta a estudiantes. |
| ***Relaciones*** | UC-05,UC-06 |
| ***Actores:***  | <br>  PersonalPDI. |
| ***Precondicion:*** | <br>  El personal PDI debe estar logueado como PDI. |
| ***Flujo Normal:*** | <br>  1. El personal PDI debe pulsar un boton para elegir la opcion de dar alta a un estudiante. <br> 2. El actor rellena un formulario con cajas de texto para los datos del estudiante que se va a dar de alta. <br> 3. El actor pulsa un botón para confirmar los cambios. <br> 4. Los datos de los estudiantes deberan ser verificados por el sistema. |
|***Flujo Alternativo:*** | <br> 2A. Si en los datos existen correlacion con un alumno el personal puede buscar en las listas de clase. <br> 2B. El sistema comprueba los datos del formulario y si no son correctos pide corrección. |
| ***Poscondiciones :*** | <br> El estudiante ha sido dado de alta. |
<br>

| ***UC-05*** |  |
| --- | --- |
| ***Nombre:***  | Buscar en listas de clase. |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El personal PDI de manera opcional puede buscar en las listas de clase. |
| ***Relaciones*** | UC-04 |
| ***Actores:***  | <br>  PersonalPDI. |
| ***Precondicion:*** | <br>  El personal debe estar logueado como PDI |
| ***Flujo Normal:*** | <br>  1. El personal PDI debe dar de alta a un alumno. <br> 2. El personal PDI puede utilizar la opcion en las listas si existen correlaciones con los datos de los alumnos <br> 3. El actor pulsa un botón para confirmar los cambios. |
|***Flujo Alternativo:*** | <br> 2A. El sistema comprueba los datos del formulario y si no son correctos pide corrección |
| ***Poscondiciones :*** | <br>  |
<br>

| ***UC-06*** |  |
| --- | --- |
| ***Nombre:***  | Dar alta estudiantes |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El personal PAS puede dar de alta a estudiantes. |
| ***Relaciones*** | UC-04 |
| ***Actores:***  | <br>  PersonalPAS. |
| ***Precondicion:*** | <br>  El personal PAS debe estar logueado como PAS. |
| ***Flujo Normal:*** | <br>  1. El personal PAS debe pulsar un boton para elegir la opcion de dar alta a un estudiante. <br> 2. El actor rellena un formulario con cajas de texto para los datos del estudiante que se va a dar de alta. <br> 3. El actor pulsa un botón para confirmar los cambios. <br> 4. Los datos de los estudiantes deberan ser verificados por el sistema. |
|***Flujo Alternativo:*** | <br> 4A. El sistema verifica los datos y comprueba que son erroneos por lo que se muestra un mensaje al personal PAS. |
| ***Poscondiciones :*** | <br> El estudiante ha sido dado de alta. |
<br>

## Tablas de los requisitos de información de Horarios

| ***INF-01*** | Usuarios del sistema. |
| --- | --- |
| ***Version:***  | Septiembre-2022 |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Referencias:*** | <br> Estudiante, PersonalPDI, personalPAS. |
| ***Fuentes:***  | <br>  Horarios.   |
| ***Descripción*** | <br> El sistema deberá almacenar los datos correspondientes a todos los usuarios del sistema. |
| ***Datos especificos:*** |  1. DNI/NIE: Cadena de máximo 10 caracteres. <br> 2. Nombre completo: Cadena de máximo 30 caracteres. <br> 3.Teléfono de contacto: Entero positivo. <br> 4. Sexo: Un carácter "F" o "M" <br>  |
| ***Importancia:*** | <br> Muy importante. |
| ***Estado:*** | <br> Aceptado. |
| ***Comentarios:*** | <br> Los datos de los usuarios del sistema son imprescindibles en el correcto funcionamiento del sistema.|
<br>

| ***INF-02*** | Información sobre altas de los estudiantes |
| --- | --- |
| ***Version:***  | Septiembre-2022 |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Referencias:*** | <br> Dar alta estudiantes. |
| ***Fuentes:***  | <br>  Horarios.   |
| ***Descripción*** | <br> El sistema deberá almacenar los datos necesarios para dar de alta a los estudiantes. |
| ***Datos especificos:*** |  1. Nombre completo del estudiante: Cadena. <br> 5. Asignaturas cursadas del estudiante: Cadena. <br>   |
| ***Importancia:*** | <br> Muy importante. |
| ***Estado:*** | <br> Aceptado. |
| ***Comentarios:*** | <br> |
<br>

| ***INF-03*** | Información sobre horarios. |
| --- | --- |
| ***Version:***  | Septiembre-2022 |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Referencias:*** | <br> Consultar horarios, Modificar horarios, Proponer cambios en los horarios. |
| ***Fuentes:***  | <br>  Horarios. |
| ***Descripción*** | <br> El sistema deberá almacenar los datos correspondientes a los horarios de las distintas asignaturas. |
| ***Datos especificos:*** |  1. Nombre de las Asignaturas: Cadena. <br> 2. Rango de horas en la que se imparte cada asignatura: Cadena con la siguiente información, hh-mm/hh-mm <br> 3.Día en el que se imparte la asignatura: Cadena  |
| ***Importancia:*** | <br> Muy importante. |
| ***Estado:*** | <br> Aceptado. |
| ***Comentarios:*** | <br> El horario es imprescindible para el correcto funcionamiento del sistema.|
<br>

| ***INF-04*** | Información sobre asignaturas. |
| --- | --- |
| ***Version:***  | Septiembre-2022 |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Referencias:*** | <br> Consultar horarios, Modificar horarios, Proponer cambios en los horarios. |
| ***Fuentes:***  | <br>  Horarios. |
| ***Descripción*** | <br> El sistema deberá almacenar los datos correspondientes a las distintas asignaturas. |
| ***Datos especificos:*** |  1. Nombre: Cadena. <br>  |
| ***Importancia:*** | <br> Muy importante. |
| ***Estado:*** | <br> Aceptado. |
| ***Comentarios:*** | <br> Las asignaturas son imprescindible para el correcto funcionamiento del sistema.|

| ***INF-05*** | Información sobre lista de clase. |
| --- | --- |
| ***Version:***  | Septiembre-2022 |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Referencias:*** | <br> Consultar horarios, Modificar horarios, Proponer cambios en los horarios. |
| ***Fuentes:***  | <br>  Horarios. |
| ***Descripción*** | <br> El sistema deberá almacenar los datos correspondientes a las listas de clases. |
| ***Datos especificos:*** |  1. Nombre de la Asignatura: Cadena. <br>  2. Nombre de los estudiantes: cadena. |
| ***Importancia:*** | <br> Muy importante. |
| ***Estado:*** | <br> Aceptado. |
| ***Comentarios:*** | <br> |

# Sistema de compras
En un sistema de compra, existen cuatro tipos de usuarios: comprador, vendedor, proveedor y administrador. Los compradores pueden agregar productos, consultar precios, finalizar la compra y consultar ofertas. Agregar productos implica marcar esos productos como bloqueados. Los vendedores también pueden consultar ofertas y consultar precios. Los proveedores pueden consultar precios, avisar de nuevos productos y consultar ofertas. Avisar de nuevos productos, de forma excepcional, realiza la incorporación de una oferta. Los proveedores también tienen una funcionalidad para avisar del fin de una oferta. Cuando se avisa del fin de una oferta, se ejecuta la funcionalidad de eliminar la oferta. Ambas funcionalidades de avisar del proveedor tienen en común que se encarga de enviar una notificación. Los administradores pueden consultar precios, consultar ofertas y eliminar productos. La funcionalidad de consultar precios incluye una funcionalidad de buscar productos que es similar a la funcionalidad de consultar productos de los compradores. Sin embargo, la funcionalidad de consultar productos añade una funcionalidad para verificar la disponibilidad. Para realizar una venta, un comprador y un vendedor participan de forma conjunta. En dicha operación, se lleva a cabo el acuerdo de un precio; excepcionalmente, durante la realización de la venta, se consultará el histórico de ventas.

## Diagrama de Sistema de compras.
![Texto alternativo](../../out/lab0/source/Sistema%20De%20Compras/Sistema%20de%20compras.svg)

## Diagrama de entidad relación de Sistema de compras
![Texto alternativo](../../out/lab1/source/SistemaComprasEntidadRelacion/Sistema.svg)

## Tabla de casos de uso de Sistema de compras

| ***UC-01*** |  |
| --- | --- |
| ***Nombre:***  | Finalizar compra |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El comprador puede finalizar una compra. |
| ***Relaciones*** | INF-02 |
| ***Actores:***  | <br>  Comprador |
| ***Precondicion:*** | <br>  El comprador debera haber agredado productos |
| ***Flujo Normal:*** | <br>  1. El comprador debera introducir la opcion de finalizar la compra. <br> 2. Se procesan los datos de los artículos selecionados y se pasa a las opciones de pago <br> 3. Se rellenan los formularios de las opciones de pago. <br> 4. Se comprueba la informacion de pago. <br> 5. Se realiza la transaccion.  |
|***Flujo Alternativo:*** | <br> 4A. La informacion de los datos de pago son erroneos y se informa al comprador |
| ***Poscondiciones :*** | <br> Se guarda en el sistema el registro de la compra. |
<br>

| ***UC-02*** |  |
| --- | --- |
| ***Nombre:***  | Agregar productos. |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El comprador puede agregar productos de su compra. |
| ***Relaciones*** | INF-04,INF-06 |
| ***Actores:***  | <br>  Comprador. |
| ***Precondicion:*** | <br>  Los productos deben mostrarse disponibles. |
| ***Flujo Normal:*** | <br>  1. El comprador puede seleccionar un producto clickando sobre el. <br> 2. El producto se agrega a la cesta de productos de la compra. <br> 3. El producto se bloquea. |
|***Flujo Alternativo:*** | <br>  |
| ***Poscondiciones :*** | <br> El producto ha sido agregado. |
<br>

| ***UC-03*** |  |
| --- | --- |
| ***Nombre:***  | Consultar productos. |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El comprador puede consultar algunos productos |
| ***Relaciones*** | UC-04, UC-06 |
| ***Actores:***  | <br>  Comprador. |
| ***Precondicion:*** | <br>  El producto tiene que estar disponible. |
| ***Flujo Normal:*** | <br>  1. Los actores deben introducir la id o palabra clave en el motor de busqueda. <br> 2. El sistema muestra informacin relacionada con los datos introducidos en el buscador. <br> 2. El sistema comprueba la disponibilad del producto <br> 3. El sistema ofrece informacion del producto consultado |
|***Flujo Alternativo:*** | <br> 3A. Si el producto no esta disponible, se muestra un mensaje advirtiendo de esto el comprador. |
| ***Poscondiciones :*** | <br>  |
<br>

| ***UC-04*** |  |
| --- | --- |
| ***Nombre:***  | Buscar productos. |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El comprador puede buscar productos y consultar su información. |
| ***Relaciones*** | INF-04 |
| ***Actores:***  | <br>  Comprador, Abstracto. |
| ***Precondicion:*** | <br>  El producto debe existir en el sistema. |
| ***Flujo Normal:*** | <br>  1. Los actores deben introducir la id o palabra clave en el motor de busqueda. <br> 2. El sistema muestra información relacionada con los datos introducidos en el buscador. |
|***Flujo Alternativo:*** | <br> 2A. El sistema no encuentra correlaciones con los datos introducidos e informa al usuario |
| ***Poscondiciones :*** | <br> El sistema ha mostrado un mensaje al usuario. |
<br>

| ***UC-05*** |  |
| --- | --- |
| ***Nombre:***  | Realizar venta. |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
<<<<<<< HEAD
| ***Descripcion:*** | <br> El comprador puede realizar la compra tras hablar . |
| ***Actores:***  | <br>  Comprador, Vendedor. |
| ***Precondicion:*** | <br>  Vendedor y comprador deben haber acordado un precio. |
| ***Flujo Normal:*** | <br>  1. El comprador debe tener sus productos agregados. <br> 2. El vendedor y el comprador acuerdan el precio.  <br> 3. Llegan a un acuerdo para poder finalizar la compra. |
|***Flujo Alternativo:*** | <br> 3A. Si el comprador no acepta el precio no se llegaria a realizar la compra. |
| ***Poscondiciones :*** | <br>  |
<br>
=======
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El comprador y el vendedor pueden realizar una venta simultaneamente. |
| ***Relaciones*** | UC-08  |
| ***Actores:***  | <br>  Comprador, Vendedor. |
| ***Precondicion:*** | <br>  El comprador y el vendedor necesitan realizar esta funcion simultaneamente. |
| ***Flujo Normal:*** | <br>  1. Los actores deben introducir la id o palabra clave en el motor de busqueda. <br> 2. El sistema muestra informacin relacionada con los datos introducidos en el buscador.<br> 3. Ambos actores deben acordar un precio. <br> 4. Se realiza la compra y se registra en el sistema <br> |
|***Flujo Alternativo:*** | <br> 2A. El sistema no encuentra correlaciones con los datos introducidos e informa al usuario |
| ***Poscondiciones :*** | <br> El sistema ha mostrado un mensaje al usuario.  |

<br>


| ***UC-06*** |  |
| --- | --- |
| ***Nombre:***  | Verificar disponibilidad |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El sistema comprueba la disponibilidad de los productos consultados. |
| ***Relaciones*** | UC-03 |
| ***Actores:***  | <br>  Comprador. |
| ***Precondicion:*** | <br>  El comprador consulta productos. |
| ***Flujo Normal:*** | <br>  1. El comprador realiza la busqueda del producto a consultar. <br> 2. El sistema comprueba la disponibilad del producto <br> 3. El sistema ofrece informacion del producto consultado |
|***Flujo Alternativo:*** | <br> 3A. Si el producto no esta disponible, se muestra un mensaje advirtiendo de esto el comprador. |
| ***Poscondiciones :*** | <br>  |
<br>


| ***UC-07*** |  |
| --- | --- |
| ***Nombre:***  | Marcar productos bloqueados |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El sistema comprueba la disponibilidad de los productos consultados. |
| ***Relaciones*** | UC-02, UC-03 |
| ***Actores:***  | <br>  Comprador. |
| ***Precondicion:*** | <br>  Un producto debe estar disponible |
| ***Flujo Normal:*** | <br>  1. El comprador puede seleccionar un producto clickando sobre el. <br> 2. El producto se agrega a la cesta de productos de la compra. <br> 3. El producto se bloquea. |
|***Flujo Alternativo:*** | <br> 2A. El producto no esta disponible e informa al comprador. |
| ***Poscondiciones :*** | <br> El producto ha sido bloqueado. |

<br>

| ***UC-08*** |  |
| --- | --- |
| ***Nombre:***  | Acordar un precio |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> Vendedor y comprador acuerdan un precio para un producto |
| ***Relaciones*** | UC-05, UC-06 |
| ***Actores:***  | <br>  Comprador, Vendedor. |
| ***Precondicion:*** | <br>  Un producto debe estar disponible |
| ***Flujo Normal:*** | <br>  1. El vendedor establece un precio inicial. <br> 2. El comprador acepta el precio. |
|***Flujo Alternativo:*** | <br> 2A. El comprador no acepta el precio y se debe establecer otro o finalizar compra. <br> 3. Consultar historico de ventas. |
| ***Poscondiciones :*** | <br>  |

<br>

| ***UC-09*** |  |
| --- | --- |
| ***Nombre:***  | Consultar historico de ventas |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> Cuando se acuerda un precio, opcionalmente se puede consultar un historico |
| ***Relaciones*** | UC-05, UC-06 |
| ***Actores:***  | <br>  Comprador, Vendedor. |
| ***Precondicion:*** | <br>  Un producto debe estar disponible |
| ***Flujo Normal:*** | <br>  1. El vendedor establece un precio inicial. <br> 2. El comprador acepta el precio. |
|***Flujo Alternativo:*** | <br> 2A. El comprador no acepta el precio y se debe establecer otro o finalizar compra. <br> 3. Consultar historico de ventas. |
| ***Poscondiciones :*** | <br>  |

<br>

| ***UC-10*** |  |
| --- | --- |
| ***Nombre:***  | Consultar precios |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> Se puede consultar el precio de un producto en venta |
| ***Relaciones*** | UC-04|
| ***Actores:***  | <br>  Abstracto. |
| ***Precondicion:*** | <br>  Un producto debe estar disponible |
| ***Flujo Normal:*** | <br>  1. Se debe buscar un producto. <br> 2. Se muestra en  pantalla el precio del producto. |
|***Flujo Alternativo:*** | <br> 2A. El producto no existe o no se encuentra disponible y se muestra el mensaje en pantalla. |
| ***Poscondiciones :*** | <br>  |

<br>

| ***UC-11*** |  |
| --- | --- |
| ***Nombre:***  | Consultar ofertas. |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> Se muestran las ofertas disponibles en el momento de la consulta. |
| ***Relaciones*** |  |
| ***Actores:***  | <br>  Abstracto. |
| ***Precondicion:*** | <br>   |
| ***Flujo Normal:*** | <br>  1. El actor pide información sobre ofertas actuales. <br> 2. El sistema agrupa información sobre las ofertas disponibles <br> 3. El sistema lista todas las ofertas en pantalla |
|***Flujo Alternativo:*** | <br> 3A. No existen ofertas disponibles y se muestra el mensaje en pantalla. |
| ***Poscondiciones :*** | <br>  |

<br>

| ***UC-12*** |  |
| --- | --- |
| ***Nombre:***  | Eliminar producto |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El administrador puede eliminar un producto existente del sistema. |
| ***Relaciones*** |  |
| ***Actores:***  | <br>  Administrador. |
| ***Precondicion:*** | <br>  El producto debe exitir en el sistema. |
| ***Flujo Normal:*** | <br>  1. El administrador escoge el producto a eliminar. <br> 2. El administrador pulsa sobre la opción "eliminar producto" <br> 3. El administrador confirma que quiere eliminar el producto. |
|***Flujo Alternativo:*** | <br> 3A. El administrador no confirma la eliminación y el producto no se elimina. |
| ***Poscondiciones :*** | <br> Se ha eliminado el producto. |

<br>

| ***UC-13*** |  |
| --- | --- |
| ***Nombre:***  | Avisar |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El proovedor puede realizar avisos con notificaciones. |
| ***Relaciones*** | UC-14, UC-15, UC-16, UC-17 |
| ***Actores:***  | <br>  Proveedor. |
| ***Precondicion:*** | <br>   |
| ***Flujo Normal:*** | <br>  1. El proveedor debe acceder a la seccion de notificaciones. <br> 2. El proveedor debe redactar el mensaje que quiere enviar. <br> 3. El proveedor debe pulsar "enviar notificacion" |
|***Flujo Alternativo:*** | <br>  |
| ***Poscondiciones :*** | <br>  |

<br>

| ***UC-14*** |  |
| --- | --- |
| ***Nombre:***  | Enviar notificacion |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El proveedor puede enviar una notificación. |
| ***Relaciones*** | UC-13 |
| ***Actores:***  | <br>  Proveedor. |
| ***Precondicion:*** | <br>   |
| ***Flujo Normal:*** | <br>  1. El provedor redacta un mensaje. <br> 2. El proveedor pulsa "enviar notificación" |
|***Flujo Alternativo:*** | <br> 3A. El administrador no confirma la eliminación y el producto no se elimina. |
| ***Poscondiciones :*** | <br>  |

<br>

| ***UC-15*** |  |
| --- | --- |
| ***Nombre:***  | Avisar fin de oferta |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El proveedor envía una notificación avisando del fin de una oferta. |
| ***Relaciones*** | UC-13, UC-16 |
| ***Actores:***  | <br>  Proveedor. |
| ***Precondicion:*** | <br>   |
| ***Flujo Normal:*** | <br> 1. El proveedor debe acceder a la seccion de notificaciones. <br> 2. El provedor redacta un mensaje. <br> 2. El proveedor pulsa "enviar notificación". <br> 3. El proveedor elimina la oferta. |
|***Flujo Alternativo:*** | <br>  |
| ***Poscondiciones :*** | <br>  |

<br>

| ***UC-16*** |  |
| --- | --- |
| ***Nombre:***  | Eliminar oferta |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El proveedor puede eliminar una oferta. |
| ***Relaciones*** | UC-13, UC-15 |
| ***Actores:***  | <br>  Proveedor. |
| ***Precondicion:*** | <br> El proovedor debe avisar del fin de oferta. |
| ***Flujo Normal:*** | <br>  1. El proveedor seleciona la oferta a eliminar. <br> 2. El proveedor pulsa la opcion "eliminar oferta". <br> 3. El proveedor confirma la eliminacion de la oferta |
|***Flujo Alternativo:*** | <br> 3A. El proveedor no confirma la eliminación y la oferta no se elimina. |
| ***Poscondiciones :*** | <br> La oferta se ha eliminado. |

<br>

| ***UC-17*** |  |
| --- | --- |
| ***Nombre:***  | Avisar nuevos productos |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El proveedor envía una notificacion informando de nuevos productos. |
| ***Relaciones*** | UC-13, UC-18 |
| ***Actores:***  | <br>  Proveedor. |
| ***Precondicion:*** | <br>   |
| ***Flujo Normal:*** | <br> 1. El proveedor debe acceder a la seccion de notificaciones. <br> 2. El provedor redacta un mensaje. <br> 2. El proveedor pulsa "enviar notificación" |
|***Flujo Alternativo:*** | <br> 3. Opcionalmente se puede realizar la incorporacion del producto |
| ***Poscondiciones :*** | <br>  |

<br>

| ***UC-18*** |  |
| --- | --- |
| ***Nombre:***  | Realizar incorporacion |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El proveedor incorpora un nuevo producto. |
| ***Relaciones*** | UC-13, UC-17 |
| ***Actores:***  | <br>  Proveedor. |
| ***Precondicion:*** | <br>  El proveedor avisa de la incorporacion del producto. |
| ***Flujo Normal:*** | <br> 1. El proveedor selecciona el producto que quiere añadir. <br> 2. El proveedor pulsa la opcion "incorporar producto". |
|***Flujo Alternativo:*** | <br> |
| ***Poscondiciones :*** | <br> La incorporacion se ha realizado y se ha guardado en el sistema. |

<br>

## Tablas de los requisitos de información de Sistema de compras.

| ***INF-01*** | Información sobre los usuarios del sistema.  |
| --- | --- |
| ***Version:***  | Septiembre-2022 |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Referencias:*** | <br> Vendedor, Proveedor, Comprador, Administrador. |
| ***Fuentes:***  | <br>   Sistema de Compras  |
| ***Descripción:*** | <br> El sistema deberá almacenar los datos sobre los diferentes roles <br> que ejerce el usuario del sistema. |
| ***Datos especificos:*** |   <br> 1. Nombre completo: Cadena de máximo 30 caracteres. <br> 2.Teléfono de contacto: Cadena de máximo 10 caracteres.  <br> 3. Email: Cadena <br> Numero de cuenta bancaria: Entero postivo. |
| ***Importancia:*** | <br> Muy importante. |
| ***Estado:*** | <br> Aceptado. |
| ***Comentarios:*** | <br> Los datos de los usuarios son imprescindibles en el correcto funcionamiento del sistema.|

 ***INF-02*** | Información sobre compras.  |
| --- | --- |
| ***Version:***  | Septiembre-2022 |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Referencias:*** | <br> Finalizar compra. |
| ***Fuentes:***  | <br>   Sistema de Compras  |
| ***Descripción:*** | <br> El sistema deberá almacenar la información correspondiente a las compras realizadas por los compradores. |
| ***Datos especificos:*** |   <br> 1. Número de referencia de la compra: Entero positivo de 5 dígitos. <br> 2.Fecha de realización de la compra: dd/mm/aaaa.  <br> 3. Destino del producto comprado: Cadena de un máximo de 30 caracteres. |
| ***Importancia:*** | <br> Muy importante. |
| ***Estado:*** | <br> Aceptado. |
| ***Comentarios:*** | <br> |

 ***INF-03*** | Información sobre las ofertas.  |
| --- | --- |
| ***Version:***  | Septiembre-2022 |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Referencias:*** | <br> Consultar ofertas. |
| ***Fuentes:***  | <br>   Sistema de Compras.  |
| ***Descripción:*** | <br> El sistema deberá almacenar la información correspondiente a las diferentes ofertas. |
| ***Datos especificos:*** |   <br> 1. Porcentaje de descuento: Cadena de 2 caracteres. Ejemplo: "%25". <br> 2. Identificador del producto ofertado: Entero positivo de 5 digitos. <br> 3. Fecha de finalización de la oferta: dd/mm/aaaa. |
| ***Importancia:*** | <br> Importante. |
| ***Estado:*** | <br> Aceptado. |
| ***Comentarios:*** | <br> Los productos ofertados deben estar presentes en el sistema junto a sus condiciones para que el comprador las pueda considerar. |
<br>

***INF-04*** | Información sobre productos.  |
| --- | --- |
| ***Version:***  | Septiembre-2022 |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Referencias:*** | <br> Buscar producto, Agregar producto. |
| ***Fuentes:***  | <br>   Sistema de Compras.  |
| ***Descripción:*** | <br> El sistema deberá almacenar la información correspondiente a los productos dsiponibles. |
| ***Datos especificos:*** |   <br> 1. Identificador del producto: entero de 3 dígitos. |
| ***Importancia:*** | <br> Muy importante. |
| ***Estado:*** | <br> Aceptado. |
| ***Comentarios:*** | <br> |

<br>

***INF-05*** | Información sobre precios.  |
| --- | --- |
| ***Version:***  | Septiembre-2022 |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Referencias:*** | <br> Consultar precios. |
| ***Fuentes:***  | <br>   Sistema de Compras.  |
| ***Descripción:*** | <br> El sistema deberá almacenar la información correspondiente a los precios. |
| ***Datos especificos:*** |   <br> 1. Identificador del producto: entero de 3 dígitos. <br> 2.Precio en euros del producto: Número real. |
| ***Importancia:*** | <br> Muy importante. |
| ***Estado:*** | <br> Aceptado. |
| ***Comentarios:*** | <br> |
<br>

***INF-06*** | Información sobre avisos.  |
| --- | --- |
| ***Version:***  | Septiembre-2022 |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Referencias:*** | <br> Avisar. |
| ***Fuentes:***  | <br>   Sistema de Compras.  |
| ***Descripción:*** | <br> El sistema deberá avisar a los usuarios de los productos que vayan saliendo a la venta. |
| ***Datos especificos:*** |   <br> 1. Notificación mostrando todos los nuevos productos: Cadena de máximo 20 caracteres por producto. <br> 2.Aviso de final de oferta: cadena |
| ***Importancia:*** | <br> Muy importante. |
| ***Estado:*** | <br> Aceptado. |
| ***Comentarios:*** | <br> |

 ***INF-07*** | Información sobre destinos.  |
| --- | --- |
| ***Version:***  | Septiembre-2022 |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Referencias:*** | <br> Finalizar compra. |
| ***Fuentes:***  | <br>   Sistema de Compras  |
| ***Descripción:*** | <br> El sistema deberá almacenar la información correspondiente al destino de cada una de las compras. |
| ***Datos especificos:*** |  <br> 1. Destino del producto comprado: Cadena de un máximo de 30 caracteres. |
| ***Importancia:*** | <br> Muy importante. |
| ***Estado:*** | <br> Aceptado. |
| ***Comentarios:*** | <br> |

***INF-08*** | Información sobre el histórico de ventas.  |
| --- | --- |
| ***Version:***  | Septiembre-2022 |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Referencias:*** | <br> Consultar histórico ventas. |
| ***Fuentes:***  | <br>   Sistema de Compras  |
| ***Descripción:*** | <br> El sistema deberá almacenar la información correspondiente al histórico de ventas. |
| ***Datos especificos:*** |  <br>  1.Nombre del usuario. <br> 2. Contraseña: cadena. |
| ***Importancia:*** | <br> Muy importante. |
| ***Estado:*** | <br> Aceptado. |
| ***Comentarios:*** | <br> |
