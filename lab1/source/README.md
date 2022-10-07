# Horarios
En una universidad, el personal del PDI, el personal del PAS y los estudiantes pueden consultar horarios. Por su parte, el personal del PAS puede modificar horarios y dar de alta estudiantes. El personal de PDI puede proponer cambios en los horarios y dar de alta estudiantes. La funcionalidad de dar de alta estudiantes del PAS realiza una verificación de los datos del estudiante. Sin embargo, la funcionalidad de dar de alta estudiantes del PDI, además de verificar los datos también permite de forma excepcional realizar la búsqueda en las listas de clase de sus asignaturas.

| ***UC-01*** |  |
| --- | --- |
| ***Nombre:***  | Proponer cambios en el horario. |
| ***Autor:***  | Fehri Gil Fernandez Besada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El personal PDI puede proponer cambios en el horario. |
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
| ***Flujo Normal:*** | <br>  1. El personal PAS debe pulsar un boton para modificar el horario. <br> 2. El actor rellena un formulario con cajas de texto para los nuevos cambios realizados. <br> 3. El actor pulsa un botón para confirmar los cambios. |
|***Flujo Alternativo:*** | <br> 2A. El sistema comprueba los datos del formulario y si no son correctos pide corrección |
| ***Poscondiciones :*** | <br> Los cambios han sido almacenados en el sistema y se actualizan para el resto de usuarios |

| ***UC-04*** |  |
| --- | --- |
| ***Nombre:***  | Dar alta estudiantes PDI |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El personal PDI puede dar de alta a estudiantes PDI. |
| ***Actores:***  | <br>  PersonalPDI. |
| ***Precondicion:*** | <br>  El personal PDI debe estar registrado como PDI. |
| ***Flujo Normal:*** | <br>  1. El personal PDI debe interactuar con un boton para dar de alta a un usuario. <br> 2. El actor rellena un formulario con cajas de texto para los datos del alumno. <br> 3. El actor pulsa un botón para confirmar los cambios. |
|***Flujo Alternativo:*** | <br> 2A. Si el los datos del alumno ya estan registrados en el sistema el personal PDI puede buscar al alumno en las listas de clase |
| ***Poscondiciones :*** | <br> Los cambios han sido almacenados en el sistema y se actualizan para el resto de usuarios |
<br>

| ***UC-05*** |  |
| --- | --- |
| ***Nombre:***  | Buscar en listas de clase. |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El personal PDI de manera opcional puede buscar en las listas de clase. |
| ***Actores:***  | <br>  PersonalPDI. |
| ***Precondicion:*** | <br>  El personal PDI debera estar dando de alta a estudiantes PDI. |
| ***Flujo Normal:*** | <br>  1. El personal PDI debe entrar en la opcion de alumno existente dando de alta a un alumno PDI. <br> 2. El personal PDI debe escoger el alumno ya existente en las listas de clase <br> 3. El actor pulsa un botón para confirmar los cambios. |
|***Flujo Alternativo:*** | <br> 2A. El sistema comprueba los datos del formulario y si no son correctos pide corrección |
| ***Poscondiciones :*** | <br> Los cambios han sido almacenados en el sistema y se actualizan para el resto de usuarios |
<br>

| ***UC-06*** |  |
| --- | --- |
| ***Nombre:***  | Dar alta estudiantes |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El personal PAS puede dar de alta a estudiantes. |
| ***Actores:***  | <br>  PersonalPAS. |
| ***Precondicion:*** | <br>  El personal PAS debe estar registrado como PAS. |
| ***Flujo Normal:*** | <br>  1. El personal PAS debe pulsar un boton para elegir la opcion de dar alta a un estudiante. <br> 2. El actor rellena un formulario con cajas de texto para los datos del estudiante que se va a dar de alta. <br> 3. El actor pulsa un botón para confirmar los cambios. <br> 4. Los datos de los estudiantes deberan ser verificados por el sistema. |
|***Flujo Alternativo:*** | <br> 4A. El sistema verifica los datos y comprueba que son erroneos por lo que se muestra un mensaje al personal PAS. |
| ***Poscondiciones :*** | <br> Los cambios han sido verificados, almacenados en el sistema y actualizados. |
# Sistema de compras
En un sistema de compra, existen cuatro tipos de usuarios: comprador, vendedor, proveedor y administrador. Los compradores pueden agregar productos, consultar precios, finalizar la compra y consultar ofertas. Agregar productos implica marcar esos productos como bloqueados. Los vendedores también pueden consultar ofertas y consultar precios. Los proveedores pueden consultar precios, avisar de nuevos productos y consultar ofertas. Avisar de nuevos productos, de forma excepcional, realiza la incorporación de una oferta. Los proveedores también tienen una funcionalidad para avisar del fin de una oferta. Cuando se avisa del fin de una oferta, se ejecuta la funcionalidad de eliminar la oferta. Ambas funcionalidades de avisar del proveedor tienen en común que se encarga de enviar una notificación. Los administradores pueden consultar precios, consultar ofertas y eliminar productos. La funcionalidad de consultar precios incluye una funcionalidad de buscar productos que es similar a la funcionalidad de consultar productos de los compradores. Sin embargo, la funcionalidad de consultar productos añade una funcionalidad para verificar la disponibilidad. Para realizar una venta, un comprador y un vendedor participan de forma conjunta. En dicha operación, se lleva a cabo el acuerdo de un precio; excepcionalmente, durante la realización de la venta, se consultará el histórico de ventas.
| ***UC-01*** |  |
| --- | --- |
| ***Nombre:***  | Finalizar compra |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El comprador puede finalizar una compra. |
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
| ***Actores:***  | <br>  Comprador. |
| ***Precondicion:*** | <br>  El producto tiene que estar disponible. |
| ***Flujo Normal:*** | <br>  1. El comprador realiza la busqueda del producto a consultar. <br> 2. El sistema comprueba la disponibilad del producto <br> 3. El sistema ofrece informacion del producto consultado |
|***Flujo Alternativo:*** | <br> 3A. Si el producto no esta disponible, se muestra un mensaje advirtiendo de esto el comprador. |
| ***Poscondiciones :*** | <br>  |
<br>

| ***UC-04*** |  |
| --- | --- |
| ***Nombre:***  | Buscar producto. |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El personal PAS puede modificar los horarios. |
| ***Actores:***  | <br>  Comprador, Abstracto. |
| ***Precondicion:*** | <br>  El producto debe existir en el sistema. |
| ***Flujo Normal:*** | <br>  1. Los actores deben introducir la id o palabra clave en el motor de busqueda. <br> 2. El sistema muestra informacin relacionada con los datos introducidos en el buscador. |
|***Flujo Alternativo:*** | <br> 2A. El sistema no encuentra correlaciones con los datos introducidos e informa al usuario |
| ***Poscondiciones :*** | <br> El sistema ha mostrado un mensaje al usuario. |