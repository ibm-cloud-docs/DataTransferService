---

copyright:
  years: 2017, 2019
lastupdated: "2019-02-05"

---
{:faq: data-hd-content-type='faq'}

# Preguntas más frecuentes

## ¿Qué es la transferencia de datos?
{: faq}

Este servicio permite que los usuarios autorizados (generalmente el administrador de la cuenta) envíen dispositivos compatibles a uno de los centros de datos de {{site.data.keyword.BluSoftlayer_full}} para conectarlos directamente a la red de la cuenta. El dispositivo está alojado en un bastidor dedicado y montado como un destino iSCSI durante dos semanas. Durante ese período, el administrador puede acceder al dispositivo de la red para utilizarlo con otros dispositivos y servicios de la cuenta. Después del período de dos semanas, puede solicitarse una ampliación para mantener el dispositivo conectado a la red. De lo contrario, el dispositivo se devuelve a la parte especificada en la solicitud o se destruye in situ.

## ¿Puede hacerse un envío internacional de un dispositivo para la transferencia de datos?
{: faq}

El hardware y los discos pueden enviarse a nivel nacional como internacional a cualquiera de los centros de datos de {{site.data.keyword.BluSoftlayer}}. Sin embargo, el cliente es responsable de:

- Asegurarse de que no se requiera ninguna licencia de importación o exportación para enviar el dispositivo al centro de datos de {{site.data.keyword.IBM}} o devolverlo al cliente (si procede);
- Asegurarse de que el cliente o cualquier usuario cliente cuyos datos se incluyen en el contenido no estén sujetos a ninguna orden del gobierno de los Estados Unidos que revoque o deniegue sus privilegios de exportación estadounidenses. Debe notificar a {{site.data.keyword.IBM}} inmediatamente si el Cliente o cualquier usuario queda sujeto a una orden de este tipo;
- Obtener todas las licencias, del envío y del despacho de aduanas para el dispositivo, incluidos el pago de aranceles, impuestos y gastos de envío al centro de datos de {{site.data.keyword.IBM}} y desde este (si es aplicable);
- Cumplir con todas las leyes aplicables, incluidas la de privacidad, importación y exportación, asociadas con la entrega y la devolución del dispositivo, y la transferencia de contenido al centro de datos de {{site.data.keyword.IBM}}; y
- Disponer los acuerdos adecuados en su lugar y obtener todos los permisos necesarios con el usuario del cliente para cualquier dato de usuario que el cliente transfiera al hardware.

Incluya una etiqueta de envío de devolución prepagada y todos los documentos de exportación correspondientes con el envío. {{site.data.keyword.BluSoftlayer}} empaqueta los dispositivos para su devolución utilizando la etiqueta y los documentos proporcionados. Si no se solicita la devolución, el dispositivo se destruye.


## ¿Qué tipos de dispositivos pueden enviarse con una solicitud de transferencia de datos?
{: faq}

Utilice las siguientes directrices al seleccionar un dispositivo o disco (CD o DVD) para enviar a la transferencia de datos:

- **Requisitos de hardware**

   - La fuente de alimentación debe ser compatible con 208v/220v.

   - El conector debe ajustarse al enchufe estándar de 120 v (NEMA 5-15P).

   - El dispositivo debe ser compatible con USB 2.0 o USB 3.0.

   - Debe proporcione un conector USB A macho (conector USB estándar que se ajusta a la mayoría de los sistemas).

- **Requisitos de CD/DVD**

   - Los discos deben enviarse en estuches para CD, cajas o contenedores similares. Si desea enviar varios discos, almacénelos juntos en una única caja o funda.

   - Cada disco debe etiquetarse de forma clara y única.

## ¿Puede devolverse el dispositivo antes o puede estarse más de dos semanas?
{: faq}

Sí, se pueden devolver el hardware o los discos en cualquier momento o tenerlos conectados durante más tiempo si es necesario. Para solicitar una devolución o una ampliación, añada un comentario a la incidencia de solicitud de transferencia de datos original con la solicitud correspondiente. Si solicita una devolución, {{site.data.keyword.BluSoftlayer}} desconecta y devuelve el hardware o discos a la dirección de devolución proporcionada en la solicitud original mediante las etiquetas de envío prepagadas y con el embalaje proporcionado.

Si solicita una ampliación, esta se procesará lo antes posible. Es importante tener en cuenta que cada solicitud de ampliación amplía una semana el tiempo que el dispositivo está conectado y puede estar sujeta a una tarifa de ampliación. Se incluirán más detalles cuando un miembro del equipo de {{site.data.keyword.BluSoftlayer_full}} responda a la solicitud en la incidencia original.

Los estados de la incidencia de la transferencia de datos indican la fase del proceso de transferencia del hardware o discos que se han enviado al centro de datos. Consulte la tabla para obtener detalles concretos sobre cada estado:

|Estado 	| Definición |
|---------| -----------|
|`Enviado a SoftLayer` |El usuario ha enviado la solicitud de transferencia de datos y el hardware o los discos se están enviando al centro de datos seleccionado.|
|`Recibido de SoftLayer` |	El centro de datos ha recibido el envío, se ha asignado un número de serie al dispositivo y se ha explorado en el sistema de {{site.data.keyword.BluSoftlayer}}.|
|`Conectar` |	El hardware o disco se ha conectado al dispositivo.|
|`Conectado` |	Se ha creado un destino iSCSI para el dispositivo.|
|`Solicitud de ampliación` | El cliente ha solicitado una ampliación del tiempo de conexión de dos semanas.|
|`Solicitud de devolución` | El cliente ha solicitado la devolución de hardware o de los discos.|
|`Desconectar` |	Se ha iniciado la desconexión del hardware o los discos.|
|`Desconectado` |	El destino se ha desconectado de forma segura.|
|`Destruido` | El dispositivo se ha destruido in situ siguiendo el procedimiento de destrucción de unidades de disco duro de {{site.data.keyword.BluSoftlayer}}.|
|`Devolución por parte de SoftLayer` |	Se han empaquetado los discos o el hardware y se han enviado a la dirección de retorno proporcionada en la solicitud original.|
