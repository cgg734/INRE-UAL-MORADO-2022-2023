# Horarios
En una universidad, el personal del PDI, el personal del PAS y los estudiantes pueden consultar horarios. Por su parte, el personal del PAS puede modificar horarios y dar de alta estudiantes. El personal de PDI puede proponer cambios en los horarios y dar de alta estudiantes. La funcionalidad de dar de alta estudiantes del PAS realiza una verificación de los datos del estudiante. Sin embargo, la funcionalidad de dar de alta estudiantes del PDI, además de verificar los datos también permite de forma excepcional realizar la búsqueda en las listas de clase de sus asignaturas.

| ***UC-01*** |  |
| --- | --- |
| ***Nombre:***  | Proponer cambios en el horario. |
| ***Autor:***  | Fehri Gil Fernandez Besada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El personal PDI puede proponer cambios en el horario. |
| ***Relaciones*** | IF |
| ***Actores:***  | <br>  PersonalPDI. |
| ***Precondicion:*** |  <br>  El personal PDI debe estar registrado. |
| ***Flujo Normal:***  | <br>  1. El personal PDI debe pulsar un boton para modificar el horario. <br> 2. El actor rellena un formulario con los cambios realizados. <br> 3. El actor pulsa un botón para confirmar los cambios. |
| ***Flujo Alternativo:*** | <br>  1. Si al confirmar no se actualiza el horario vuelve a mostrar el formulario. <br> 2. Si no se rellena el formulario se mostrará un mensaje de error. |
| ***Poscondiciones*** | <br>  La solicitud se ha realizado correctamente. |


| ***UC-02*** |  |
| --- | --- |
| ***Nombre:***  | Consultar horarios. |
| ***Autor:***  | Fehri Gil Fernandez Besada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El usuario puede comprobar el horario correspondiente |
| ***Relaciones*** | IF |
| ***Actores:***  | <br>  Estudiantes. |
| ***Precondicion:*** |  <br>  El estudiante debe de tener sus datos personales en la universidad y por tanto estar dado de alta. |
| ***Flujo Normal:***  | <br>  1. El estudiante accede a la pestaña de horario. <br> 2. El estudiante debe de elegir el dia y el mes. <br> 3. El actor pulsa un botón para el envio del formulario. <br> 4. El sistema comprueba que los datos introducidos. <br> 5. Visualizacion del horario. |
|***Flujo Alternativo:*** | <br> 4.A.- El sistema comprueba que los datos introducidos son correctos, en caso de que en el dia no haya ninguna clase se enviara un mensaje de error.<br>4.B.- El sistema comprueba que los datos introducidos son correctos, en caso de que los datos no lo sean, se avisara al usuario que los corrija.|
|***Postcondiciones*** | <br> El sistema ha comprobado que los datos introducidos son correctos y el horario se muestra satisfactoriamente |
<br>

| ***UC-03*** |  |
| --- | --- |
| ***Nombre:***  | Modificar horarios. |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El personal PAS puede modificar los horarios. |
| ***Actores:***  | <br>  PersonalPAS. |
| ***Precondicion:*** | <br>  El personal PAS debe estar registrado como PAS. |
| ***Relaciones*** | IF |
| ***Flujo Normal:*** | <br>  1. El personal PAS debe pulsar un boton para modificar el horario. <br> 2. El actor rellena un formulario con cajas de texto para los nuevos cambios realizados. <br> 3. El actor pulsa un botón para confirmar los cambios. |
|***Flujo Alternativo:*** | <br> 2A. El sistema comprueba los datos del formulario y si no son correctos pide corrección |
| ***Poscondiciones :*** | <br> Los cambios han sido almacenados en el sistema y se actualizan para el resto de usuarios |

| ***UC-04*** |  |
| --- | --- |
| ***Nombre:***  | Dar alta estudiantes (PDI) |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El personal PDI puede dar de alta a estudiantes. |
| ***Relaciones*** | UC-05,UC-06 |
| ***Actores:***  | <br>  PersonalPDI. |
| ***Precondicion:*** | <br>  El personal PDI debe estar registrado como PDI. |
| ***Flujo Normal:*** | <br>  1. El personal PDI debe pulsar un boton para elegir la opcion de dar alta a un estudiante. <br> 2. El actor rellena un formulario con cajas de texto para los datos del estudiante que se va a dar de alta. <br> 3. El actor pulsa un botón para confirmar los cambios. <br> 4. Los datos de los estudiantes deberan ser verificados por el sistema. |
|***Flujo Alternativo:*** | <br> 2A. Si en los datos existen correlacion con un alumno el personal puede buscar en las listas de clase. <br> 2B. El sistema comprueba los datos del formulario y si no son correctos pide corrección |
| ***Poscondiciones :*** | <br> Los cambios han sido almacenados en el sistema y se actualizan para el resto de usuarios |
<br>

| ***UC-05*** |  |
| --- | --- |
| ***Nombre:***  | Buscar en listas de clase. |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El personal PDI de manera opcional puede buscar en las listas de clase. |
| ***Relaciones*** | UC-04 |
| ***Actores:***  | <br>  PersonalPDI. |
| ***Precondicion:*** | <br>  El personal debe estar registrado como PDI |
| ***Flujo Normal:*** | <br>  1. El personal PDI debe dar de alta a un alumno. <br> 2. El personal PDI puede utilizar la opcion en las listas si existen correlaciones con los datos de los alumnos <br> 3. El actor pulsa un botón para confirmar los cambios. |
|***Flujo Alternativo:*** | <br> 2A. El sistema comprueba los datos del formulario y si no son correctos pide corrección |
| ***Poscondiciones :*** | <br> Los cambios han sido almacenados en el sistema y se actualizan para el resto de usuarios |
<br>

| ***UC-06*** |  |
| --- | --- |
| ***Nombre:***  | Dar alta estudiantes |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El personal PAS puede dar de alta a estudiantes. |
| ***Relaciones*** | UC-04 |
| ***Actores:***  | <br>  PersonalPAS. |
| ***Precondicion:*** | <br>  El personal PAS debe estar registrado como PAS. |
| ***Flujo Normal:*** | <br>  1. El personal PAS debe pulsar un boton para elegir la opcion de dar alta a un estudiante. <br> 2. El actor rellena un formulario con cajas de texto para los datos del estudiante que se va a dar de alta. <br> 3. El actor pulsa un botón para confirmar los cambios. <br> 4. Los datos de los estudiantes deberan ser verificados por el sistema. |
|***Flujo Alternativo:*** | <br> 4A. El sistema verifica los datos y comprueba que son erroneos por lo que se muestra un mensaje al personal PAS. |
| ***Poscondiciones :*** | <br> Los cambios han sido verificados, almacenados en el sistema y actualizados. |
<br>

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

# Sistema de compras
En un sistema de compra, existen cuatro tipos de usuarios: comprador, vendedor, proveedor y administrador. Los compradores pueden agregar productos, consultar precios, finalizar la compra y consultar ofertas. Agregar productos implica marcar esos productos como bloqueados. Los vendedores también pueden consultar ofertas y consultar precios. Los proveedores pueden consultar precios, avisar de nuevos productos y consultar ofertas. Avisar de nuevos productos, de forma excepcional, realiza la incorporación de una oferta. Los proveedores también tienen una funcionalidad para avisar del fin de una oferta. Cuando se avisa del fin de una oferta, se ejecuta la funcionalidad de eliminar la oferta. Ambas funcionalidades de avisar del proveedor tienen en común que se encarga de enviar una notificación. Los administradores pueden consultar precios, consultar ofertas y eliminar productos. La funcionalidad de consultar precios incluye una funcionalidad de buscar productos que es similar a la funcionalidad de consultar productos de los compradores. Sin embargo, la funcionalidad de consultar productos añade una funcionalidad para verificar la disponibilidad. Para realizar una venta, un comprador y un vendedor participan de forma conjunta. En dicha operación, se lleva a cabo el acuerdo de un precio; excepcionalmente, durante la realización de la venta, se consultará el histórico de ventas.

