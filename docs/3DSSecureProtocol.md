<!--
type: tab
title: ¿Qué es el Protocolo 3-D Secure?
-->

# ¿Qué es el Protocolo 3-D Secure?

El protocolo 3-D Secure es un documento que describe la infraestructura y los componentes del EMV 3-D Secure para la autenticación del tarjetahabiente durante una transacción de comercio electrónico. Fue creado por EMVCo, un organismo global que busca la interoperabilidad en transacciones electrónicas de modo seguro.

El protocolo de autenticación 3-D Secure se basa en un modelo de tres dominios, en el que el Dominio del Adquirente y el Dominio del Emisor están conectados por el Dominio de Interoperabilidad a través de una serie de mensajes, con el fin de autenticar a un tarjetahabiente durante una transacción de comercio electrónico (e-commerce) o para verificar la identidad o la cuenta del tarjetahabiente en autenticaciones de no pago. El proceso de autenticación puede darse mediante un flujo sin fricción o con fricción dependiendo del nivel de legitimidad evaluado en la información provista por el tarjetabiente.

# Dominios y Componentes

El protocolo 3-D Secure en su modelo posee tres dominios que se comunican entre sí y entre los cuales fluyen los mensajes para el proceso de autenticación. 
Así mismo, estos dominios poseen una serie de componentes en cada uno, los cuales cumplen funciones específicas en el flujo de autenticación.

Los dominios son los siguientes:

**1. Dominio Adquiriente: **Inicia el flujo de autenticación. 

El dominio Adquiriente tiene los siguientes componentes:
      
- Entorno de solicitud de 3DS (3DS Requestor Environment)
    - Solicitante 3DS (3DS Requestor)
    - Cliente 3DS (3DS Client)
    - Servidor 3DS (3DS Server)
          
- Integrador 3DS (3DS Integrator)
- Adquiriente (Acquirer)

**2. Dominio de Interoperabilidad:** Conecta al dominio Adquiriente y Emisor a través de los mensajes que contienen información acerca de la autenticación.

El dominio de Interoperabilidad tiene los siguientes componentes:
      
- Servidor de Directorio (Directory Server, DS)
- Autoridad de Certificación del Servidor de Directorio (Directory Server Certificate Authority, DS CA)
- Sistema de autorización (Authorisation System)

**3. Dominio Emisor: **Las transacciones se autentican en este dominio. 
El dominio Emisor tiene los siguientes componentes:
       
- Titular de la tarjeta (Cardholder)
- Dispositivo de consumo (Consumer Device)
- Emisor (Issuer)
- Servidor de Control de Acceso (Access Control Server, ACS)

# Funcionamiento del componente 3DS Server

El componente 3DS Server pertenece al Dominio del Adquiriente. Este componente se comunica con el comercio o pasarela de pagos, para permitir las autenticaciones de las transacciones electrónicas. 

Este componente se encarga de:

- Recopilar los datos necesarios para los mensajes de 3-D Secure.

- Recibir la petición de sesión enviada por el comercio o pasarela de pagos.

- Responder al comercio o pasarela la petición de sesión. En esta respuesta se incluye la redirectUrl (url de redirección), en la cual el cliente realiza el proceso de autenticación.

- Recibir la petición de información enviada por el comercio o pasarela de pagos.

- Solicitar a la franquicia emisora, la validación del tarjetahabiente.

- Responder al comercio o pasarela de pagos la petición de información. En esta respuesta se incluye el estado final de la autenticación.

# Mensajes del Procolo 3-D Secure y su relación con el 3DS Server

El protocolo 3-D Secure define una serie de mensajes de petición y de respuesta, para ofrecer información acerca del estado del proceso de autenticación y del tipo de flujo en el que se encuentra.

> El componente de 3DS Server, se encarga de crear los siguientes mensajes:

**AReq (Authentication Request Message): **
      El mensaje AReq es el mensaje inicial en el flujo de autenticación 3-D Secure. El 3DS Server crea este mensaje cuando inicia el proceso de autenticación. Puede contener información del titular de la tarjeta, el pago y el dispositivo para la transacción. 

**RRes (Results Response Message): **
      El mensaje RRes comunica el resultado del mensaje RReq. El mensaje es creado y enviado por el 3DS Server a través del DS al ACS. 
      
**PReq (Preparation Request Message): **
      El mensaje PReq se crea y envía desde el 3DS Server al DS para solicitar información sobre el ACS y DS. Este mensaje no forma parte del flujo de mensajes de autenticación de 3-D Secure.

**Error Message: **
      Los mensajes de error proporcionan información adicional sobre un error que se produjo durante el procesamiento de un mensaje.
      
      
> Además, el componente 3DS Server valida los siguientes mensajes:
      

**ARes (Authentication Response Message):**
      El mensaje ARes es la respuesta al mensaje AReq. Puede indicar que el tarjetahabiente ha sido autenticado, o que se requiere una mayor interacción del tarjetahabiente para completar la autenticación (autenticación con challenge). 

