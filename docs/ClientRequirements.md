# Requerimientos para el cliente que va a integrarse

Para integrarse al servicio de 3DS Server o 3DS Secure Merchant Plugin (MPI) de Evertec, el comercio o pasarela deberá cumplir con los siguientes requisitos, necesarios para garantizar la compatibilidad en la conexión:

- **Encabezados HTTP:** Los encabezados HTTP deben estar parametrizados con los siguientes valores:

        Content-Type: application/json; charset=UTF-8

- ** Método HTTP:** Las peticiones al servicio de autenticación deben hacerse usando el método POST.

- **Comunicaciones seguras:** Para establecer los enlaces asegurados por Transport Layer Security (TLS), entre el servicio y los clientes conectados, el número de versión debe ser 1.2 o superior. Las claves RSA deben tener una longitud mínima de 2048 bits.
    
- **Autenticación:** Cualquier petición al servicio requiere un token de autenticación. El token se enviará en el encabezado HTTP como un “Bearer Token” de acuerdo con el RFC 6750. 
      
  Ejemplo de un Bearer Token:	

      Authorization:"Bearer 1c6b2cda415f40f6f9f82e24d31d3fa6deb3cbcdd1def686fef7ed721a8abf83"