| ***UC-01*** |  |
| --- | --- |
| ***Nombre:***  | Finalizar compra |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El comprador puede finalizar una compra. |
| ***Relaciones*** | IF |
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
| ***Relaciones*** | If |
| ***Actores:***  | <br>  Comprador. |
| ***Precondicion:*** | <br>  Los productos deben mostrarse disponibles. |
| ***Flujo Normal:*** | <br>  1. El comprador puede seleccionar un producto clickando sobre el. <br> 2. El producto se agrega a la cesta de productos de la compra. <br> 3. El producto se bloquea. |
|***Flujo Alternativo:*** | <br> 2A. El producto no esta disponible e informa al comprador. |
| ***Poscondiciones :*** | <br> Los cambios han sido almacenados en el sistema y el producto bloqueado para el comprador. |
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
| ***Descripcion:*** | <br> El personal PAS puede modificar los horarios. |
| ***Actores:***  | <br>  Comprador, Abstracto. |
| ***Precondicion:*** | <br>  El producto debe existir en el sistema. |
| ***Flujo Normal:*** | <br>  1. Los actores deben introducir la id o palabra clave en el motor de busqueda. <br> 2. El sistema muestra informacin relacionada con los datos introducidos en el buscador. |
|***Flujo Alternativo:*** | <br> 2A. El sistema no encuentra correlaciones con los datos introducidos e informa al usuario |
| ***Poscondiciones :*** | <br> El sistema ha mostrado un mensaje al usuario. |
<br>

| ***UC-05*** | |
|--- | --- |
| ***Nombre*** | Realizar venta |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El comprador y el vendedor pueden realizar una venta simultaneamente. |
| ***Relaciones*** | UC-08  |
| ***Actores:***  | <br>  Comprador, Vendedor. |
| ***Precondicion:*** | <br>  El comprador y el vendedor necesitan realizar esta funcion simultaneamente. |
| ***Flujo Normal:*** | <br>  1. Los actores deben introducir la id o palabra clave en el motor de busqueda. <br> 2. El sistema muestra informacin relacionada con los datos introducidos en el buscador.<br> 3. Ambos actores deben acordar un precio. <br> 4. Se realiza la compra y se registra en el sistema <br> |
|***Flujo Alternativo:*** | <br> 2A. El sistema no encuentra correlaciones con los datos introducidos e informa al usuario |
| ***Poscondiciones :*** | <br> El sistema ha mostrado un mensaje al usuario. |

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
| ***Poscondiciones :*** | <br> Los cambios han sido almacenados en el sistema y el producto bloqueado para el comprador. |

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
| ***Poscondiciones :*** | <br> Los cambios han sido almacenados en el sistema y el producto bloqueado para el comprador. |

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
| ***Poscondiciones :*** | <br> Los cambios han sido almacenados en el sistema y el producto bloqueado para el comprador. |

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
| ***Poscondiciones :*** | <br> Los cambios han sido almacenados en el sistema y el producto 
ha sido eliminado. |

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
| ***Poscondiciones :*** | <br> Los cambios han sido almacenados en el sistema y el producto 
ha sido eliminado. |

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
| ***Poscondiciones :*** | <br> Los cambios han sido almacenados en el sistema y la oferta ha sido eliminada. |

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
<<<<<<< HEAD
<<<<<<< HEAD
<<<<<<< HEAD
=======

>>>>>>> 13c210f7b6cf0e62a52afb25b7568846093c9de9
=======
>>>>>>> 96f9d75adb75a664bd8d822dd86ecbd1443f0871
=======
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

***INF-04*** | Información sobre avisos.  |
| --- | --- |
| ***Version:***  | Septiembre-2022 |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Referencias:*** | <br> Avisar. |
| ***Fuentes:***  | <br>   Sistema de Compras.  |
| ***Descripción:*** | <br> El sistema deberá avisar a los usuarios de los productos que vayan saliendo a la venta. |
| ***Datos especificos:*** |   <br> 1. Notificación mostrando todos los nuevos productos: Cadena de máximo 20 caracteres por producto. |
| ***Importancia:*** | <br> Muy importante. |
| ***Estado:*** | <br> Aceptado. |
| ***Comentarios:*** | <br> |
>>>>>>> 76503cea91e6489dbb7947f5feb999c38120477b


