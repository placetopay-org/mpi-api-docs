<!--
type: tab
title: Preguntas frecuentes
-->

# Preguntas frecuentes sobre el funcionamiento MPI

En esta sección podrá encontrar respuestas a preguntas o solución a problemas que puede encontrarse en MPI.

## ¿Qué significan las siglas MPI?

MPI traduce en inglés Merchant Server Plugin o en español, Complemento del Servidor de Comercio.

## ¿Para qué es necesario MPI?

La aplicación de MPI... verifica si una autenticación está disponible para un número de tarjeta, cumpliendo la importante función de autenticar a los tarjetahabientes en el flujo transaccional. Además, en el proceso de autenticación, es ACS el encargado de validar los datos ingresados y registrados para una transacción.

## ¿Por qué se debe autenticar a un tarjetahabiente?

El proceso de autenticación permite reducir el riesgo de fraude en las transacciones virtuales, a través de la  verificación de cuenta, la identidad del tarjehabiente y la corroboración de información transaccional y personal brindada.

## ¿Cómo se parametriza el proceso de autenticación de un tarjetahabiente?

El Protocolo 3-D Secure es quien define y describe la infraestructura y las pautas para la autenticación del tarjetahabiente durante una transacción de comercio electrónico.

> Recomendamos leer la documentación en su totalidad, ya que en cada una de las secciones se describen situaciones particulares que se pueden experimentar y sus respectivas soluciones

## ¿Cómo acceder a MPI?

Para acceder a la consola de MPI, se requiere de un usuario registrado con el cual procederá a iniciar sesión. 

### Usuario:
Para obtener el usuario de MPI, se debe hacer mediante una invitación que creará un usuario registrado y autenticado actualmente en la aplicación.

> Para obtener más información de las invitaciones, diríjase a la sección de **Seguridad** y luego **Invitaciones**, de esta documentación.

### Activación de usuario:

Posterior a la creación de una invitación, será enviado un correo electrónico al correo registrado en el formulario de creación, con el cual podrá activar el usuario. El correo se verá similar al siguiente:

![](https://wiki.placetopay.com/images/b/be/Invitation-email.png)

Para activar el usuario, haga clic en el botón **Activar Registro** y se redireccionará a la página de inicio de sesión de MPI.

### Inicio de sesión:

La página de inicio de sesión o login será similar a la siguiente:

![](https://wiki.placetopay.com/images/a/ad/Acs-login.png)

En este formulario de inicio de sesión, ingrese el correo electrónico con el cual fue creada la invitación y la contraseña.

### Restablecimiento de contraseña:

Si olvidó la contraseña de inicio de sesión, puede hacer clic en la opción **¿Olvidaste tu contraseña?** y se redireccionará a un formalario para ingresar su correo electrónico y enviar una solicitud de cambio de contraseña. Visualizará un formulario como el siguiente:

![](https://wiki.placetopay.com/images/a/ad/Password-login.png)


## ¿Cómo mostrar datos en las diferentes métricas?

Cuando accede a la sección de métricas puede preguntarse ¿cómo obtener información a partir de las gráficas?, la respuesta a esta pregunta es que debe hacer un filtrado de datos en primer lugar, para ello haga clic en el botón **Filtrar** como lo ilustra la siguiente imagen y posteriormente seleccione los datos con los cuales desea que se grafiquen y se muestren estadísticas de funcionamiento de la aplicación.

![](https://wiki.placetopay.com/images/c/c3/Mpi-metrics-filters.png)

> Para obtener información más detallada del funcionamiento de las métricas, diríjase al menú **Funcionamiento de MPI** -> **Funcionalidades**.

## ¿Puedo acceder a registros de cambios e interacciones realizadas en la aplicación?

La aplicación de MPI contiene un módulo ubicado en el menú **Seguridad** -> **Logs**, donde se registran los movimientos realizados en la aplicación, con el detalle del número de registro, la fecha, hora, usuario, descripción del movimiento y datos del equipo desde el cual se realizó. Se visualizan como el siguiente ejemplo:

![](https://wiki.placetopay.com/images/b/b3/Log-detail.png)

## ¿Cómo se validan los datos que ingresan los usuarios en los diferentes formularios de la aplicación?

### Validación de datos:

Para todos los formularios de la aplicación, se dispone de la funcionalidad de validación de los datos ingresados, lo cual permite asegurar la integridad y veracidad de éstos.

De esta forma, al diligenciar el formulario puede encontrar y verificar dos tipos de validaciones:

1. **Validaciones de lado del cliente:**

    Estas validaciones se realizan cuando un dato no cumple las reglas mínimas de aceptación y no hay necesidad de enviar la respuesta al servidor si se ha validado previamente que está errónea la información. Se visualizan con mensajes en rojo para el campo erróneo y le ofrece al usuario una ayuda de cómo debe diligenciar el campo en cuestión para ser aceptado. Si hay errores en estas validaciones, la aplicación no permite el envío del formulario.

    La siguiente imagen ilustra errores en validaciones del lado del cliente:


    ![](https://wiki.placetopay.com/images/3/30/Issuer-pre-validations.png)

1. **Validaciones de lado del servidor:**

    Estas validaciones se aplican cuando se envía un formulario o unos datos al servidor y estos no cumplen con las validaciones requeridas, por lo cual se genera un error,se deniega la solicitud y posteriormente, se muestra al usuario el error encontrado. Estas validaciones se ejecutan cuando no se han registrado como validaciones del lado del cliente, o son complicadas de validar del lado del cliente o el usuario logra por algún medio pasar el primer filtro de validaciones del cliente con la información errónea, sin embargo, este filtro de validaciones detiene una solicitud con datos inválidos.

    La siguiente imagen ilustra errores en validaciones del lado del servidor, en la cual se logró enviar el formulario con datos inválidos, pero al momento de recibirlo y validarlo, se encontraron errores en los datos de la solicitud, por lo cual no pudo ser procesada correctamente:


    ![](https://wiki.placetopay.com/images/9/91/Image-issuer-error.png)    

<!--
type: tab
title: Eventos frecuentes
-->

# Eventos frecuentes y soluciones 

## ¿Cómo ocultar la pestaña de selección de filtros?

Cuando accede a módulos de la aplicación que contienen la funcionalidad de filtros (para hacer búsquedas específicas de información). Puede encontrarse con la necesidad de ocultar la pestaña de filtros para tener mayor acceso y visualización a la información mostrada.

Para ocultar la pestaña o sección, lo único que debe hacer es dar clic nuevamente en el botón de filtros, como se ilustra en el siguiente ejemplo:

![](https://wiki.placetopay.com/images/6/6b/Mpi-open-filters-2.png)

Luego obtendrá un índice de datos con mejor visualización como se muestra en la siguiente imagen:

![](https://wiki.placetopay.com/images/7/71/Transactions-hidden-filters.png)


<!--
type: tab
title: Contáctenos
-->

# Contacto y soporte

Si existe alguna duda o la solución al problema que posee no está contenida en esta documentación, puede acceder al servicio de posventa que brinda la compañía para atender su requerimiento.

Tenga en cuenta que para brindar un excelente servicio de soporte, es necesario que provea todos los detalles de la incidencia. 

Para acceder a este servicio, puede contactarse por alguno de los siguientes medios y le atenderemos con gusto.

  - **Página web:** https://www.placetopay.com
  - **Teléfonos:** 444 2310 / 317 431 0510
  - **Correo electrónico:** servicioposventa@placetopay.com
  - **Dirección:** Carrera 65 # 45 - 20 oficina 430 Medellín - Colombia


<!-- type: tab-end -->