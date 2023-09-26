# Términos y Definiciones

Las siguientes definiciones pretenden dar claridad sobre la información presentada a lo largo de este documento.

- **EMVCo:** Es un organismo técnico global de propiedad de American Express, Discover, JCB, MasterCard, UnionPay y Visa. El cual facilita la interoperabilidad mundial y la aceptación de transacciones de pago seguras mediante la utilización de las especificaciones dadas por EMV.
      
- **EMV:** Es una marca comercial que ofrece especificaciones para desarrollar e implementar productos de pago basados en tarjetas que funcionarán juntos de manera transparente y segura, creando con ello interoperabilidad global en el marco transaccional.
      
- **Tarjetahabiente:** Es una persona a la cual se le expide una tarjeta o está autorizada para usar una tarjeta, que en el caso del protocolo, le permitirá hacer compras de comercio electrónico.

- **3DS:** Es un protocolo de mensajería antifraude que le permite a los consumidores autenticarse a sí mismos con el emisor de su tarjeta de pago en el momento de la realización de transacciones no presenciales.

- **ACS:** Access Control Server (ACS) es el componente del protocolo 3DS que opera en el dominio del emisor y tiene como finalidad autenticar al cardholder.

- **RSA:** Es un algoritmo de cifrado asimétrico o de clave pública. Sirve para cifrar y descifrar información, trabajando con dos llaves, una pública y una privada.

- **Token de autenticación:**  Es una cadena de texto que no pretende tener un significado alguno y representa un acceso de autorización que es emitido al cliente. El token permite reemplazar las credenciales de autenticación del propietario directamente, con el fin de proteger la información.

- **RFC 6750:** Es un documento normativo en el cual se define el marco de autorización de OAuth 2.0 para el uso del token de portador. Para ampliar la información, consulte esta url https://tools.ietf.org/html/rfc6750

- **Bank Identification Number (BIN):** Hace referencia a los primeros seis dígitos del número de una tarjeta.

- **Certificado SSL:** Un documento electrónico que contiene una llave pública legalizada o atestiguada por una Autoridad de Certificación (CA). Esta legalización consiste en la firma con la llave privada de la CA.

- **Slug:** Se nombra así a la parte final de la URL que identifica una página dentro de un sitio web.

- **Challenge:** Proceso mediante el cual el ACS se comunica el con 3DS Client para obtener información adicional a través de la interacción con el cardholder.

- **Dispositivo de consumo:** El dispositivo usado por el cardholder (smartphone, laptop, tablet) como conducto para realizar las operaciones de pago (autenticación y compra).

- **Adquiriente:** Es una institución financiera que establece un contrato con los comercios con el objetivo aceptar pagos con tarjeta. En el contexto de 3DS, el Adquirente también tiene la potestad de determinar si un comercio es elegible para participar el protocolo 3DS.