## Entidad relación horarios
<?xml version="1.0" encoding="UTF-8" standalone="no"?><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" contentStyleType="text/css" height="581px" preserveAspectRatio="none" style="width:429px;height:581px;background:#FFFFFF;" version="1.1" viewBox="0 0 429 581" width="429px" zoomAndPan="magnify"><defs/><g><!--MD5=[9196e7f5424c8ba52e10312e1fe81956]
class Estudiante--><g id="elem_Estudiante"><rect codeLine="1" fill="#F1F1F1" height="118.4375" id="Estudiante" rx="2.5" ry="2.5" style="stroke:#181818;stroke-width:0.5;" width="121" x="260.5" y="456"/><ellipse cx="285.4" cy="472" fill="#ADD1B2" rx="11" ry="11" style="stroke:#181818;stroke-width:1.0;"/><path d="M288.1656,467.875 Q288.3219,467.6563 288.5094,467.5469 Q288.6969,467.4375 288.9156,467.4375 Q289.2906,467.4375 289.525,467.7031 Q289.7594,467.9531 289.7594,468.5625 L289.7594,470.0156 Q289.7594,470.625 289.525,470.8906 Q289.2906,471.1563 288.9156,471.1563 Q288.5719,471.1563 288.3688,470.9531 Q288.1656,470.7656 288.0563,470.25 Q288.0094,469.8906 287.8219,469.7031 Q287.4938,469.3281 286.8844,469.1094 Q286.275,468.8906 285.65,468.8906 Q284.8844,468.8906 284.2438,469.2188 Q283.6188,469.5469 283.1188,470.2969 Q282.6344,471.0469 282.6344,472.0781 L282.6344,473.1719 Q282.6344,474.4063 283.525,475.2344 Q284.4156,476.0469 286.0094,476.0469 Q286.9469,476.0469 287.6031,475.7969 Q287.9938,475.6406 288.4156,475.2031 Q288.6813,474.9375 288.8219,474.8594 Q288.9781,474.7813 289.1813,474.7813 Q289.5094,474.7813 289.7594,475.0469 Q290.025,475.2969 290.025,475.6406 Q290.025,475.9844 289.6813,476.3906 Q289.1813,476.9688 288.3844,477.2969 Q287.3063,477.75 286.0094,477.75 Q284.4938,477.75 283.2906,477.125 Q282.3063,476.625 281.6188,475.5625 Q280.9313,474.4844 280.9313,473.2031 L280.9313,472.0469 Q280.9313,470.7188 281.5406,469.5781 Q282.1656,468.4219 283.2594,467.8125 Q284.3531,467.1875 285.5875,467.1875 Q286.3219,467.1875 286.9625,467.3594 Q287.6188,467.5156 288.1656,467.875 Z " fill="#000000"/><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="67" x="301.6" y="477.7285">Estudiante</text><line style="stroke:#181818;stroke-width:0.5;" x1="261.5" x2="380.5" y1="488" y2="488"/><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="47" x="266.5" y="506.5332">DNI/NIE</text><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="109" x="266.5" y="524.1426">NombreCompleto</text><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="56" x="266.5" y="541.752">Telefono</text><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="31" x="266.5" y="559.3613">Sexo</text><line style="stroke:#181818;stroke-width:0.5;" x1="261.5" x2="380.5" y1="566.4375" y2="566.4375"/></g><!--MD5=[b4ad1b83a0bbbe5b274e4fd9e75e34c1]
class Horarios--><g id="elem_Horarios"><rect codeLine="7" fill="#F1F1F1" height="100.8281" id="Horarios" rx="2.5" ry="2.5" style="stroke:#181818;stroke-width:0.5;" width="129" x="256.5" y="277"/><ellipse cx="291.3" cy="293" fill="#ADD1B2" rx="11" ry="11" style="stroke:#181818;stroke-width:1.0;"/><path d="M294.0656,288.875 Q294.2219,288.6563 294.4094,288.5469 Q294.5969,288.4375 294.8156,288.4375 Q295.1906,288.4375 295.425,288.7031 Q295.6594,288.9531 295.6594,289.5625 L295.6594,291.0156 Q295.6594,291.625 295.425,291.8906 Q295.1906,292.1563 294.8156,292.1563 Q294.4719,292.1563 294.2688,291.9531 Q294.0656,291.7656 293.9563,291.25 Q293.9094,290.8906 293.7219,290.7031 Q293.3938,290.3281 292.7844,290.1094 Q292.175,289.8906 291.55,289.8906 Q290.7844,289.8906 290.1438,290.2188 Q289.5188,290.5469 289.0188,291.2969 Q288.5344,292.0469 288.5344,293.0781 L288.5344,294.1719 Q288.5344,295.4063 289.425,296.2344 Q290.3156,297.0469 291.9094,297.0469 Q292.8469,297.0469 293.5031,296.7969 Q293.8938,296.6406 294.3156,296.2031 Q294.5813,295.9375 294.7219,295.8594 Q294.8781,295.7813 295.0813,295.7813 Q295.4094,295.7813 295.6594,296.0469 Q295.925,296.2969 295.925,296.6406 Q295.925,296.9844 295.5813,297.3906 Q295.0813,297.9688 294.2844,298.2969 Q293.2063,298.75 291.9094,298.75 Q290.3938,298.75 289.1906,298.125 Q288.2063,297.625 287.5188,296.5625 Q286.8313,295.4844 286.8313,294.2031 L286.8313,293.0469 Q286.8313,291.7188 287.4406,290.5781 Q288.0656,289.4219 289.1594,288.8125 Q290.2531,288.1875 291.4875,288.1875 Q292.2219,288.1875 292.8625,288.3594 Q293.5188,288.5156 294.0656,288.875 Z " fill="#000000"/><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="53" x="309.7" y="298.7285">Horarios</text><line style="stroke:#181818;stroke-width:0.5;" x1="257.5" x2="384.5" y1="309" y2="309"/><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="117" x="262.5" y="327.5332">NombreAsignatura</text><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="105" x="262.5" y="345.1426">HorasAsignatura</text><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="89" x="262.5" y="362.752">DiaAsignatura</text><line style="stroke:#181818;stroke-width:0.5;" x1="257.5" x2="384.5" y1="369.8281" y2="369.8281"/></g><!--MD5=[82bd83a36b8e65dbb86a63e1a11596d9]
class DarAltaEstudiante--><g id="elem_DarAltaEstudiante"><rect codeLine="13" fill="#F1F1F1" height="83.2188" id="DarAltaEstudiante" rx="2.5" ry="2.5" style="stroke:#181818;stroke-width:0.5;" width="148" x="82" y="7"/><ellipse cx="97.9" cy="23" fill="#ADD1B2" rx="11" ry="11" style="stroke:#181818;stroke-width:1.0;"/><path d="M100.6656,18.875 Q100.8219,18.6563 101.0094,18.5469 Q101.1969,18.4375 101.4156,18.4375 Q101.7906,18.4375 102.025,18.7031 Q102.2594,18.9531 102.2594,19.5625 L102.2594,21.0156 Q102.2594,21.625 102.025,21.8906 Q101.7906,22.1563 101.4156,22.1563 Q101.0719,22.1563 100.8688,21.9531 Q100.6656,21.7656 100.5563,21.25 Q100.5094,20.8906 100.3219,20.7031 Q99.9938,20.3281 99.3844,20.1094 Q98.775,19.8906 98.15,19.8906 Q97.3844,19.8906 96.7438,20.2188 Q96.1188,20.5469 95.6188,21.2969 Q95.1344,22.0469 95.1344,23.0781 L95.1344,24.1719 Q95.1344,25.4063 96.025,26.2344 Q96.9156,27.0469 98.5094,27.0469 Q99.4469,27.0469 100.1031,26.7969 Q100.4938,26.6406 100.9156,26.2031 Q101.1813,25.9375 101.3219,25.8594 Q101.4781,25.7813 101.6813,25.7813 Q102.0094,25.7813 102.2594,26.0469 Q102.525,26.2969 102.525,26.6406 Q102.525,26.9844 102.1813,27.3906 Q101.6813,27.9688 100.8844,28.2969 Q99.8063,28.75 98.5094,28.75 Q96.9938,28.75 95.7906,28.125 Q94.8063,27.625 94.1188,26.5625 Q93.4313,25.4844 93.4313,24.2031 L93.4313,23.0469 Q93.4313,21.7188 94.0406,20.5781 Q94.6656,19.4219 95.7594,18.8125 Q96.8531,18.1875 98.0875,18.1875 Q98.8219,18.1875 99.4625,18.3594 Q100.1188,18.5156 100.6656,18.875 Z " fill="#000000"/><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="114" x="112.1" y="28.7285">DarAltaEstudiante</text><line style="stroke:#181818;stroke-width:0.5;" x1="83" x2="229" y1="39" y2="39"/><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="116" x="88" y="57.5332">NombreEstudiante</text><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="136" x="88" y="75.1426">AsignaturasCursadas</text><line style="stroke:#181818;stroke-width:0.5;" x1="83" x2="229" y1="82.2188" y2="82.2188"/></g><!--MD5=[c9adfff1edbca196486ac5da9e1683ec]
class PersonalPDI--><g id="elem_PersonalPDI"><rect fill="#F1F1F1" height="48" id="PersonalPDI" rx="2.5" ry="2.5" style="stroke:#181818;stroke-width:0.5;" width="110" x="7" y="303.5"/><ellipse cx="22" cy="319.5" fill="#ADD1B2" rx="11" ry="11" style="stroke:#181818;stroke-width:1.0;"/><path d="M24.7656,315.375 Q24.9219,315.1563 25.1094,315.0469 Q25.2969,314.9375 25.5156,314.9375 Q25.8906,314.9375 26.125,315.2031 Q26.3594,315.4531 26.3594,316.0625 L26.3594,317.5156 Q26.3594,318.125 26.125,318.3906 Q25.8906,318.6563 25.5156,318.6563 Q25.1719,318.6563 24.9688,318.4531 Q24.7656,318.2656 24.6563,317.75 Q24.6094,317.3906 24.4219,317.2031 Q24.0938,316.8281 23.4844,316.6094 Q22.875,316.3906 22.25,316.3906 Q21.4844,316.3906 20.8438,316.7188 Q20.2188,317.0469 19.7188,317.7969 Q19.2344,318.5469 19.2344,319.5781 L19.2344,320.6719 Q19.2344,321.9063 20.125,322.7344 Q21.0156,323.5469 22.6094,323.5469 Q23.5469,323.5469 24.2031,323.2969 Q24.5938,323.1406 25.0156,322.7031 Q25.2813,322.4375 25.4219,322.3594 Q25.5781,322.2813 25.7813,322.2813 Q26.1094,322.2813 26.3594,322.5469 Q26.625,322.7969 26.625,323.1406 Q26.625,323.4844 26.2813,323.8906 Q25.7813,324.4688 24.9844,324.7969 Q23.9063,325.25 22.6094,325.25 Q21.0938,325.25 19.8906,324.625 Q18.9063,324.125 18.2188,323.0625 Q17.5313,321.9844 17.5313,320.7031 L17.5313,319.5469 Q17.5313,318.2188 18.1406,317.0781 Q18.7656,315.9219 19.8594,315.3125 Q20.9531,314.6875 22.1875,314.6875 Q22.9219,314.6875 23.5625,314.8594 Q24.2188,315.0156 24.7656,315.375 Z " fill="#000000"/><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="78" x="36" y="325.2285">PersonalPDI</text><line style="stroke:#181818;stroke-width:0.5;" x1="8" x2="116" y1="335.5" y2="335.5"/><line style="stroke:#181818;stroke-width:0.5;" x1="8" x2="116" y1="343.5" y2="343.5"/></g><!--MD5=[02db5d10e61597e32ed558157bf408c4]
class PersonalPAS--><g id="elem_PersonalPAS"><rect fill="#F1F1F1" height="48" id="PersonalPAS" rx="2.5" ry="2.5" style="stroke:#181818;stroke-width:0.5;" width="115" x="263.5" y="151"/><ellipse cx="278.5" cy="167" fill="#ADD1B2" rx="11" ry="11" style="stroke:#181818;stroke-width:1.0;"/><path d="M281.2656,162.875 Q281.4219,162.6563 281.6094,162.5469 Q281.7969,162.4375 282.0156,162.4375 Q282.3906,162.4375 282.625,162.7031 Q282.8594,162.9531 282.8594,163.5625 L282.8594,165.0156 Q282.8594,165.625 282.625,165.8906 Q282.3906,166.1563 282.0156,166.1563 Q281.6719,166.1563 281.4688,165.9531 Q281.2656,165.7656 281.1563,165.25 Q281.1094,164.8906 280.9219,164.7031 Q280.5938,164.3281 279.9844,164.1094 Q279.375,163.8906 278.75,163.8906 Q277.9844,163.8906 277.3438,164.2188 Q276.7188,164.5469 276.2188,165.2969 Q275.7344,166.0469 275.7344,167.0781 L275.7344,168.1719 Q275.7344,169.4063 276.625,170.2344 Q277.5156,171.0469 279.1094,171.0469 Q280.0469,171.0469 280.7031,170.7969 Q281.0938,170.6406 281.5156,170.2031 Q281.7813,169.9375 281.9219,169.8594 Q282.0781,169.7813 282.2813,169.7813 Q282.6094,169.7813 282.8594,170.0469 Q283.125,170.2969 283.125,170.6406 Q283.125,170.9844 282.7813,171.3906 Q282.2813,171.9688 281.4844,172.2969 Q280.4063,172.75 279.1094,172.75 Q277.5938,172.75 276.3906,172.125 Q275.4063,171.625 274.7188,170.5625 Q274.0313,169.4844 274.0313,168.2031 L274.0313,167.0469 Q274.0313,165.7188 274.6406,164.5781 Q275.2656,163.4219 276.3594,162.8125 Q277.4531,162.1875 278.6875,162.1875 Q279.4219,162.1875 280.0625,162.3594 Q280.7188,162.5156 281.2656,162.875 Z " fill="#000000"/><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="83" x="292.5" y="172.7285">PersonalPAS</text><line style="stroke:#181818;stroke-width:0.5;" x1="264.5" x2="377.5" y1="183" y2="183"/><line style="stroke:#181818;stroke-width:0.5;" x1="264.5" x2="377.5" y1="191" y2="191"/></g><!--MD5=[2b05f4afa5075432514dba4c80908943]
link PersonalPDI to Estudiante--><g id="link_PersonalPDI_Estudiante"><path codeLine="18" d="M94.28,351.62 C131.5,378.28 193.97,423.02 243.92,458.79 " fill="none" id="PersonalPDI-to-Estudiante" style="stroke:#181818;stroke-width:1.0;"/><polygon fill="none" points="248.14,453.21,260.33,470.54,239.99,464.59,248.14,453.21" style="stroke:#181818;stroke-width:1.0;"/></g><!--MD5=[dcd5e2ca0a01ef1d88397ca0337e95d3]
reverse link Estudiante to PersonalPAS--><g id="link_Estudiante_PersonalPAS"><path codeLine="19" d="M378.93,438.88 C389.77,420.04 398.97,399.15 403,378 C415.52,312.37 422.32,283.02 383,229 C374.92,217.89 364.06,207.6 353.69,199.09 " fill="none" id="Estudiante-backto-PersonalPAS" style="stroke:#181818;stroke-width:1.0;"/><polygon fill="none" points="384.87,442.58,368.38,455.89,372.97,435.2,384.87,442.58" style="stroke:#181818;stroke-width:1.0;"/></g><!--MD5=[d818663ee5c8b736f48fac9242219d65]
reverse link Horarios to Estudiante--><g id="link_Horarios_Estudiante"><path codeLine="20" d="M321,383.33 C321,406.18 321,432.74 321,455.92 " fill="none" id="Horarios-backto-Estudiante" style="stroke:#181818;stroke-width:1.0;"/><polygon fill="#181818" points="321,378.21,317,387.21,321,383.21,325,387.21,321,378.21" style="stroke:#181818;stroke-width:1.0;"/><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="53" x="322" y="422.4951">consultar</text><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="20" x="299.7188" y="399.2609">1..*</text><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="7" x="313.5734" y="445.2345">1</text></g><!--MD5=[5631b959925e3f2a071d411cae8f52fa]
link PersonalPDI to Horarios--><g id="link_PersonalPDI_Horarios"><path codeLine="21" d="M117.24,327.5 C156.36,327.5 209.13,327.5 251.17,327.5 " fill="none" id="PersonalPDI-to-Horarios" style="stroke:#181818;stroke-width:1.0;"/><polygon fill="#181818" points="256.24,327.5,247.24,323.5,251.24,327.5,247.24,331.5,256.24,327.5" style="stroke:#181818;stroke-width:1.0;"/><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="103" x="135.25" y="320.9951">ProponerCambios</text><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="7" x="125.1332" y="323.9437">1</text><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="20" x="228.5304" y="341.8471">1..*</text></g><!--MD5=[618b6bef81b01a4d85e317bd74772759]
link PersonalPAS to Horarios--><g id="link_PersonalPAS_Horarios"><path codeLine="22" d="M321,199.19 C321,218.43 321,246.59 321,271.53 " fill="none" id="PersonalPAS-to-Horarios" style="stroke:#181818;stroke-width:1.0;"/><polygon fill="#181818" points="321,276.8,325,267.8,321,271.8,317,267.8,321,276.8" style="stroke:#181818;stroke-width:1.0;"/><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="52" x="322" y="243.4951">Modificar</text><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="7" x="313.1469" y="220.5743">1</text><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="20" x="299.5938" y="266.0772">1..*</text></g><!--MD5=[2589d99f278b8c304e749e715a1d1e33]
reverse link DarAltaEstudiante to PersonalPAS--><g id="link_DarAltaEstudiante_PersonalPAS"><path codeLine="23" d="M214.13,93.36 C239.87,112.78 269.09,134.83 290.46,150.96 " fill="none" id="DarAltaEstudiante-backto-PersonalPAS" style="stroke:#181818;stroke-width:1.0;"/><polygon fill="#181818" points="210.03,90.27,214.7955,98.8891,214.018,93.286,219.6211,92.5084,210.03,90.27" style="stroke:#181818;stroke-width:1.0;"/><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="20" x="197.0473" y="111.7078">1..*</text><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="7" x="274.7372" y="140.2899">1</text></g><!--MD5=[e05c88df44ec4377e76fb222e8b51910]
reverse link DarAltaEstudiante to PersonalPDI--><g id="link_DarAltaEstudiante_PersonalPDI"><path codeLine="24" d="M140.56,95.01 C120.27,154.8 85.39,257.56 69.86,303.33 " fill="none" id="DarAltaEstudiante-backto-PersonalPDI" style="stroke:#181818;stroke-width:1.0;"/><polygon fill="#181818" points="142.23,90.07,135.5564,97.3131,140.6274,94.8062,143.1343,99.8773,142.23,90.07" style="stroke:#181818;stroke-width:1.0;"/><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="20" x="118.2931" y="111.7861">1..*</text><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="7" x="63.9773" y="292.6266">1</text></g><!--MD5=[6e207c45a3b2b8c8ee502f7eb9581c78]


