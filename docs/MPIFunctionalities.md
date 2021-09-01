<!--
type: tab
title: Métricas
-->

# Métricas

Las métricas son estadísticas que reportan el comportamiento de la aplicación conforme al flujo de transacciones procesadas.

Para acceder a la gestión de métricas de la aplicación vaya al menú lateral izquierdo, seleccione la opción *Tablero* y luego *Métricas*.

![](https://wiki.placetopay.com/images/e/ea/Mpi-metrics-menu-2.png)

## Filtros:

Para mostrar en la gráfica de la métrica los datos específicos que se requieran, se debe hacer un filtro de las transacciones. 

Para acceder a los filtros haga clic en el botón **Filtrar**, ubicado en la parte superior lateral derecha.

### Datos en los filtros:

La vista de filtros se visualiza de la siguiente manera:

![](https://wiki.placetopay.com/images/a/af/Mpi-filters-metrics-2.png)

Para filtrar las transacciones se requieren los siguientes datos:

- **Rango de fecha,** seleccione una fecha inicial y una posterior en el calendario. Luego de clic en el botón con ícono de *check*, para guardar el rango.

- **Periodo,** seleccione si desea filtrar por días con fechas o por días con sus nombres.

- **Moneda,** divisa utilizada al procesas las transacciones a filtrar.

- **Comercio,** comercio para el cual se procesaron las transacciones a buscar.

### Tipos de métricas:

MPI cuenta actualmente con los siguientes dos tipos de métricas:

## Métrica de verificaciones

## Métrica de autenticaciones

## Métrica de flujo de autenticación

## Métrica de razones por rechazo de marca

## Métrica de tasa de conversión

## Métrica de estado de transacción

## Métrica de tasa de sesiones

ej

## Métrica por estado de transacción

Esta métrica muestra en una gráfica la cantidad de transacciones procesadas por el ACS, filtradas por un rango de fechas y diferenciadas por el estatus obtenido en la autenticación. 

Un ejemplo de métrica por estado de transacción, se presenta a continuación:

![](https://wiki.placetopay.com/images/8/8f/Acs-metric.png)

En la parte inferior puede visualizarse el rango de fecha con el cual se obtuvo la métrica y la cantidad de transacciones que cumplieron con los filtros.

> Para generar nuevas métricas, haga clic en el botón *Limpiar filtros* y genera un nuevo rango de fechas, moneda y emisor.


<!--
type: tab
title: Transacciones
-->

# Transacciones

Para acceder a la gestión de transacciones, vaya al menú lateral izquierdo, seleccione la opción *Tablero* y luego *Transacciones*.

![](https://wiki.placetopay.com/images/1/1a/Mpi-metrics-transactions-2.png)

## Índice de transacciones:

En este módulo se registra la información de todas las autenticaciones procesadas por el ACS. En la primera vista se encuentra el listado de las transacciones con fecha, estado y otros datos importantes. También, puede desplegar más información de cada transacción con el botón desplegable ubicado antes del botón *Ver*.

![](https://wiki.placetopay.com/images/f/fd/Acs-auth-index.png)

## Filtros:

Para buscar un listado o una transacción en específico puede utilizar los filtros. ACS cuenta con dos tipos de filtros para las autenticaciones, uno básico y otro avanzado para hacer consultas más rigurosas.

Para acceder a la funcionalidad, dé clic en el botón *Filtrar* ubicado en la parte lateral superior izquierda de la vista:

#### Filtros básicos:

![](https://wiki.placetopay.com/images/b/b7/Acs-auth-filters.png)

La búsqueda se hace por:

- **Rango de fecha:** Debe dar clic en una fecha inicial del calendario y luego en otra fecha posterior a la primera (el rango no debe ser mayor a 60 días y no debe superar la fecha actual), luego dé clic en el botón negro para guardar el rango de fechas.

- **ID de la transacción:** Aquí se registra el identificador único de la transacción.


#### Filtros avanzados:

![](https://wiki.placetopay.com/images/6/67/Acs-advanced-filters.png)

Al desplegar los filtros básicos, hay una opción *Ver filtros avanzados*, seleccionela y se desplegará una vista como la siguiente:

Aquí además de los dos filtros básicos, se pueden agregar más datos de búsqueda, tales como:

- BIN
- Últimos 4 dígitos del número de tarjeta
- Número de tarjeta
- Banco emisor
- Estado de la transacción


## Detalle de una transacción:

En el detalle de la autenticación, el cual se puede visualizar dando clic en el botón *Ver* de una autenticación, se encuentra información esencial del proceso de autenticación, como el estado de la autenticación, la información básica de la transacción, la información del tarjetahabiente, del comercio, los datos de entrega y una línea de tiempo con los detalles de todo el proceso de autenticación y de la información captada por cada uno de los mensajes presentes en el proceso y correspondientes al protocolo 3-D Secure.

![](https://wiki.placetopay.com/images/b/be/Acs-auth-details.png)

### Calificación:

Algunas autenticaciones cuentan con calificaciones que permiten darle un puntaje de seguridad. Este puntaje determina el nivel de riesgo de la transacción, teniendo en cuenta el historial de transacciones que poseen características similares.

![](https://wiki.placetopay.com/images/5/5f/Acs-scores.png)

### Información de entrega:

Aquí se visualiza la información relacionada con la ubicación en la cual se va a entregar el bien o servicio adquirido con la transacción. También, se puede visualizar un mapa con la ubicación.

![](https://wiki.placetopay.com/images/d/d6/Acs-delivery-data.png)


### Traza de la autenticación:

Cada autenticación tiene una traza, la cual se entiende en ACS como una línea secuencial que registra los pasos realizados en el proceso de autenticación, los datos que recibe, las peticiones y respuestas de los tipos de mensaje que procesa, los estados y descripción de errores si se presentan.

Este es un ejemplo de una traza de una autenticación exitosa:

![](https://wiki.placetopay.com/images/c/c4/Acs-auth-trace.png)

Además, cada paso tiene la opción *Ver más*, la cual muestra la estructura de la petición o la respuesta con sus respectivos datos. Un ejemplo de este detalle es el siguiente:

![](https://wiki.placetopay.com/images/c/c1/Acs-trace-detail.png)

<!--
type: tab
title: Reportes
-->

# Reportes

Para acceder al módulo de reportes, diríjase al menú lateral izquierdo, despliegue la opción *Tablero* y busque la sección de *Reportes* en los títulos.

![](https://wiki.placetopay.com/images/e/e4/Mpi-metrics-reports-2.png)

## Índice de reportes:

Los reportes son archivos que contienen registros de las autenticaciones procesadas por ACS. La siguiente imagen muestra un ejemplo de la vista con el índice de reportes generados. Estos reportes se pueden ver y descargar los archivos con toda la información de los mismos.

![](https://wiki.placetopay.com/images/1/12/Acs-report-index.png)

## ¿Cómo crear nuevos reportes?

Para crear un nuevo reporte haga clic en el botón *Crear*. 
Actualmente se manejan dos tipos de reportes:

### Reportes de Autenticaciones

El sistema de reportes permite generar un archivo con el reporte de las autenticaciones procesadas por ACS. Para el reporte se puede definir un rango de fechas, identificador de la transacción, BIN de tarjetas, banco emisor y uno o varios estados de las autenticaciones que se desean registrar en el reporte. El siguiente es un ejemplo de creación de un reporte de autenticaciones:

![](https://wiki.placetopay.com/images/b/bd/Acs-auth-report.png)

### Reportes de Abandonos 

Con este reporte se generan los datos de las autenticaciones que son abandonadas en el ACS. Para el reporte se puede definir un rango de fechas y el banco emisor. El siguiente es un ejemplo de creación de un reporte de abandonos:

![](https://wiki.placetopay.com/images/4/42/Acs-abandoned-report.png)


## Tipos de archivos generados para los reportes
- Archivo separado por comas.
- Archivo separado por tabuladores.
- Archivo de Excel


<!-- type: tab-end -->

