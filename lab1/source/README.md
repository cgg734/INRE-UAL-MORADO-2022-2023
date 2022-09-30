# Horarios
En una universidad, el personal del PDI, el personal del PAS y los estudiantes pueden consultar horarios. Por su parte, el personal del PAS puede modificar horarios y dar de alta estudiantes. El personal de PDI puede proponer cambios en los horarios y dar de alta estudiantes. La funcionalidad de dar de alta estudiantes del PAS realiza una verificación de los datos del estudiante. Sin embargo, la funcionalidad de dar de alta estudiantes del PDI, además de verificar los datos también permite de forma excepcional realizar la búsqueda en las listas de clase de sus asignaturas.

| ***UC-01*** |  |
| --- | --- |
| ***Nombre:***  | Proponer cambios en el horario. |
| ***Autor:***  | Fehri Gil Fernandez Besada |
| ***Fecha:***  | 30/09/22 |
<<<<<<< HEAD
| ***Descripcion:*** | <br> El personal PDI puede proponer cambios en el horario. |
| ***Actores:***  | <br>  PersonalPDI. |
| ***Precondicion:*** |  <br>  El personal PDI debe estar registrado. |
| ***Flujo Normal:***  | <br>  1. El personal PDI debe pulsar un boton para modificar el horario. <br> 2. El actor rellena un formulario con los cambios realizados. <br> 3. El actor pulsa un botón para confirmar los cambios. |


<br>
<br>

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

4.B.- El sistema comprueba que los datos introducidos son correctos, en caso de que los datos no lo sean, se avisara al usuario que los corrija.<br>
|***Postcondiciones*** | <br> El sistema ha comprobado que los datos introducidos son correctos y el horario se muestra satisfactoriamente








=======
| ***Descripcion:*** <br> El personal PDI puede proponer cambios en el horario. |
| ***Actores:*** | <br> PersonalPDI. |
| ***Precondicion:*** | <br>  El personal PDI debe estar registrado. |
| ***Flujo Normal:*** | <br>  1. El personal PDI debe pulsar un botón para proponer cambios en el horario. <br> 2. El actor rellena un formulario con los cambios solicitados. <br> 3. El actor pulsa un botón para confirmar la solicitud. |
| ***Flujo Alternativo:*** | <br>  1. Si al confirmar no se actualiza el horario vuelve a mostrar el formulario. <br> 2. Si no se rellena el formulario se mostrará un mensaje de error. |
| ***Poscondiciones***  <br>  La solicitud se ha realizado correctamente. |
>>>>>>> 8637d28108a2e0d73a771ec0f67a1cf235e1e098

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