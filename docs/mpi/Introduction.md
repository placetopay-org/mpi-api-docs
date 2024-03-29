# Introducción

3DS Placetopay es el servicio de [Evertec, Inc](https://www.evertecinc.com) que facilita al adquirente la posibilidad de enrolar a los comercios y enrutar las transacciones a través del protocolo EMV® 3DS. Este servicio permite realizar el proceso de autenticación del usuario, reduciendo así la exposición de los comercios a los contracargos. Utilizar 3DS Placetopay puede aumentar la seguridad y la eficiencia en las transacciones en línea.

## Redes Soportadas

3DS Placetopay se encuentra certificado en las versiones EMV® 3DS 2.1.0 y 2.2.0 en los siguientes programas:

|                           | EMV® 3DS 2.1.0 | EMV® 3DS 2.2.0 |
|---------------------------|----------------|----------------|
| Visa Secure               | **Soportado**  | **Soportado**  |
| Mastercard Identity Check | **Soportado**  | **Soportado**  |
| American Express SafeKey® | **Soportado**  | **Soportado**  |
| Discover ProtectBuy       | **Soportado**  | **Soportado**  |
| Diners ProtectBuy         | **Soportado**  | **Soportado**  |
| ELO (Brasil)              | En progreso    | En progreso    |

**Nota:** "Soportado" significa que la red ya está completamente integrada y funcional. "En progreso" indica que estamos trabajando en la integración y se espera que esté disponible próximamente.

Actualmente, estamos en el proceso de obtener la certificación para EMV® 3DS 2.3.1, la cual esperamos completar en 2024.

## Acerca de este Documento
Este documento inicialmente describe qué es el protocolo 3DS y ofrece información básica necesaria para entender el proceso de autenticación en el 3DS Server.

Detalla cómo configurar la aplicación desde la consola administrativa, las funcionalidades disponibles y cómo se manejan la seguridad y los permisos. Además, presenta el esquema del flujo del 3DS Server en el proceso de autenticación del tarjetahabiente.

En la sección de la API, se definen los endpoints del servicio, los campos a recibir y sus especificaciones, así como ejemplos de peticiones y respuestas. También se incluyen datos de tarjetas de prueba y sus respectivos comportamientos.

El documento también abarca términos y definiciones, códigos de error, códigos HTTP y los estados posibles para una autenticación. Incluye una sección de Preguntas Frecuentes (FAQ) para resolver dudas y conflictos.

La información contenida en este documento está diseñada para ser útil y comprensible tanto para los colaboradores de Evertec Placetopay como para los comercios interesados en integrarse con este servicio.
