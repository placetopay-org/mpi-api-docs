# Obtener información de una autenticación

Este servicio le permite consultar el estado de una transacción que pasó por el proceso de autenticación del tarjetahabiente con el 3DS Server.

## Datos del servicio
|          |                                          |
|----------|------------------------------------------|
| Endpoint | **/api/v2/transactions/{transactionID}** |
| Método   | GET                                      |

**Nota:** {transactionID} se debe tomar del dato transactionID en [Crear Sesión](crear-session)

### Respuesta
```json
{
    "enrolled": "Y",
    "transStatus": "Y",
    "transStatusReason": null,
    "eci": "05",
    "acsTransID": "6f4b8e53-d838-4c38-9ab9-e130911503cb",
    "dsTransID": "d991c86e-f21c-412c-9ff7-c91b4eaaaba0",
    "threeDSServerTransID": "549ced88-3a1b-4aa8-8f03-1f8937a6c2f2",
    "sdkTransID": null,
    "authenticationValue": "AJkCBzBjSQAAAAPohAAmdEeHIJE=",
    "messageVersion": "2.2.0",
    "authMethod": "02",
    "authTimestamp": "2020-04-21T01:44:54+00:00",
    "messageCategory": "01"
}
```

## Posibles errores

| Código | Causa                                       |
|--------|---------------------------------------------|
| 403    | El token no está autorizado.                | 
| 404    | Transacción no existe                       | 
| 500    | El servidor ha encontrado un error interno. | 
