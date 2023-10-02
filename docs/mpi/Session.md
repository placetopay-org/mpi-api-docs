# Sesión

El término **"Sesión"** Se refiere a la solicitud de autenticación en el contexto de 3DS. Para llevar a cabo una solicitud de autenticación exitosa, es esencial crear una sesión que se ajuste a las especificaciones y necesidades del protocolo 3DS. Puedes encontrar los detalles en [API - Iniciar Sesión](crear-una-nueva-sesion).

**Autorización:** Hace referencia al método indispensable de autorización con nuestra API para realizar peticiones. Dicho método se basa en **Bearer Token**. Para más información, consulta [Autorización](authorization).

**Crear Sesión:** Al enviar una solicitud para crear una sesión, 3DS Placetopay comprueba que el rango de la tarjeta sea compatible con el protocolo 3DS (donde verifica la versión del protocolo que soporta). Una vez realizada la verificación, responde proporcionando la URL hacia donde se realizará la redirección para completar el proceso de autenticación.

### Ejemplo de solicitud
```json
{
  "acctNumber": "4009000000502",
  "cardExpiryDate": "2902",
  "purchaseAmount": "10",
  "redirectURI": "https://www.placetopay.com/web",
  "purchaseCurrency": "USD",
  "reference": "1234567890"
}
```
*Este es el ejemplo más básico para crear una sesión de autenticación*

### Respuesta
```json
{
  "sessionToken": "d801d6f4993fc2efd3aff71a162f33888c19282e4686bd50ff4b8624e1527dbc",
  "redirectURL": "https://3dss.placetopay.com/threeds/v2/sessions/571/d801d6f4993fc2efd3aff71a162f33888c19282e4686bd50ff4b8624e1527dbc",
  "transactionID": 580
}
```

> La sesión cuenta con una duración de 15 minutos, periodo durante el cual se debe redirigir al usuario (redirectURL).

## Posibles errores


| Código | Causa                                                                            |
|--------|----------------------------------------------------------------------------------|
| 1003   | No existe un comercio asociado                                                   | 
| 1004   | No existe una suscripción asociada                                               | 
| 1005   | La marca asociada no está habilitada                                             | 
| 1006   | El adquirente asociado no está habilitado                                        | 
| 1007   | La suscripción asociada no está completamente configurada                        | 
| 1011   | Argumentos no válidos para iniciar la solicitud / El comercio no está habilitado | 
| 1012   | El comerciante no tiene un código de categoría de comercio (MCC)                 | 

```json
{
    "error_number": 1011,
    "error_description": "Invalid arguments to initiate request",
    "errors": {
        "purchaseCurrency": [
            "The purchase currency field is required when purchase amount is present."
        ]
    }
}
```
*Ejemplo de un mensaje de error*


### Mensaje de "Unauthenticated"
```json
{
  "message": "Unauthenticated."
}
```
Este mensaje se puede presentar cuando en los siguientes casos:
- El token no existe.
- El token se encuentra expirado.
