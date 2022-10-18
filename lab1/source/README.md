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









| ***UC-01*** | --- |
| --- | --- |
| ***Nombre:***  | Consultar horarios. |
| ***Autor:***  | Fehri Gil Fernandez Besada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El usuario puede comprobar el horario correspondiente |
| ***Actores:***  | <br>  Estudiantes. |
| ***Precondicion:*** |  <br>  El estudiante debe de tener sus datos personales en la universidad y por tanto estar dado de alta. |
| ***Flujo Normal:***  | <br>  1. El estudiante accede a la pestaña de horario. <br> 2. El estudiante debe de elegir el dia y el mes. <br> 3. El actor pulsa un botón para el envio del formulario. <br> 4. El sistema comprueba que los datos introducidos. <br> 5. Visualizacion del horario.
|***Flujo Alternativo:*** | <br> 4.A.- El sistema comprueba que los datos introducidos son correctos, en caso de que en el dia no haya ninguna clase se enviara un mensaje de error.<br>

4.B.- El sistema comprueba que los datos in
troducidos son correctos, en caso de que los datos no lo sean, se avisara al usuario que los corrija.<br>
|***Postcondiciones*** | <br> El sistema ha comprobado que los datos introducidos son correctos y el horario se muestra satisfactoriamente

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
<<<<<<< HEAD
| ***Poscondiciones :*** | <br> Los cambios han sido almacenados en el sistema y se actualizan para el resto de usuarios |
=======
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

| ***INF-01*** | Estudiantes |
| --- | --- |
| ***Version:***  | Septiembre-2022 |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Referencias:*** | <br> Ninguna. |
| ***Fuentes:***  | <br>  Mátricula del estudiante   |
| ***Descripción*** | <br> El sistema deberá almacenar los datos correspondientes a los estudiantes. |
| ***Datos especificos:*** |  1. Documento nacional de identidad (DNI) o NIE. <br> 2. Nombre completo. <br> 3.Teléfono de contacto. <br> 4. Sexo del estudiante. <br> 5. Calificaciones.  |
| ***Importancia:*** | <br> Muy importante. |
| ***Estado:*** | <br> Aceptado. |
| ***Comentarios:*** | <br> Los datos del estudiante son imprescindibles en el correcto funcionamiento del sistema.|
<br>

| ***INF-02*** | Personal Docente |
| --- | --- |
| ***Version:***  | Septiembre-2022 |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Referencias:*** | <br> Ninguna. |
| ***Fuentes:***  | <br>  Contrato de trabajo.   |
| ***Descripción*** | <br> El sistema deberá almacenar los datos correspondientes al personal docente. |
| ***Datos especificos:*** |  1. Documento nacional de identidad (DNI) o NIE. <br> 2. Nombre completo. <br> 3.Teléfono de contacto.  <br> 4. Email de contacto. <br> 5. Asignaturas impartidas. <br>   |
| ***Importancia:*** | <br> Muy importante. |
| ***Estado:*** | <br> Aceptado. |
| ***Comentarios:*** | <br> Los datos del personal docente son imprescindibles en el correcto funcionamiento del sistema.|
<br>

| ***INF-03*** | Información sobre horarios. |
| --- | --- |
| ***Version:***  | Septiembre-2022 |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Referencias:*** | <br> Ninguna. |
| ***Fuentes:***  | <br>  Tabla de horarios. |
| ***Descripción*** | <br> El sistema deberá almacenar los datos correspondientes a los horarios de las distintas asignaturas. |
| ***Datos especificos:*** |  1. Nombre de las Asignaturas. <br> 2. Rango de horas en la que se imparte cada asignatura. <br> 3.Día en el que se imparte la asignatura.  |
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

