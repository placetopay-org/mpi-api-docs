# Comercios en MPI

[NO ACTUALIZADO]

## ¿Qué es un comercio?

Un comercio es...

Entre las funciones de un emisor están:

- El comercio tiene la responsabilidad de...


## ¿Cómo acceder a la gestión de comercios de MPI?

Para acceder al listado de comercios de la aplicación siga los siguientes pasos:

1. Remítase al menú lateral izquierdo dónde visualizará tres opciones, "Tablero", "Configuración" y "Seguridad", seleccione "Configuración" y luego "Comercios":

![](https://wiki.placetopay.com/images/2/28/Mpi-merchants-menu.png)

2. Visualizará una pantalla similar a la siguiente:

![](https://wiki.placetopay.com/images/4/4e/Issuer-index.png)

## ¿Cómo crear un comercio en MPI?

Para crear un comercio, haga clic en el botón **Crear** ubicado en la parte lateral derecha del índice de comercios.

Visualizará un formulario similar al siguiente:

![]()

Para diligenciarlo tenga en cuenta los siguientes datos:

- **Nombre:** Ingrese en este campo el nombre del banco emisor que va a crear.

- **Idioma:** Seleccione de la lista desplegable el idioma principal con el cual desea que se procesen las autenticaciones para los usuarios.

- **País:** Seleccione de la lista desplegable el país dónde opera el banco emisor.

- **Slug:** Ingrese una cadena clave para el emisor. Esta cadena se agregará a las URL donde se gestionen configuraciones y servicios del emisor.

- **Logo:** Aquí puede cargar una imagen con el logo del emisor. Para hacerlo haga clic en la opción *Seleccionar archivo* y busque la imagen correspondiente al logo en su equipo. La imagen debe tener unas dimensiones máximas de 1000x1000.


## ¿Cuáles son los requerimientos para crear un comercio en MPI?

Para crear y configurar un emisor en ACS, este debe haber emitido tarjetas de pago con las franquicias que ya hayan sido certificadas para funcionar en ACS.

Se requiere que el país y el idioma con el cual se vaya a crear el emisor, estén disponibles para ACS.

Se requiere que exista una relación entre emisor, adquiriente y comercio y que estos estén registrados en las aplicaciones de ACS y de MPI de PlacetoPay Evertec, para lograr un proceso de autenticación exitosa. 

Importante tener en cuenta habilitar todos los campos de configuración del menú *Campos de configuración* de la aplicación, antes de crear el emisor, ya que todos estos campos son requeridos para el funcionamiento básico de un emisor.

> En este punto es importante recordar que la aplicación de **MPI** también implementa y pertenece al flujo propuesto por el protocolo 3-D Secure para autenticar un tarjetahabiente.
Pertenece al dominio el adquiriente y entre sus funciones principales están:
  >> - Recibir y responder la petición de autenticación enviada por el comercio o pasarela de pagos.
  >> - Solicitar al emisor la autorización del pago.
  >> - Responder al comercio o pasarela de pagos el estado final de la autenticación.


## Índice de comercios

En esta sección se visualiza el listado o índice de emisores, la información se presenta en una tabla donde se muestran los datos principales de cada emisor, tales como: Nombre, País y Estado. 

![](https://wiki.placetopay.com/images/4/4a/Issuer-actions.png)

#### Filtros:

En el índice de datos se encuentra la funcionalidad de filtros, esta funcionalidad permite hacer búsquedas específicas de datos. Los filtros están ubicados en la parte superior lateral izquierda.

Para los ** están disponibles para búsquedas, los campos de **.

Para ejecutar la búsqueda haga clic en el botón **Buscar** y para limpiar los datos de búsqueda ingresados previamente, haga clic en el botón **Limpiar filtros**.

![]()

### Acciones disponibles para los comercios:

En el título "Acciones" ubicado en la parte lateral derecha del índice de emisores, se encuentra un menú con tres puntos,haga clic en este menú y despliegue las acciones o funcionalidades disponibles para cada emisor. En el menú se encuentran las siguientes acciones:

- **Ver:** Seleccione esta opción para visualizar los detalles del emisor, sus configuraciones y componentes.

  Visualizará una vista similar a la siguiente:

![](https://wiki.placetopay.com/images/c/c6/Issuer-detail2.png)

- **Editar:** Seleccione esta opción para actualizar o corregir los datos con los cuales creó el emisor. 

  Visualizará un formulario similar al de creación del emisor. Todos los datos son editables.

![](https://wiki.placetopay.com/images/3/3c/Edit-issuer.png)

- **Habilitar o Deshabilitar:** Deslice el botón tipo switch para habilitar el emisor si se encuentra deshabilitado o para deshabilitarlo cuando se encuentre habilitado. 

![](https://wiki.placetopay.com/images/8/81/Issuer-actions-toggle.png)

Al habilitar o deshabilitar, la aplicación le entregará un mensaje de confirmación similar al siguiente e inmediatamente cambiará el estado del emisor editado.

![](https://wiki.placetopay.com/images/c/ca/Issuer-toggle.png)

### ¿Cómo habilitar un comercio?

1. **Active los campos de configuración requeridos:** En el menú *Campos de configuración* de la aplicación, habilite todos los campos de configuración (debe habilitarlos antes de crear el emisor), ya que estos son requeridos para la habilitación del emisor. Para obtener más información de los campos de configuración, vaya al título *Campos de configuración* del presente documento.

    La siguiente imagen muestra un índice de los campos de configuración donde todos los campos visibles están habilitados, así deben estar para comenzar a configurar correctamente el emisor.

    ![](https://wiki.placetopay.com/images/a/a7/Settings-index-2.png)

    > Si algún campo se encuentra deshabilitado, despliegue el menú de la parte lateral derecha y seleccione la opción *Habilitar*.

2. **Habilitar estrategias del emisor:** En los detalles del emisor, en la pestaña *Configuraciones*, y luego en la pestaña *Servicios*, encontrará las estrategias disponibles para el emisor (esta funcionalidad se explica más adelante), debe habilitar ambas estrategias (cardholderStrategy y otpStrategy).

    Un ejemplo del menú *Services* es el siguiente:

   ![](https://wiki.placetopay.com/images/c/c4/Issuer-settings-disable-services.png)

    
    Nótese que en la imagen anterior, las estrategia se encuentran deshabilitadas. Si se intentara habilitar el emisor con una o ambas estrategias deshabilitadas, arrojaría un error como el siguiente y no permitiría ejecutar la habilitación del emisor.

    ![](https://wiki.placetopay.com/images/f/f6/Issuer-enable-error2.png)


3. **Suscribir franquicia al emisor:** En la pestaña *Franquicias suscritas* del detalle del emisor, seleccione una franquicia del listado, sino hay franquicias disponibles, debe ir al menú *Franquicias* de la aplicación y crear una nueva franquicia para el emisor, para esto guíese de la sección *Configuración de franquicias* de la presente documentación.

    > La franquicia seleccionada debe ser diferente a franquicias previamente suscritas a otros emisores. 
    
4. **Configurar rangos de tarjeta para el emisor:** En la pestaña *Gestionar rangos de tarjetas* del detalle del emisor, haga clic en el botón *Crear* y cree rangos de tarjeta manuales o por importación, para ello guíese de la sección *Gestión de rangos de tarjetas* del presente documento.
    
5. **Crear certificado tipo Cliente para las franquicias del emisor:** Para habilitar un emisor debe crear un certificado tipo *CLIENT*, en el menú de *Certificados*, y seleccionar el emisor correspondiente y una franquicia suscrita para el mismo emisor. Luego debe firmar el certificado con la entidad certificadora y en el índice de certificados, este debe registrar en el campo *Certificado* con el estado *Encontrado*, que indica que fue validado correctamente. 

    Para crear el certificado, guíese de la sección *Otras configuraciones* pestaña *Certificados SSL*.

    Un ejemplo de la primera vista del formulario de creación de un certificado es el siguiente:

    ![](https://wiki.placetopay.com/images/8/8a/Client-certificate.png)

## Detalles de un comercio

### Información principal del comercio:

Para ir a los detalles de un emisor, haga clic en la acción *Ver* del menú desplegable del emisor, ubicado en el índice de emisores. 

En la siguiente imagen se visualiza un ejemplo de la parte superior de la vista de *Detalles de un emisor*. En la vista se encuentra la información con la cual se creó el emisor, el estado en que se encuentra el emisor (está habilitado o no),las fechas de creación del emisor y de actualización y los usuarios que hicieron la creación y/o la actualización.

En la parte lateral derecha hay un recuadro en el cual se debe mostrar el logo del emisor, para este ejemplo no se cargó una imagen, por lo cual se muestra en negro.

Además, en la parte lateral derecha, hay un botón para acceder al formulario de edición en caso de requerirlo.

![](https://wiki.placetopay.com/images/c/c6/Issuer-detail2.png)

## Gestión de sursales:

Para acceder a este menú, haga clic en el menú *Franquicias suscritas*, que actualmente se ubica al lado derecho del menú *Detalles del emisor*. 

Luego visualizará una vista similar a la siguiente:

![](https://wiki.placetopay.com/images/6/62/Issuer-franchises.png)

En ella encontrará el listado de franquicias agregadas para el emisor y un formulario para agregar nuevas franquicias.

> Para las franquicias solo está disponible la función de *Eliminar*, la cual se ejecuta dando clic en el botón con el mismo nombre ubicado al frente de cada franquicia.

### Agregar una nueva sucursal:

Para suscribir una nueva franquicia a su emisor, dírijase a la primera sección de la vista actual, al apartado *Franquicia* y despliegue la lista de franquicias disponibles haciendo clic en la flecha hacia abajo. Seleccione una franquicia y haga clic en el botón *Agregar*.

![](https://wiki.placetopay.com/images/1/1f/Add-franchise.png)

## Gestión de contactos:

Para acceder a este menú, haga clic en el menú *Gestionar rangos de tarjetas*, ubicado en la parte superior de la vista.

Visualizará un índice similar al siguiente:

![](https://wiki.placetopay.com/images/2/22/Acs-card-ranges-index.png)

En esta sección se importan y crean los rangos de tarjetas aceptadas para un emisor específico. Puede ver la información principal de cada rango organizada en una tabla, entre los datos están: BIN del rango, Rango inicial, Rango final, Franquicia, Clase y las respectivas acciones que tienen cada uno de los rangos.


### Gestión de adjuntos:

Para acceder a este menú, haga clic en el menú *Configuraciones*, del detalle del emisor. 

Luego visualizará una vista similar a la siguiente:

![](https://wiki.placetopay.com/images/7/75/Issuer-general-settings2.png)

En la parte inferior de la vista, encontrará tres pestañas que contienen los campos de configuración de los emisores, agrupados en tres secciones: General, Desafíos y Servicios.

Ingresando a cada una de las pestañas, podrá ver la información de los campos del emisor organizada en tablas, en las cuales se muestra el nombre, el valor inicial del campo y el estado del mismo.