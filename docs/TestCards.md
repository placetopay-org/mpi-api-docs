# Tarjetas de Prueba

Los siguientes números de tarjetas de crédito le permitirán hacer peticiones al servicio y obtener las respuestas específicas que se describen para cada una.


Tarjeta           | Comportamiento                                                                                 |
----------------- |------------------------------------------------------------------------------------------------|
 4005580000000040 | Autentica de manera satisfactoria con un flujo sin fricción (transStatus = Y).                 |  
 4009000000502    | Requiere challenge en el proceso de autenticación (transStatus = C).                           | 
 4009000000403    | El emisor rechaza la autenticación (transStatus = R).                                          |
 4005580000000008 | La autenticación no se puede realizar porque el dispositivo no es soportado (transStatus = U). | 
 4009000000304    | Genera un intento de autenticación (transStatus = A).                                          | 
 4100000000038    | La transacción es de información y no pago(transStatus = I).                                   | 