| ***UC-05*** |  |
| --- | --- |
| ***Nombre:***  | Realizar venta. |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Fecha:***  | 30/09/22 |
| ***Descripcion:*** | <br> El comprador puede realizar la compra tras hablar . |
| ***Actores:***  | <br>  Comprador, Vendedor. |
| ***Precondicion:*** | <br>  Vendedor y comprador deben haber acordado un precio. |
| ***Flujo Normal:*** | <br>  1. El comprador debe tener sus productos agregados. <br> 2. El vendedor y el comprador acuerdan el precio.  <br> 3. Llegan a un acuerdo para poder finalizar la compra. |
|***Flujo Alternativo:*** | <br> 3A. Si el comprador no acepta el precio no se llegaria a realizar la compra. |
| ***Poscondiciones :*** | <br>  |
<br>
=======
| ***Descripcion:*** | <br> El comprador y el vendedor pueden realizar una venta simultaneamente. |
| ***Relaciones*** |   |
| ***Actores:***  | <br>  Comprador, Vendedor. |
| ***Precondicion:*** | <br>  El comprador y el vendedor necesitan realizar esta funcion simultaneamente. |
| ***Flujo Normal:*** | <br>  1. Los actores deben introducir la id o palabra clave en el motor de busqueda. <br> 2. El sistema muestra informacin relacionada con los datos introducidos en el buscador. |
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
=======
| ***Poscondiciones :*** | <br> Los cambios han sido almacenados en el sistema y el producto bloqueado para el comprador.|
=======
| ***Poscondiciones :*** | <br> Los cambios han sido almacenados en el sistema y el producto bloqueado para el comprador.|

<br>

| ***INF-01*** | Información sobre los usuarios del sistema.  |
| --- | --- |
| ***Version:***  | Septiembre-2022 |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Referencias:*** | <br> Ninguna. |
| ***Fuentes:***  | <br>     |
| ***Descripción:*** | <br> El sistema deberá almacenar los datos sobre los diferentes roles <br> que ejerce el usuario del sistema. |
| ***Datos especificos:*** |   <br> 1. Nombre completo. <br> 2.Teléfono de contacto.  <br> 3. Email <br> Numero de cuenta bancaria. |
| ***Importancia:*** | <br> Muy importante. |
| ***Estado:*** | <br> Aceptado. |
| ***Comentarios:*** | <br> Los datos de los usuarios son imprescindibles en el correcto funcionamiento del sistema.|

 ***INF-02*** | Información sobre compras.  |
| --- | --- |
| ***Version:***  | Septiembre-2022 |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Referencias:*** | <br> Ninguna. |
| ***Fuentes:***  | <br>     |
| ***Descripción:*** | <br> El sistema deberá almacenar la información correspondiente a las compras realizadas por los compradores. |
| ***Datos especificos:*** |   <br> 1. Número de referencia de la compra: 10 dígitos. <br> 2.Fecha de realización de la compra.  <br> 3. Destino del producto comprado: Calle/Portal/Número. |
| ***Importancia:*** | <br> Muy importante. |
| ***Estado:*** | <br> Aceptado. |
| ***Comentarios:*** | <br> |

 ***INF-02*** | Información sobre las ofertas.  |
| --- | --- |
| ***Version:***  | Septiembre-2022 |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Referencias:*** | <br> Ninguna. |
| ***Fuentes:***  | <br>     |
| ***Descripción:*** | <br> El sistema deberá almacenar la información correspondiente a las diferentes ofertas. |
| ***Datos especificos:*** |   <br> 1. Porcentaje de descuento. <br> 2. Identificador del producto ofertado: 3 dígitos. <br> 3. Fecha de finalización de la oferta: dd/mm/aaaa. |
| ***Importancia:*** | <br> Importante. |
| ***Estado:*** | <br> Aceptado. |
| ***Comentarios:*** | <br> Los productos ofertados deben estar presentes en el sistema junto a sus condiciones para que el comprador la pueda considerar. |
<br>

***INF-03*** | Información sobre compras.  |
| --- | --- |
| ***Version:***  | Septiembre-2022 |
| ***Autor:***  | FehriGilFernandezBesada |
| ***Referencias:*** | <br> Ninguna. |
| ***Fuentes:***  | <br>     |
| ***Descripción:*** | <br> El sistema deberá almacenar la información correspondiente a las compras realizadas por los compradores. |
| ***Datos especificos:*** |   <br> 1. Número de referencia de la compra: 10 dígitos. <br> 2.Fecha de realización de la compra.  <br> 3. Destino del producto comprado: Calle/Portal/Número. |
| ***Importancia:*** | <br> Muy importante. |
| ***Estado:*** | <br> Aceptado. |
| ***Comentarios:*** | <br> |
