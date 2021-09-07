# Franquicias en MPI

## ¿Qué es una franquicia?

Una franquicia de una tarjeta de crédito, es una compañía aliada con los bancos emisores de tarjetas de crédito. Tienen como función proveer diversos beneficios bancarios a sus clientes (tarjetabientes) y gestionar el uso de las tarjetas. 

## ¿Cómo acceder a la gestión de franquicias de MPI?

Para acceder al listado de franquicias de la aplicación siga los siguientes pasos:

1. Remítase al menú lateral izquierdo dónde visualizará tres opciones, "Tablero", "Configuración" y "Seguridad", seleccione la opción **Configuración** y luego **Franquicias**, como muestra la siguiente imagen:

    ![](https://wiki.placetopay.com/images/7/76/Mpi-franchises-menu-2.png)

2. Visualizará una pantalla con el listado de franquicias organizadas en una tabla, la cual corresponde al índice de franquicias:

## ¿Cómo crear una franquicia en MPI?

Para crear una franquicia, haga clic en el botón **Crear** ubicado en la parte lateral derecha del índice de franquicias, posteriormente diligencie los datos del formulario teniendo en cuenta la siguiente información:

- **Marca,** Ingrese el nombre de la franquicia, por ejemplo Mastercard, VISA...

- **ID de negocio,** Ingrese el identificador numérico de la franquicia.

- **Prefijo del Id del solicitante,** Ingrese al menos 3 carácteres que correspondan al identificador del solicitante de la creación de la franquicia.

- **Certificados intermedios,** Copie y pegue en este campo el bloque de texto correspondiente al certificado intermedio.

- **Certificados raíz,** Copie y pegue en este campo el bloque de texto correspondiente al certificado raíz.

En la siguiente imagen se puede visualizar un ejemplo del formulario de creación de una franquicia:

![](https://wiki.placetopay.com/images/9/9f/Create-franchise-mpi.png)

## ¿Cuáles son los requerimientos para crear una franquicia?

Para crear una franquicia, esta debe haber pasado por un proceso de certificación de la marca con PlacetoPay Evertec.

También, la franquicia debe proporcionar información como el tipo de tarjetas que soportan, las clases y los bines aceptados, para proceder a realizar una creación exitosa de franquicia en MPI y que esta coincida con las especificaciones y requerimientos esperados en la aplicación.

## Listado y funciones de las franquicias

En esta sección se visualiza el listado o índice de franquicias en una tabla donde se muestran los datos principales de cada una, tales como: Nombre, ID de negocio Estado y Acciones. 

Al final de cada registro de franquicia, en la parte lateral derecha, se encuentra un menú con tres puntos, haga clic en este menú y despliegue las acciones o funcionalidades disponibles para cada franquicia.

 El menú que se despliega se visualizará como la siguiente imagen:

![](https://wiki.placetopay.com/images/1/13/Franchises-index-mpi.png)

### Acciones para las franquicias:

- **Ver:** Seleccione esta opción para visualizar más detalles de la franquicia.

  Visualizará una vista similar a la siguiente:

  ![](https://wiki.placetopay.com/images/b/b6/Franchise-detail-mpi.png)

- **Habilitar/Deshabilitar:** Esta opción se encuentra disponible en el detalle de la franquicia (diríjase a la imagen anterior para visualizar el botón de deshabilitar), deslice el botón tipo switch para habilitar la franquicia si se encuentra deshabilitada o para deshabilitarla cuando se encuentre habilitada. 
  
  > Al habilitar o deshabilitar, la aplicación le entregará un mensaje de confirmación de habilitación y cambiará el estado en la franquicia editada.

- **Editar:** Seleccione esta opción para actualizar o corregir los datos con los cuales creó la franquicia. 
Visualizará un formulario similar al de creación de la franquicia, el cual se explicó previamente.

- **Eliminar:** Puede eliminar una clase, haciendo clic en la opción *Eliminar*. 

### ¿Qué ocurre al deshabilitar una franquicia?

Tenga en cuenta que si una franquicia se encuentra deshabilitada, no podrá hacer movimientos con ella en la aplicación. Por ejemplo no puede seleccionar una franquicia deshabilitada en el listado de franquicias disponibles, al momento de crear una suscripción de un adquieriente para un comercio. 

Tampoco podrán autenticarse las transacciones cuyas tarjetas pertenezcan a una franquicia deshabilitada. 

Así mismo, deshabilitar una franquicia puede causar el fallo en los adquirientes y comercios que tengan suscrita tal franquicia.