## Entidad relación sistema de compras
<?xml version="1.0" encoding="UTF-8" standalone="no"?><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" contentStyleType="text/css" height="526px" preserveAspectRatio="none" style="width:776px;height:526px;background:#FFFFFF;" version="1.1" viewBox="0 0 776 526" width="776px" zoomAndPan="magnify"><defs/><g><!--MD5=[b3fed880fe33e1395404e2a133ef8753]
class Proovedor--><g id="elem_Proovedor"><rect codeLine="2" fill="#F1F1F1" height="83.2188" id="Proovedor" rx="2.5" ry="2.5" style="stroke:#181818;stroke-width:0.5;" width="176" x="7" y="58.76"/><ellipse cx="57.75" cy="74.76" fill="#ADD1B2" rx="11" ry="11" style="stroke:#181818;stroke-width:1.0;"/><path d="M60.5156,70.635 Q60.6719,70.4162 60.8594,70.3069 Q61.0469,70.1975 61.2656,70.1975 Q61.6406,70.1975 61.875,70.4631 Q62.1094,70.7131 62.1094,71.3225 L62.1094,72.7756 Q62.1094,73.385 61.875,73.6506 Q61.6406,73.9162 61.2656,73.9162 Q60.9219,73.9162 60.7188,73.7131 Q60.5156,73.5256 60.4063,73.01 Q60.3594,72.6506 60.1719,72.4631 Q59.8438,72.0881 59.2344,71.8694 Q58.625,71.6506 58,71.6506 Q57.2344,71.6506 56.5938,71.9787 Q55.9688,72.3069 55.4688,73.0569 Q54.9844,73.8069 54.9844,74.8381 L54.9844,75.9319 Q54.9844,77.1662 55.875,77.9944 Q56.7656,78.8069 58.3594,78.8069 Q59.2969,78.8069 59.9531,78.5569 Q60.3438,78.4006 60.7656,77.9631 Q61.0313,77.6975 61.1719,77.6194 Q61.3281,77.5412 61.5313,77.5412 Q61.8594,77.5412 62.1094,77.8069 Q62.375,78.0569 62.375,78.4006 Q62.375,78.7444 62.0313,79.1506 Q61.5313,79.7287 60.7344,80.0569 Q59.6563,80.51 58.3594,80.51 Q56.8438,80.51 55.6406,79.885 Q54.6563,79.385 53.9688,78.3225 Q53.2813,77.2444 53.2813,75.9631 L53.2813,74.8069 Q53.2813,73.4787 53.8906,72.3381 Q54.5156,71.1819 55.6094,70.5725 Q56.7031,69.9475 57.9375,69.9475 Q58.6719,69.9475 59.3125,70.1194 Q59.9688,70.2756 60.5156,70.635 Z " fill="#000000"/><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="66" x="78.25" y="80.4885">Proovedor</text><line style="stroke:#181818;stroke-width:0.5;" x1="8" x2="182" y1="90.76" y2="90.76"/><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="156" x="13" y="109.2932">Avisar nuevos productos</text><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="164" x="13" y="126.9026">Avisar fin -&gt; elimina oferta</text><line style="stroke:#181818;stroke-width:0.5;" x1="8" x2="182" y1="133.9788" y2="133.9788"/></g><!--MD5=[9231e5b138909734b576f3545e846cfa]
class Productos--><g id="elem_Productos"><rect codeLine="8" fill="#F1F1F1" height="65.6094" id="Productos" rx="2.5" ry="2.5" style="stroke:#181818;stroke-width:0.5;" width="96" x="218" y="67.26"/><ellipse cx="233" cy="83.26" fill="#ADD1B2" rx="11" ry="11" style="stroke:#181818;stroke-width:1.0;"/><path d="M235.7656,79.135 Q235.9219,78.9162 236.1094,78.8069 Q236.2969,78.6975 236.5156,78.6975 Q236.8906,78.6975 237.125,78.9631 Q237.3594,79.2131 237.3594,79.8225 L237.3594,81.2756 Q237.3594,81.885 237.125,82.1506 Q236.8906,82.4162 236.5156,82.4162 Q236.1719,82.4162 235.9688,82.2131 Q235.7656,82.0256 235.6563,81.51 Q235.6094,81.1506 235.4219,80.9631 Q235.0938,80.5881 234.4844,80.3694 Q233.875,80.1506 233.25,80.1506 Q232.4844,80.1506 231.8438,80.4787 Q231.2188,80.8069 230.7188,81.5569 Q230.2344,82.3069 230.2344,83.3381 L230.2344,84.4319 Q230.2344,85.6662 231.125,86.4944 Q232.0156,87.3069 233.6094,87.3069 Q234.5469,87.3069 235.2031,87.0569 Q235.5938,86.9006 236.0156,86.4631 Q236.2813,86.1975 236.4219,86.1194 Q236.5781,86.0412 236.7813,86.0412 Q237.1094,86.0412 237.3594,86.3069 Q237.625,86.5569 237.625,86.9006 Q237.625,87.2444 237.2813,87.6506 Q236.7813,88.2287 235.9844,88.5569 Q234.9063,89.01 233.6094,89.01 Q232.0938,89.01 230.8906,88.385 Q229.9063,87.885 229.2188,86.8225 Q228.5313,85.7444 228.5313,84.4631 L228.5313,83.3069 Q228.5313,81.9787 229.1406,80.8381 Q229.7656,79.6819 230.8594,79.0725 Q231.9531,78.4475 233.1875,78.4475 Q233.9219,78.4475 234.5625,78.6194 Q235.2188,78.7756 235.7656,79.135 Z " fill="#000000"/><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="64" x="247" y="88.9885">Productos</text><line style="stroke:#181818;stroke-width:0.5;" x1="219" x2="313" y1="99.26" y2="99.26"/><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="44" x="224" y="117.7932">Estado</text><line style="stroke:#181818;stroke-width:0.5;" x1="219" x2="313" y1="124.8694" y2="124.8694"/></g><!--MD5=[4668456ee0d5bf931cf805ae22408c96]
class Oferta--><g id="elem_Oferta"><rect codeLine="11" fill="#F1F1F1" height="48" id="Oferta" rx="2.5" ry="2.5" style="stroke:#181818;stroke-width:0.5;" width="72" x="542" y="76.26"/><ellipse cx="557" cy="92.26" fill="#ADD1B2" rx="11" ry="11" style="stroke:#181818;stroke-width:1.0;"/><path d="M559.7656,88.135 Q559.9219,87.9162 560.1094,87.8069 Q560.2969,87.6975 560.5156,87.6975 Q560.8906,87.6975 561.125,87.9631 Q561.3594,88.2131 561.3594,88.8225 L561.3594,90.2756 Q561.3594,90.885 561.125,91.1506 Q560.8906,91.4162 560.5156,91.4162 Q560.1719,91.4162 559.9688,91.2131 Q559.7656,91.0256 559.6563,90.51 Q559.6094,90.1506 559.4219,89.9631 Q559.0938,89.5881 558.4844,89.3694 Q557.875,89.1506 557.25,89.1506 Q556.4844,89.1506 555.8438,89.4787 Q555.2188,89.8069 554.7188,90.5569 Q554.2344,91.3069 554.2344,92.3381 L554.2344,93.4319 Q554.2344,94.6662 555.125,95.4944 Q556.0156,96.3069 557.6094,96.3069 Q558.5469,96.3069 559.2031,96.0569 Q559.5938,95.9006 560.0156,95.4631 Q560.2813,95.1975 560.4219,95.1194 Q560.5781,95.0412 560.7813,95.0412 Q561.1094,95.0412 561.3594,95.3069 Q561.625,95.5569 561.625,95.9006 Q561.625,96.2444 561.2813,96.6506 Q560.7813,97.2287 559.9844,97.5569 Q558.9063,98.01 557.6094,98.01 Q556.0938,98.01 554.8906,97.385 Q553.9063,96.885 553.2188,95.8225 Q552.5313,94.7444 552.5313,93.4631 L552.5313,92.3069 Q552.5313,90.9787 553.1406,89.8381 Q553.7656,88.6819 554.8594,88.0725 Q555.9531,87.4475 557.1875,87.4475 Q557.9219,87.4475 558.5625,87.6194 Q559.2188,87.7756 559.7656,88.135 Z " fill="#000000"/><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="40" x="571" y="97.9885">Oferta</text><line style="stroke:#181818;stroke-width:0.5;" x1="543" x2="613" y1="108.26" y2="108.26"/><line style="stroke:#181818;stroke-width:0.5;" x1="543" x2="613" y1="116.26" y2="116.26"/></g><!--MD5=[15e9b30b2ef5e94ac5c226f45dfb44fa]
class RealizarVenta--><g id="elem_RealizarVenta"><rect codeLine="14" fill="#F1F1F1" height="48" id="RealizarVenta" rx="2.5" ry="2.5" style="stroke:#181818;stroke-width:0.5;" width="120" x="649" y="76.26"/><ellipse cx="664" cy="92.26" fill="#ADD1B2" rx="11" ry="11" style="stroke:#181818;stroke-width:1.0;"/><path d="M666.7656,88.135 Q666.9219,87.9162 667.1094,87.8069 Q667.2969,87.6975 667.5156,87.6975 Q667.8906,87.6975 668.125,87.9631 Q668.3594,88.2131 668.3594,88.8225 L668.3594,90.2756 Q668.3594,90.885 668.125,91.1506 Q667.8906,91.4162 667.5156,91.4162 Q667.1719,91.4162 666.9688,91.2131 Q666.7656,91.0256 666.6563,90.51 Q666.6094,90.1506 666.4219,89.9631 Q666.0938,89.5881 665.4844,89.3694 Q664.875,89.1506 664.25,89.1506 Q663.4844,89.1506 662.8438,89.4787 Q662.2188,89.8069 661.7188,90.5569 Q661.2344,91.3069 661.2344,92.3381 L661.2344,93.4319 Q661.2344,94.6662 662.125,95.4944 Q663.0156,96.3069 664.6094,96.3069 Q665.5469,96.3069 666.2031,96.0569 Q666.5938,95.9006 667.0156,95.4631 Q667.2813,95.1975 667.4219,95.1194 Q667.5781,95.0412 667.7813,95.0412 Q668.1094,95.0412 668.3594,95.3069 Q668.625,95.5569 668.625,95.9006 Q668.625,96.2444 668.2813,96.6506 Q667.7813,97.2287 666.9844,97.5569 Q665.9063,98.01 664.6094,98.01 Q663.0938,98.01 661.8906,97.385 Q660.9063,96.885 660.2188,95.8225 Q659.5313,94.7444 659.5313,93.4631 L659.5313,92.3069 Q659.5313,90.9787 660.1406,89.8381 Q660.7656,88.6819 661.8594,88.0725 Q662.9531,87.4475 664.1875,87.4475 Q664.9219,87.4475 665.5625,87.6194 Q666.2188,87.7756 666.7656,88.135 Z " fill="#000000"/><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="88" x="678" y="97.9885">RealizarVenta</text><line style="stroke:#181818;stroke-width:0.5;" x1="650" x2="768" y1="108.26" y2="108.26"/><line style="stroke:#181818;stroke-width:0.5;" x1="650" x2="768" y1="116.26" y2="116.26"/></g><!--MD5=[e0abbd9070b521e31286504acc171f60]
class ConsultarHistoricoVenta--><g id="elem_ConsultarHistoricoVenta"><rect codeLine="17" fill="#F1F1F1" height="48" id="ConsultarHistoricoVenta" rx="2.5" ry="2.5" style="stroke:#181818;stroke-width:0.5;" width="184" x="486" y="219.76"/><ellipse cx="501" cy="235.76" fill="#ADD1B2" rx="11" ry="11" style="stroke:#181818;stroke-width:1.0;"/><path d="M503.7656,231.635 Q503.9219,231.4163 504.1094,231.3069 Q504.2969,231.1975 504.5156,231.1975 Q504.8906,231.1975 505.125,231.4631 Q505.3594,231.7131 505.3594,232.3225 L505.3594,233.7756 Q505.3594,234.385 505.125,234.6506 Q504.8906,234.9163 504.5156,234.9163 Q504.1719,234.9163 503.9688,234.7131 Q503.7656,234.5256 503.6563,234.01 Q503.6094,233.6506 503.4219,233.4631 Q503.0938,233.0881 502.4844,232.8694 Q501.875,232.6506 501.25,232.6506 Q500.4844,232.6506 499.8438,232.9788 Q499.2188,233.3069 498.7188,234.0569 Q498.2344,234.8069 498.2344,235.8381 L498.2344,236.9319 Q498.2344,238.1663 499.125,238.9944 Q500.0156,239.8069 501.6094,239.8069 Q502.5469,239.8069 503.2031,239.5569 Q503.5938,239.4006 504.0156,238.9631 Q504.2813,238.6975 504.4219,238.6194 Q504.5781,238.5413 504.7813,238.5413 Q505.1094,238.5413 505.3594,238.8069 Q505.625,239.0569 505.625,239.4006 Q505.625,239.7444 505.2813,240.1506 Q504.7813,240.7288 503.9844,241.0569 Q502.9063,241.51 501.6094,241.51 Q500.0938,241.51 498.8906,240.885 Q497.9063,240.385 497.2188,239.3225 Q496.5313,238.2444 496.5313,236.9631 L496.5313,235.8069 Q496.5313,234.4788 497.1406,233.3381 Q497.7656,232.1819 498.8594,231.5725 Q499.9531,230.9475 501.1875,230.9475 Q501.9219,230.9475 502.5625,231.1194 Q503.2188,231.2756 503.7656,231.635 Z " fill="#000000"/><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="152" x="515" y="241.4885">ConsultarHistoricoVenta</text><line style="stroke:#181818;stroke-width:0.5;" x1="487" x2="669" y1="251.76" y2="251.76"/><line style="stroke:#181818;stroke-width:0.5;" x1="487" x2="669" y1="259.76" y2="259.76"/></g><!--MD5=[ff4ee7c548b4e3b0c36f635dcbd8d015]
class Compras--><g id="elem_Compras"><rect fill="#F1F1F1" height="48" id="Compras" rx="2.5" ry="2.5" style="stroke:#181818;stroke-width:0.5;" width="89" x="290.5" y="345.76"/><ellipse cx="305.5" cy="361.76" fill="#ADD1B2" rx="11" ry="11" style="stroke:#181818;stroke-width:1.0;"/><path d="M308.2656,357.635 Q308.4219,357.4163 308.6094,357.3069 Q308.7969,357.1975 309.0156,357.1975 Q309.3906,357.1975 309.625,357.4631 Q309.8594,357.7131 309.8594,358.3225 L309.8594,359.7756 Q309.8594,360.385 309.625,360.6506 Q309.3906,360.9163 309.0156,360.9163 Q308.6719,360.9163 308.4688,360.7131 Q308.2656,360.5256 308.1563,360.01 Q308.1094,359.6506 307.9219,359.4631 Q307.5938,359.0881 306.9844,358.8694 Q306.375,358.6506 305.75,358.6506 Q304.9844,358.6506 304.3438,358.9788 Q303.7188,359.3069 303.2188,360.0569 Q302.7344,360.8069 302.7344,361.8381 L302.7344,362.9319 Q302.7344,364.1663 303.625,364.9944 Q304.5156,365.8069 306.1094,365.8069 Q307.0469,365.8069 307.7031,365.5569 Q308.0938,365.4006 308.5156,364.9631 Q308.7813,364.6975 308.9219,364.6194 Q309.0781,364.5413 309.2813,364.5413 Q309.6094,364.5413 309.8594,364.8069 Q310.125,365.0569 310.125,365.4006 Q310.125,365.7444 309.7813,366.1506 Q309.2813,366.7288 308.4844,367.0569 Q307.4063,367.51 306.1094,367.51 Q304.5938,367.51 303.3906,366.885 Q302.4063,366.385 301.7188,365.3225 Q301.0313,364.2444 301.0313,362.9631 L301.0313,361.8069 Q301.0313,360.4788 301.6406,359.3381 Q302.2656,358.1819 303.3594,357.5725 Q304.4531,356.9475 305.6875,356.9475 Q306.4219,356.9475 307.0625,357.1194 Q307.7188,357.2756 308.2656,357.635 Z " fill="#000000"/><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="57" x="319.5" y="367.4885">Compras</text><line style="stroke:#181818;stroke-width:0.5;" x1="291.5" x2="378.5" y1="377.76" y2="377.76"/><line style="stroke:#181818;stroke-width:0.5;" x1="291.5" x2="378.5" y1="385.76" y2="385.76"/></g><!--MD5=[42ab3172323ec0cd54427087d08fabe5]
class Comprador--><g id="elem_Comprador"><rect fill="#F1F1F1" height="48" id="Comprador" rx="2.5" ry="2.5" style="stroke:#181818;stroke-width:0.5;" width="103" x="274.5" y="219.76"/><ellipse cx="289.5" cy="235.76" fill="#ADD1B2" rx="11" ry="11" style="stroke:#181818;stroke-width:1.0;"/><path d="M292.2656,231.635 Q292.4219,231.4163 292.6094,231.3069 Q292.7969,231.1975 293.0156,231.1975 Q293.3906,231.1975 293.625,231.4631 Q293.8594,231.7131 293.8594,232.3225 L293.8594,233.7756 Q293.8594,234.385 293.625,234.6506 Q293.3906,234.9163 293.0156,234.9163 Q292.6719,234.9163 292.4688,234.7131 Q292.2656,234.5256 292.1563,234.01 Q292.1094,233.6506 291.9219,233.4631 Q291.5938,233.0881 290.9844,232.8694 Q290.375,232.6506 289.75,232.6506 Q288.9844,232.6506 288.3438,232.9788 Q287.7188,233.3069 287.2188,234.0569 Q286.7344,234.8069 286.7344,235.8381 L286.7344,236.9319 Q286.7344,238.1663 287.625,238.9944 Q288.5156,239.8069 290.1094,239.8069 Q291.0469,239.8069 291.7031,239.5569 Q292.0938,239.4006 292.5156,238.9631 Q292.7813,238.6975 292.9219,238.6194 Q293.0781,238.5413 293.2813,238.5413 Q293.6094,238.5413 293.8594,238.8069 Q294.125,239.0569 294.125,239.4006 Q294.125,239.7444 293.7813,240.1506 Q293.2813,240.7288 292.4844,241.0569 Q291.4063,241.51 290.1094,241.51 Q288.5938,241.51 287.3906,240.885 Q286.4063,240.385 285.7188,239.3225 Q285.0313,238.2444 285.0313,236.9631 L285.0313,235.8069 Q285.0313,234.4788 285.6406,233.3381 Q286.2656,232.1819 287.3594,231.5725 Q288.4531,230.9475 289.6875,230.9475 Q290.4219,230.9475 291.0625,231.1194 Q291.7188,231.2756 292.2656,231.635 Z " fill="#000000"/><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="71" x="303.5" y="241.4885">Comprador</text><line style="stroke:#181818;stroke-width:0.5;" x1="275.5" x2="376.5" y1="251.76" y2="251.76"/><line style="stroke:#181818;stroke-width:0.5;" x1="275.5" x2="376.5" y1="259.76" y2="259.76"/></g><!--MD5=[f1bb1dd1304d20aae45885461e08742c]
class Ofertas--><g id="elem_Ofertas"><rect fill="#F1F1F1" height="48" id="Ofertas" rx="2.5" ry="2.5" style="stroke:#181818;stroke-width:0.5;" width="79" x="158.5" y="345.76"/><ellipse cx="173.5" cy="361.76" fill="#ADD1B2" rx="11" ry="11" style="stroke:#181818;stroke-width:1.0;"/><path d="M176.2656,357.635 Q176.4219,357.4163 176.6094,357.3069 Q176.7969,357.1975 177.0156,357.1975 Q177.3906,357.1975 177.625,357.4631 Q177.8594,357.7131 177.8594,358.3225 L177.8594,359.7756 Q177.8594,360.385 177.625,360.6506 Q177.3906,360.9163 177.0156,360.9163 Q176.6719,360.9163 176.4688,360.7131 Q176.2656,360.5256 176.1563,360.01 Q176.1094,359.6506 175.9219,359.4631 Q175.5938,359.0881 174.9844,358.8694 Q174.375,358.6506 173.75,358.6506 Q172.9844,358.6506 172.3438,358.9788 Q171.7188,359.3069 171.2188,360.0569 Q170.7344,360.8069 170.7344,361.8381 L170.7344,362.9319 Q170.7344,364.1663 171.625,364.9944 Q172.5156,365.8069 174.1094,365.8069 Q175.0469,365.8069 175.7031,365.5569 Q176.0938,365.4006 176.5156,364.9631 Q176.7813,364.6975 176.9219,364.6194 Q177.0781,364.5413 177.2813,364.5413 Q177.6094,364.5413 177.8594,364.8069 Q178.125,365.0569 178.125,365.4006 Q178.125,365.7444 177.7813,366.1506 Q177.2813,366.7288 176.4844,367.0569 Q175.4063,367.51 174.1094,367.51 Q172.5938,367.51 171.3906,366.885 Q170.4063,366.385 169.7188,365.3225 Q169.0313,364.2444 169.0313,362.9631 L169.0313,361.8069 Q169.0313,360.4788 169.6406,359.3381 Q170.2656,358.1819 171.3594,357.5725 Q172.4531,356.9475 173.6875,356.9475 Q174.4219,356.9475 175.0625,357.1194 Q175.7188,357.2756 176.2656,357.635 Z " fill="#000000"/><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="47" x="187.5" y="367.4885">Ofertas</text><line style="stroke:#181818;stroke-width:0.5;" x1="159.5" x2="236.5" y1="377.76" y2="377.76"/><line style="stroke:#181818;stroke-width:0.5;" x1="159.5" x2="236.5" y1="385.76" y2="385.76"/></g><!--MD5=[5309a96cdd996ef96cbc3c9ac6102b67]
class Precios--><g id="elem_Precios"><rect fill="#F1F1F1" height="48" id="Precios" rx="2.5" ry="2.5" style="stroke:#181818;stroke-width:0.5;" width="79" x="349.5" y="76.26"/><ellipse cx="364.5" cy="92.26" fill="#ADD1B2" rx="11" ry="11" style="stroke:#181818;stroke-width:1.0;"/><path d="M367.2656,88.135 Q367.4219,87.9162 367.6094,87.8069 Q367.7969,87.6975 368.0156,87.6975 Q368.3906,87.6975 368.625,87.9631 Q368.8594,88.2131 368.8594,88.8225 L368.8594,90.2756 Q368.8594,90.885 368.625,91.1506 Q368.3906,91.4162 368.0156,91.4162 Q367.6719,91.4162 367.4688,91.2131 Q367.2656,91.0256 367.1563,90.51 Q367.1094,90.1506 366.9219,89.9631 Q366.5938,89.5881 365.9844,89.3694 Q365.375,89.1506 364.75,89.1506 Q363.9844,89.1506 363.3438,89.4787 Q362.7188,89.8069 362.2188,90.5569 Q361.7344,91.3069 361.7344,92.3381 L361.7344,93.4319 Q361.7344,94.6662 362.625,95.4944 Q363.5156,96.3069 365.1094,96.3069 Q366.0469,96.3069 366.7031,96.0569 Q367.0938,95.9006 367.5156,95.4631 Q367.7813,95.1975 367.9219,95.1194 Q368.0781,95.0412 368.2813,95.0412 Q368.6094,95.0412 368.8594,95.3069 Q369.125,95.5569 369.125,95.9006 Q369.125,96.2444 368.7813,96.6506 Q368.2813,97.2287 367.4844,97.5569 Q366.4063,98.01 365.1094,98.01 Q363.5938,98.01 362.3906,97.385 Q361.4063,96.885 360.7188,95.8225 Q360.0313,94.7444 360.0313,93.4631 L360.0313,92.3069 Q360.0313,90.9787 360.6406,89.8381 Q361.2656,88.6819 362.3594,88.0725 Q363.4531,87.4475 364.6875,87.4475 Q365.4219,87.4475 366.0625,87.6194 Q366.7188,87.7756 367.2656,88.135 Z " fill="#000000"/><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="47" x="378.5" y="97.9885">Precios</text><line style="stroke:#181818;stroke-width:0.5;" x1="350.5" x2="427.5" y1="108.26" y2="108.26"/><line style="stroke:#181818;stroke-width:0.5;" x1="350.5" x2="427.5" y1="116.26" y2="116.26"/></g><!--MD5=[e363550a3c76349e2d25d63e24111731]
class Vendedor--><g id="elem_Vendedor"><rect fill="#F1F1F1" height="48" id="Vendedor" rx="2.5" ry="2.5" style="stroke:#181818;stroke-width:0.5;" width="94" x="278" y="471.76"/><ellipse cx="293" cy="487.76" fill="#ADD1B2" rx="11" ry="11" style="stroke:#181818;stroke-width:1.0;"/><path d="M295.7656,483.635 Q295.9219,483.4163 296.1094,483.3069 Q296.2969,483.1975 296.5156,483.1975 Q296.8906,483.1975 297.125,483.4631 Q297.3594,483.7131 297.3594,484.3225 L297.3594,485.7756 Q297.3594,486.385 297.125,486.6506 Q296.8906,486.9163 296.5156,486.9163 Q296.1719,486.9163 295.9688,486.7131 Q295.7656,486.5256 295.6563,486.01 Q295.6094,485.6506 295.4219,485.4631 Q295.0938,485.0881 294.4844,484.8694 Q293.875,484.6506 293.25,484.6506 Q292.4844,484.6506 291.8438,484.9788 Q291.2188,485.3069 290.7188,486.0569 Q290.2344,486.8069 290.2344,487.8381 L290.2344,488.9319 Q290.2344,490.1663 291.125,490.9944 Q292.0156,491.8069 293.6094,491.8069 Q294.5469,491.8069 295.2031,491.5569 Q295.5938,491.4006 296.0156,490.9631 Q296.2813,490.6975 296.4219,490.6194 Q296.5781,490.5413 296.7813,490.5413 Q297.1094,490.5413 297.3594,490.8069 Q297.625,491.0569 297.625,491.4006 Q297.625,491.7444 297.2813,492.1506 Q296.7813,492.7288 295.9844,493.0569 Q294.9063,493.51 293.6094,493.51 Q292.0938,493.51 290.8906,492.885 Q289.9063,492.385 289.2188,491.3225 Q288.5313,490.2444 288.5313,488.9631 L288.5313,487.8069 Q288.5313,486.4788 289.1406,485.3381 Q289.7656,484.1819 290.8594,483.5725 Q291.9531,482.9475 293.1875,482.9475 Q293.9219,482.9475 294.5625,483.1194 Q295.2188,483.2756 295.7656,483.635 Z " fill="#000000"/><text fill="#000000" font-family="sans-serif" font-size="14" lengthAdjust="spacing" textLength="62" x="307" y="493.4885">Vendedor</text><line style="stroke:#181818;stroke-width:0.5;" x1="279" x2="371" y1="503.76" y2="503.76"/><line style="stroke:#181818;stroke-width:0.5;" x1="279" x2="371" y1="511.76" y2="511.76"/></g><!--MD5=[d20768d34e4e8467ac91302bf7ce0d3f]
link Comprador to Compras--><g id="link_Comprador_Compras"><path codeLine="21" d="M327.67,267.79 C328.85,283.96 330.45,306.07 331.86,325.48 " fill="none" id="Comprador-to-Compras" style="stroke:#181818;stroke-width:1.0;"/><polygon fill="none" points="338.84,324.98,333.31,345.43,324.88,325.99,338.84,324.98" style="stroke:#181818;stroke-width:1.0;"/><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="49" x="333" y="312.2551">Finalizar</text></g><!--MD5=[ae038c0d206b3314b9bd8e5e96d8d824]
link Comprador to Ofertas--><g id="link_Comprador_Ofertas"><path codeLine="22" d="M298.16,267.94 C287.57,277.02 275.53,287.66 265,297.76 C254.24,308.09 242.96,319.71 232.78,330.51 " fill="none" id="Comprador-to-Ofertas" style="stroke:#181818;stroke-width:1.0;"/><polygon fill="none" points="237.6,335.61,218.87,345.5,227.34,326.08,237.6,335.61" style="stroke:#181818;stroke-width:1.0;"/><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="55" x="266" y="312.2551">Consultar</text><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="20" x="201.6554" y="334.7735">1..*</text></g><!--MD5=[53ad0cc2ef6a32f6ea59a50508fb06c1]
reverse link Precios to Comprador--><g id="link_Precios_Comprador"><path codeLine="23" d="M364.72,142.24 C359.53,151.76 354.31,161.98 350,171.76 C343.12,187.35 336.99,205.58 332.66,219.66 " fill="none" id="Precios-backto-Comprador" style="stroke:#181818;stroke-width:1.0;"/><polygon fill="none" points="358.79,138.5,374.74,124.54,370.97,145.4,358.79,138.5" style="stroke:#181818;stroke-width:1.0;"/><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="55" x="351" y="186.2551">Consultar</text></g><!--MD5=[cff3c82f54c258799cccda1fc53f98e0]
reverse link Productos to Comprador--><g id="link_Productos_Comprador"><path codeLine="24" d="M257.39,138.39 C255.39,154.83 255.65,173.97 263,189.76 C268.43,201.42 277.83,211.43 287.73,219.52 " fill="none" id="Productos-backto-Comprador" style="stroke:#181818;stroke-width:1.0;"/><polygon fill="#181818" points="258.08,133.38,252.9082,141.7617,257.4089,138.3348,260.8358,142.8354,258.08,133.38" style="stroke:#181818;stroke-width:1.0;"/><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="45" x="264" y="186.2551">Agregar</text><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="20" x="234.888" y="154.2657">1..*</text><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="7" x="270.0264" y="208.7987">1</text></g><!--MD5=[268cd9e7c89642762d4c2e7f0b9d21c1]
link Proovedor to Precios--><g id="link_Proovedor_Precios"><path codeLine="25" d="M147.65,58.63 C187.71,32.18 244.32,6 294.5,23.76 C321.69,33.39 346.78,54.54 364.27,72.16 " fill="none" id="Proovedor-to-Precios" style="stroke:#181818;stroke-width:1.0;"/><polygon fill="#181818" points="368.1,76.1,364.6575,66.8724,364.6004,72.5289,358.9438,72.4718,368.1,76.1" style="stroke:#181818;stroke-width:1.0;"/><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="55" x="238.5" y="25.2551">Consultar</text><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="7" x="148.7905" y="47.9161">1</text><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="20" x="340.1819" y="65.3992">1..*</text></g><!--MD5=[9883091d7127910f8023c892882e1d40]
link Proovedor to Ofertas--><g id="link_Proovedor_Ofertas"><path codeLine="26" d="M110.64,141.89 C131.81,196.85 169.01,293.48 187.27,340.91 " fill="none" id="Proovedor-to-Ofertas" style="stroke:#181818;stroke-width:1.0;"/><polygon fill="#181818" points="189.09,345.61,189.5764,335.7732,187.2874,340.9462,182.1144,338.6573,189.09,345.61" style="stroke:#181818;stroke-width:1.0;"/><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="55" x="160" y="249.2551">Consultar</text><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="7" x="105.6507" y="163.6161">1</text><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="20" x="164.2443" y="334.9117">1..*</text></g><!--MD5=[778a4712bb417aa70406fa58042cbdf4]
reverse link Ofertas to Proovedor--><g id="link_Ofertas_Proovedor"><path codeLine="27" d="M153.94,348.03 C123.64,331.13 85.78,304.09 68,267.76 C48.5,227.91 61.53,176.92 75.43,141.92 " fill="none" id="Ofertas-backto-Proovedor" style="stroke:#181818;stroke-width:1.0;"/><polygon fill="#181818" points="158.35,350.45,152.3751,342.6206,153.9638,348.0497,148.5346,349.6385,158.35,350.45" style="stroke:#181818;stroke-width:1.0;"/><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="64" x="69" y="249.2551">Incoorporar</text><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="20" x="130.437" y="343.6206">1..*</text><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="7" x="64.7532" y="163.3403">1</text></g><!--MD5=[2074ddc396b7e6ee2376ecc2efdb117a]
link Precios to Vendedor--><g id="link_Precios_Vendedor"><path codeLine="28" d="M402.45,136.99 C405.95,147.98 409.24,160.23 411,171.76 C421.15,238.37 493.11,125.41 397,393.76 C388.04,418.79 355.0191,462.4929 355.0191,462.4929 " fill="none" id="Precios-Vendedor" style="stroke:#181818;stroke-width:1.0;"/><polygon fill="#181818" points="347.24,471.63,354.1752,469.6545,355.0191,462.4929,348.0838,464.4684,347.24,471.63" style="stroke:#181818;stroke-width:1.0;"/><polygon fill="#181818" points="398.15,124.34,397.249,134.1476,399.7542,129.0757,404.8261,131.5808,398.15,124.34" style="stroke:#181818;stroke-width:1.0;"/><line style="stroke:#181818;stroke-width:1.0;" x1="399.7542" x2="402.33" y1="129.0757" y2="136.65"/><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="55" x="431" y="312.2551">Consultar</text><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="7" x="345.0421" y="460.9368">1</text></g><!--MD5=[85b7bb01aa6d9f7dd0f364e77e7a9036]
reverse link Ofertas to Vendedor--><g id="link_Ofertas_Vendedor"><path codeLine="29" d="M225.41,397.52 C247.95,419.53 279.58,450.41 301.11,471.43 " fill="none" id="Ofertas-backto-Vendedor" style="stroke:#181818;stroke-width:1.0;"/><polygon fill="#181818" points="221.59,393.79,225.2552,402.9315,225.1752,397.2752,230.8315,397.1952,221.59,393.79" style="stroke:#181818;stroke-width:1.0;"/><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="55" x="271" y="438.2551">Consultar</text><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="20" x="204.9026" y="415.1353">1..*</text><text fill="#000000" font-family="sans-serif" font-size="13" lengthAdjust="spacing" textLength="7" x="287.4337" y="461.0875">1</text></g><!--MD5=[b7b5d5abd1e86f3dd83c32d0a03bd960]
