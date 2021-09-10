<!--
type: tab
title: Información General 
-->

# Comercios en MPI

## ¿Qué es un comercio?

Un comercio en MPI son todas aquellas organizaciones establecidas legalmente y con convenio con Evertec Placetopay, que permiten la compra y venta de bienes o servicios de forma virtual, utilizando los productos que ofrece la compañía en cuanto a soluciones transaccionales y de seguridad.

## ¿Cómo acceder a la gestión de comercios de MPI?

Para acceder al listado de comercios de la aplicación siga los siguientes pasos:

1. Remítase al menú lateral izquierdo dónde visualizará tres opciones, "Tablero", "Configuración" y "Seguridad", seleccione **Configuración** y luego **Comercios**:

    ![](https://wiki.placetopay.com/images/d/d2/Mpi-merchants-menu-2.png)

2. Visualizará una pantalla similar a la siguiente:

    ![](https://wiki.placetopay.com/images/8/8b/Merchant-index-2.png)

<!--
type: tab
title: Creación de un comercio
-->

# ¿Cómo crear un comercio en MPI?

Para crear un comercio, haga clic en el botón **Crear** ubicado en la parte lateral derecha del índice de comercios.

Visualizará un formulario similar al siguiente:

![](https://wiki.placetopay.com/images/2/22/Merchant-create.png)

Para diligenciarlo tenga en cuenta los siguientes datos:

- **Nombre:** Ingrese en este campo el nombre del comercio que va a crear.

- **Marca:** Ingrese en este campo el nombre de la marca oficial del comercio que va a crear.

- **País:** Seleccione de la lista desplegable el país dónde opera el comercio.

- **Documento:** Seleccione de la lista desplegable el documento con el cual se identifica al comercio, y en el campo siguiente digite el número de documento correspondiente al tipo seleccionado.

- **Moneda:** Seleccione de la lista desplegable la moneda con la cual procesa las transacciones el comercio.

- **Clase CIIU:** Seleccione de la lista desplegable la clase de categoría de actividad económica del comercio, para ello guíese con el indicador numérico que precede a la descripción de la actividad. Para más información de este campo, puede dirigirse al módulo de esta documentación en la siguiente ruta: **Funcionamiento de MPI** -> **Configuración** -> **Otras configuraciones** -> **Clases CIIU**.

- **Código de categoría del comerciante:** Seleccione de la lista desplegable el código de categoría del comerciante correspondiente al comercio a registrar, para ello guíese con el indicador numérico que precede a la descripción de la actividad. Para más información de este campo, puede dirigirse al módulo de esta documentación en la siguiente ruta: **Funcionamiento de MPI** -> **Configuración** -> **Otras configuraciones** -> **Códigos del comercio**.

- **Consultor comercial:** Seleccione de la lista desplegable el consultor comercial que opera para el comercio en el país seleccionado.

- **Aliado comercial:** Seleccione de la lista desplegable el aliado comercial que opera para el comercio en el país seleccionado.

- **Url:** Ingrese una URL válida que funcionará para conectar el comercio con MPI. A esta URL se redirigirá el usuario al procesar una autenticación.

- **Habilitar/Deshabilitar:** Puede habilitar o deshabilitar un comercio, deslizando el botón tipo switch con nombre *Habilitar* cuando está deshabilitado el comercio, o con nombre *Deshabilitar* cuando está habilitado y desea deshabilitarlo.


## ¿Cuáles son los requerimientos para crear un comercio en MPI?

Para crear y configurar un comercio en MPI, se requiere inicialmente que tenga un convenio y esté certificado con Evertec Placetopay, también que el país y el idioma con el cual opera el comercio, estén disponibles para MPI.

Se requiere que exista una relación entre emisor, adquiriente y comercio y que estos estén registrados en las aplicaciones de ACS y de MPI de Evertec Placetopay, para lograr un proceso de autenticación exitosa utilizando el protocolo 3-D Secure. 

Importante tener en cuenta que previo a la creación del comercio, debe haber creado previamente en MPI, el consultor y el aliado comercial con los cuales operarán el comercio.

<!--
type: tab
title: Índice de comercios 
-->

# Índice de comercios

En esta sección se visualiza el listado o índice de comercios, la información se presenta en una tabla donde se muestran los datos principales de cada comercio, tales como: Nombre, Documento, País, Estado y acciones disponibles para cada comercio. 

![](https://wiki.placetopay.com/images/4/43/Merchant-index-1.png)

### Buscador de comercios:

El índice de comercios tiene la funcionalidad de buscador,está ubicado en la parte lateral izquierda y se puede buscar por el nombre completo del comercio, el documento, el código ISO alfa-3 o fragmentos de éstos datos.

### Acciones disponibles para los comercios:

En el índice de comercios se encuentran las acciones disponibles para cada comercio. Para visualizarlo, diríjase a cada registro de comercio y en la parte lateral derecha encontrará un menú con tres puntos, haga clic en este menú y despliegue las acciones, en las cuales se encuentran:

- **Ver:** Seleccione esta opción para visualizar los detalles del comercio, sus configuraciones y componentes.

  Visualizará una pantalla similar a la siguiente:

  ![](https://wiki.placetopay.com/images/1/1f/Merchant-detail.png)

- **Editar:** Seleccione esta opción para actualizar o corregir los datos con los cuales creó el comercio. Visualizará un formulario similar al de creación del comercio. Todos los datos son editables.

  En el formulario de edición también se encuentra la opción de deshabilitar:

  - **Habilitar/Deshabilitar:** Deslice el botón tipo switch para habilitar el comercio si se encuentra deshabilitado o para deshabilitarlo cuando se encuentre habilitado. Esta opción se encuentra en la vista de editar comercio.

    > Tenga en cuenta que al inhabilitar un comercio resultará en el fallo de todas las transacciones y usuarios dependientes del mismo.


- **Eliminar:** Puede eliminar un comercio, haciendo clic en la opción *Eliminar*. 

<!--
type: tab
title: Importación de comercios
-->

# Importación de comercios

En el índice de comercios, en la parte lateral derecha, se encuentra el acceso a la funcionalidad de importación de comercios, para acceder a esta, haga clic en el botón **Importe**.

<!--
type: tab
title: Métricas de los comercios
-->

# Métricas de los comercios

En el índice de comercios, en la parte lateral derecha, se encuentra el acceso a la funcionalidad de métricas para los comercios, para acceder a esta, haga clic en el botón **Métricas**.

<!--
type: tab
title: Información principal del comercio
-->

# Información principal del comercio

Para ir a los detalles de un comercio, haga clic en la acción **Ver** del menú desplegable del comercio. 

En la vista del detalle se encuentra la información con la cual se creó el comercio, el estado en que se encuentra(está habilitado o no), las fechas de creación del comercio y de actualización y los usuarios que hicieron la creación y/o la actualización.

Además, en la parte lateral derecha, hay un botón para acceder al formulario de edición en caso de requerirlo. Y a la opción de eliminar.

Además, tiene los accesos para gestionar las sucursales de un comercio, los contactos y los adjuntos.

En la siguiente imagen se resalta el acceso a cada uno de estos módulos y se describen a continuación:

![](https://wiki.placetopay.com/images/4/49/Merchant-components.png)

<!--
type: tab
title: Gestión de sucursales 
-->

# Gestión de sursales

Para acceder a este menú, haga clic en el menú **Sucursales**, que se ubica al lado derecho del menú **Detalles del comercio**, en el detalle del comercio.

Luego visualizará una vista similar a la siguiente:

![](https://wiki.placetopay.com/images/f/fb/Merchant-branches.png)

En ella encontrará el listado de sucursales agregadas para el comercio, un buscador de sucursales en el cual puede hacer búsquedas por nombre, marca o país. Además, de las acciones y el botón para crear nueva sucursal.

### Agregar una nueva sucursal:

Para crear una nueva sucursal para el comercio, haga clic en el botón **Crear**, ubicado en la parte lateral derecha y visualizará un formulario como el siguiente:

![](https://wiki.placetopay.com/images/5/5d/Create-branch.png)

Para diligenciarlo tenga en cuenta los siguientes datos:

- **Nombre:** Ingrese en este campo el nombre de la sucursal que va a crear.

- **Marca:** Ingrese en este campo el nombre de la marca oficial del comercio al cual le va a crear una nueva sucursal.

- **País:** Seleccione de la lista desplegable el país dónde opera la sucursal.

- **Moneda:** Seleccione de la lista desplegable la moneda con la cual procesa las transacciones la sucursal.

- **Url:** Ingrese una URL válida que funcionará para conectar la sucursal con MPI. A esta URL se redirigirá el usuario al procesar una autenticación.

- **Habilitar/Deshabilitar:** Puede habilitar o deshabilitar la sucursal, deslizando el botón tipo switch con nombre *Habilitar* cuando está deshabilitada la sucursal, o con nombre *Deshabilitar* cuando está habilitada y desea deshabilitarla.

<!--
type: tab
title: Gestión de contactos 
-->

# Gestión de contactos

Para acceder a este menú, haga clic en el menú **Contactos**, que se ubica al lado derecho del menú **Sucursales**. 

Luego visualizará un índice como el siguiente:

![](https://wiki.placetopay.com/images/3/3d/Contacts-index.png)

En ella encontrará el listado de contactos agregados para el comercio, un buscador de contactos en el cual puede hacer búsquedas por nombre, tipo o correco electrónico. Además, de las acciones y el botón para crear un nuevo contacto.

### Agregar un nuevo contacto:

Para crear una nueva sucursal para el comercio, haga clic en el botón **Crear**, ubicado en la parte lateral derecha y visualizará un formulario como el siguiente:

![](https://wiki.placetopay.com/images/c/c1/Create-contact.png)

Para diligenciarlo tenga en cuenta los siguientes datos:

- **Tipo de adjunto:** Seleccione de la lista desplegable el tipo de contacto que desea agregar al comercio.

- **Nombre:** Ingrese el nombre del contacto o persona.

- **Apellido:** Ingrese el apellido del contacto o persona.

- **Correo electrónico:** Ingrese el correo electrónico
del contacto.

- **Cargo:** Ingrese el nombre del cargo que ocupa el contacto.

- **Tipo de documento:** Seleccione de la lista desplegable el documento con el cual se identifica el contacto.

- **Documento:** Digite el número de documento correspondiente al tipo seleccionado.

- **Móvil:** Ingrese el teléfono correspondiente al móvil, ingrese solo números en este campo.

- **Teléfono:** Ingrese el teléfono correspondiente al fijo u otro número móvil, ingrese solo números en este campo.

- **Dirección:** Ingrese la direcció en la cual se encuentra ubicado el contacto.

<!--
type: tab
title: Gestión de adjuntos 
-->

# Gestión de adjuntos

Para acceder a este menú, haga clic en el menú **Adjuntos**, que se ubica al lado derecho del menú **Contactos**. 

Luego visualizará un índice como el siguiente:

![](https://wiki.placetopay.com/images/d/d3/Attachments-index.png)

En ella encontrará el listado de adjuntos agregados para el comercio, un buscador de adjuntos en el cual puede hacer búsquedas por nombre o tipo. Además, de las acciones y el botón para crear un nuevo adjuntos.

### Agregar un nuevo adjunto:

Para crear una nueva sucursal para el comercio, haga clic en el botón **Crear**, ubicado en la parte lateral derecha y visualizará un formulario como el siguiente:

![](https://wiki.placetopay.com/images/1/15/Attachment-create-mpi.png)

Para diligenciarlo tenga en cuenta los siguientes datos:

- **Tipo de adjunto:** Seleccione de la lista desplegable el tipo de archivo adjunto que desea cargar.

- **Nombre:** Ingrese en el campo el nombre a asignarle al nuevo tipo de archivo adjunto.

- **Carga de archivo:** Haga clic en el campo y se redireccionará a los archivos de su equipo personal, seleccione y cargue el archivo que desea subir.

### ¿Cómo descargar el archivo creado?

Al dar clic en el botón **Guardar**, se redireccionará a una vista como la siguiente, en la cual puede descargar el archivo creado, haciendo clic en el botón **Descargar**:

  ![](https://wiki.placetopay.com/images/a/a7/Attachment-detail.png)

<!--
type: tab
title: Secciones en el detalle del comercio 
-->

# Otras gestiones en el detalle del comercio

En el detalle de un comercio se encuentra la gestión de diversos componentes y configuraciones que requiere este para su buen funcionamiento.

La siguiente imagen muestra cada una de estas secciones y se procede a describir cada una a continuación:

![](https://wiki.placetopay.com/images/2/21/Merchant-detail-sections.png)


<!-- type: tab-end -->
