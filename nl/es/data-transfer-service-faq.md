---

copyright:
  years: 1994, 2017
lastupdated: "2017-12-18"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Preguntas más frecuentes sobre el servicio de transferencia de datos

## ¿Qué es la transferencia de datos?

La transferencia de datos permite que los usuarios autorizados (generalmente el administrador de la cuenta) envíen dispositivos compatibles a uno de nuestros centros de datos para conectarlos directamente a la red de la cuenta. El dispositivo está alojado en un bastidor dedicado en el centro seleccionado y está montado como un destino iSCSI por un período de dos (2) semanas. Durante ese período, el administrador puede acceder al dispositivo de la red para utilizarlo con otros dispositivos o servicios de la cuenta. Después del período de dos semanas, puede solicitarse una prórroga para mantener el dispositivo conectado a la red. De lo contrario, el dispositivo se devuelve a la parte especificada en el apartado de dirección de devolución al crear la solicitud o se destruye in situ si no se solicita la devolución.


## ¿Se puede hacer un envío internacional de un dispositivo para la transferencia de datos?

El hardware y los discos pueden enviarse tanto a nivel nacional como internacional a cualquiera de nuestros centros. Sin embargo, como el cliente, es responsable de:

- asegurarse de que no se requiera ninguna licencia de importación o exportación para enviar el dispositivo al centro de datos de {{site.data.keyword.IBM}} o devolverlo al cliente (si procede);
- asegurarse de que ni el cliente ni ningún usuario final del cliente cuyos datos se incluyen en el contenido estén sujetos a ninguna orden del gobierno de los Estados Unidos que revoque o deniegue sus privilegios de exportación estadounidenses. El Cliente acepta notificar a {{site.data.keyword.IBM}} inmediatamente si el Cliente o cualquier usuario final queda sujeto a una orden de este tipo;
- obtener todas las licencias, del envío y del despacho de aduanas para el dispositivo, incluidos el pago de aranceles, impuestos y gastos de envío al centro de datos de {{site.data.keyword.IBM}} y desde este (si es aplicable);
- cumplir con todas las leyes aplicables, incluidas la de privacidad, importación y exportación, asociadas con la entrega y la devolución del dispositivo, y la transferencia de contenido al centro de datos de {{site.data.keyword.IBM}}; y
- disponer los acuerdos adecuados en su lugar y obtener todos los permisos necesarios con el usuario final del cliente para cualquier dato de usuario final que el cliente transfiera al hardware.

Incluya una etiqueta de envío de devolución prepagada y todos los documentos de exportación correspondientes con el envío y empaquetaremos los dispositivos para su devolución mediante la etiqueta y los documentos proporcionados. Si no se solicita la devolución, el dispositivo se destruirá.


## ¿Qué tipos de dispositivos se pueden enviar con una solicitud de transferencia de datos?
Utilice las siguientes directrices al seleccionar un dispositivo o disco (CD o DVD) para enviar a la transferencia de datos:

- Requisitos de hardware:
   - La fuente de alimentación debe ser compatible con 208v/220v.

   - El conector debe ajustarse al enchufe estándar de 120 v (NEMA 5-15P).

   - El dispositivo debe ser compatible con USB 2.0 o USB 3.0.

   - Debe proporcione un conector USB A macho (conector USB estándar que se ajusta a la mayoría de los sistemas).
 
- Requisitos de CD/DVD:

   - Los discos deben enviarse en estuches para CD, cajas o contenedores similares. Si envía varios discos, almacénelos juntos en una única caja o funda.

   - Cada disco debe etiquetarse de forma clara y única (es decir, disco A, disco B, disco C, etc.).
   
## ¿Se puedo devolver el dispositivo antes o tenerlo durante más de dos semanas durante el proceso de transferencia de datos? 

Sí, se pueden devolver el hardware o los discos en cualquier momento o tenerlos conectados durante más tiempo si es necesario. Para solicitar una devolución o una prórroga, añada un comentario a la incidencia de solicitud de transferencia de datos original con la solicitud correspondiente. Si solicita una devolución, desconectaremos y devolveremos el hardware o discos a la dirección de envío de devolución proporcionada en la solicitud original mediante las etiquetas de envío prepagadas y con el embalaje proporcionado. 

Si solicita una prórroga, esta se procesará lo antes posible. Es importante tener en cuenta que cada solicitud de prórroga amplía una semana el tiempo que el dispositivo está conectado y puede estar sujeta a una tarifa de prórroga. Se incluirán detalles adicionales cuando un miembro de nuestro equipo responda a la solicitud en la incidencia original.
   
## ¿Qué significan los estados de la incidencia de transferencia de datos?

Los estados de la incidencia de la transferencia de datos indican la fase del proceso de transferencia del hardware o discos enviado al centro de datos. Consulte la tabla siguiente para obtener detalles concretos sobre cada estado:

|Estado 	| Definición |
|---------| -----------|
|Enviado a SoftLayer 	|El usuario ha enviado la solicitud de transferencia de datos y el hardware o discos se están enviando al centro de datos seleccionado.|
|Recibido por SoftLayer |	El centro de datos ha recibido el envío, al que se ha asignado un número de serie y se ha explorado en nuestro sistema.|
|Conectar |	El hardware o disco se ha conectado al dispositivo.|
|Conectado |	Se ha creado un destino iSCSI para el dispositivo.|
|Solicitud de prórroga |	El usuario ha solicitado una prórroga de dos (2) semanas del tiempo de conexión.|
|Solicitud de devolución | El usuario ha solicitado la devolución de hardware o de los discos.|
|Desconectar |	Se ha iniciado la desconexión del hardware o discos.|
|Desconectado |	Los sistemas de información han desconectado de forma segura el objetivo.|
|Destruido | El dispositivo se ha destruido in situ siguiendo el procedimiento de destrucción de unidades de disco duro.|
|Devolución por parte de SoftLayer |	Se han empaquetado los discos o el hardware y se han enviado a la dirección de retorno proporcionada en la solicitud original.|