**RReq (Results Request Message): **      
      El mensaje RReq comunica los resultados de la autenticación. Este mensaje es enviado por el componente ACS al DS y es recibido por el 3DS Server. Este mensaje no está presente en una transacción sin fricción.
      
**PRes (Preparation Response Message): **      
      El mensaje RReq comunica los resultados de la autenticación. Este mensaje es enviado por el componente ACS al DS y es recibido por el 3DS Server. Este mensaje no forma parte del flujo de mensajes de autenticación de 3-D Secure.

> Finalmente, están los mensajes originados en un flujo con fricción o challenge:

**CReq (Challenge Request Message): **      
      Inicia la interacción del tarjetahabiente en un flujo con challenge.
      
**CRes (Challenge Response Message): **      
      Indica el resultado de la autenticación o también puede indicar que se requiere la interacción del tarjetahabiente para completar la autenticación.


# Canales del dispositivo 

Los canales son los medios por los cuales un cliente puede iniciar el flujo de autenticación, dependiendo del dispositivo utilizado al momento de realizar la transacción electrónica.

Los campos de un mensaje específico pueden variar dependiendo del dispositivo utilizado por el cliente. 

Los siguientes son los canales del dispositivo posibles:

- **APP: **Autenticación de una transacción originada en una aplicación del comercio o pasarela de pago.
      
- **BRW:** Autenticación de una transacción originada en un sitio web del comercio o pasarela de pago, que utiliza un navegador.
      
- **RI:** Autenticación para confirmar la cuenta y verificar la identidad del tarjetahabiente. Este tipo de autenticación es de no pago y no requiere la presencia del tarjetahabiente. Se puede utilizar  por ejemplo para confirmar suscripciones.

# Categorías de los mensajes 

Los mensajes creados por el Procolo 3-D Secure, están categorizados en dos grupos:

- **PA (Payment Authentication):** Autenticación para transacciones de comercio electrónico que incluyen pago.
      
- **NPA (Non-Payment Authentication):** Autenticación de no pago, utilizada para verficar la identidad y la cuenta del tarjetahabiente.

# Flujos de autenticación 

El protocolo 3-D Secure contiene dos posibles flujos para el proceso de autenticación del tarjetahabiente:

- **Flujo sin fricción:**
      
  El flujo sin fricción o sin challenge, no requiere interacción adicional por parte del tarjetahabiente para lograr una autenticación exitosa con 3-D Secure, ya que se evalúa la información obtenida del tarjetahabiente como legítima y de bajo riesgo. Se considera información de bajo riesgo por ejemplo cuando el tarjetabiente registra los mismos datos personales que suele registrar.
      
  Este flujo inicia el proceso de autenticación de 3-D Secure y consiste en el envío de un mensaje de petición de autenticación (AReq) y posteriormente, un mensaje de respuesta a la autenticación (ARes).

---         
        
- **Flujo con fricción o challenge:**

  Este flujo se presenta si el componente ACS determina que la interacción del tarjetahabiente es necesaria para completar la autenticación. Esta determinación puede originarse porque la transacción es considerada de alto riesgo, se encuentra por encima de ciertos umbrales o requiere un mayor nivel de autenticación debido a mandatos o regulaciones del país. 
      
  Ocurre entonces que el flujo sin fricción pasa a ser un flujo con fricción o challenge, donde el challenge consiste en un desafío que se le presenta al tarjetahabiente para comprobar la legitimidad de su identidad y de su cuenta. 
      
### Los tipos de challenge posibles son:
  
  - **Autenticación con challenge:** Se suele presentar al tarjetahabiente un formulario de preguntas sobre su información personal.

  - **Autenticación desacoplada:** En esta autenticación el flujo se pone en pausa y es el emisor de la tarjeta el que se comunica con el tarjetabiente para comprobar los datos dados y lo hace a través de un proceso manual.
          
  - **Autenticación fuera de banda:** El proceso de comprobación de los datos del tarjetabiente queda a cargo del emisor de la tarjeta. Puede incluir otros medios de autenticación como un QR, un código enviado a una app, entre otros.
      
> En cuanto a los mensajes presentes en este tipo de flujo, en adición a los mensajes AReq y ARes que comprenden el flujo sin fricción. El flujo con fricción o challenge comprende los mensajes CReq y CRes (excepto en el caso de una autenticación desacoplada) y los mensajes RReq y RRes.
  
  - El mensaje CReq se construye basado en la información recibida en el mensaje ARes.
  
  - El mensaje CRes puede indicar el resultado de la autenticación o puede indicar que se requiere mayor interacción del tarjetahabiente para completar la autenticación. Este mensaje es la respuesta al mensaje CReq.
  
> Para la autenticación desacoplada, en lugar de utilizar CReq y CRes mensajes, el ACS autentica al titular de la tarjeta fuera del 3-D Secure protocolo.
  
  - El mensaje RReq se construye basado en la información recibida en el mensaje Ares y comunica los resultados de la autenticación.
  
  - El mensaje RRes comunica la recepción del mensaje RReq y los resultados de la autenticación y su estado.

<!-- type: tab-end -->
