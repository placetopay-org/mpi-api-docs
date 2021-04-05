# ¿Qué es el Protocolo 3-D Secure?

El protocolo 3-D Secure es un documento que describe la infraestructura y los componentes del EMV 3-D Secure para la autenticación del tarjetahabiente durante una transacción de comercio electrónico. Fue creado por EMVCo, un organismo global que busca la interoperabilidad en transacciones electrónicas de modo seguro.

El protocolo de autenticación 3-D Secure se basa en un modelo de tres dominios, en el que el Dominio del Adquirente y el Dominio del Emisor están conectados por el Dominio de Interoperabilidad a través de una serie de mensajes, con el fin de autenticar a un tarjetahabiente durante una transacción de comercio electrónico (e-commerce) o para verificar la identidad o la cuenta del tarjetahabiente en autenticaciones de no pago.

El protocolo cuenta actualmente con dos versiones activas, la versión 2.10 y la versión 2.2O. La principal diferencia entre ambas versiones es que en la 2.10, la autenticación del tarjetahabiente siempre va a requerir de un reto para comprobar su identidad, el cual consiste en aportar información personal adicional o en la verificación de un código o similares. Mientras que en la versión 2.20, se implementó el flujo de autenticación sin reto o challenge, dado cuando el tarjetahabiente aporta datos completos y seguros; además se creó para esta versión otro tipo de autenticación nombrada como desacoplada.

De esta forma, el proceso de autenticación puede darse mediante un flujo sin fricción o con fricción, entendiendo la fricción como el reto para autenticarse, y es el componente ACS el cual decide cual de estos flujos es el requerido en una autenticación, dependiendo del nivel de legitimidad evaluado en la información provista por el tarjetabiente y de la versión utilizada del protocolo.
