---

copyright:
  years: 1994, 2018
lastupdated: "2018-05-22"

---
{:new_window: target="_blank"}

# Iniciación al servicio de transferencia de datos

El servicio de transferencia de datos de {{site.data.keyword.BluSoftlayer_full}} permite a los clientes enviar un dispositivo USB 2.0 o USB 3.0 compatible, CD y DVD a un centro de datos de {{site.data.keyword.BluSoftlayer}} para conectarlos directamente a su red para controlar de forma remota la transferencia de datos. El dispositivo está alojado en un bastidor dedicado ubicado en el centro de datos del cliente y montado como un destino iSCSI. Nuestro servicio de transferencia de datos es ideal cuando es necesario transferir grandes cantidades de datos sin utilizar nuestra red privada y es un servicio que se ofrece de forma gratuita para todos los clientes de {{site.data.keyword.BluSoftlayer}}.

## Acceso a la pantalla de servicio de transferencia de datos

**Nota**: actualmente, esta pantalla solo está disponible para el usuario maestro de la cuenta.

1. Acceda al [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} utilizando sus credenciales exclusivas.
2. Seleccione **Almacenamiento** > **Migración de datos** > **Transferencia de datos** desde la barra de navegación para acceder a la pantalla del servicio de transferencia de datos. <br/>

En la pantalla del **servicio de transferencia de datos**, los usuarios pueden enviar una solicitud de transferencia de datos, ver los detalles de una solicitud, ver el historial de incidencias asociadas con el seguimiento de una solicitud de dispositivo y cancelar una solicitud existente.

## Envío de una solicitud de transferencia de datos

Las solicitudes de transferencia de datos están diseñadas para permitir que las partes de nuestros centros de datos a las que corresponda sepan cuándo esperar un envío de un cliente. Las solicitudes se envían mediante el [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window}. Al crear una solicitud, tenga en cuenta las directrices siguientes:

- Asegúrese de que el dispositivo que desea enviar cumple con todos los [requisitos de hardware](/docs/infrastructure/DataTransferService/data-transfer-service-faq.html).
- Solo se puede asociar un dispositivo con una solicitud. Si desea enviar varios dispositivos, debe crear una solicitud nueva para cada dispositivo.
- Si hay que devolver el dispositivo, proporcione una etiqueta de envío prepagada y documentos de exportación según sea necesario en el paquete, de manera que el dispositivo pueda devolverse tras el periodo de transferencia.
- Si el envío es internacional, el usuario es el responsable de obtener todas las licencias, del envío y del despacho de aduanas para el dispositivo. Entre las responsabilidades del usuario se incluyen el pago de aranceles, impuestos y los costes de envío (si se aplica) a y desde el centro de datos de {{site.data.keyword.BluSoftlayer}}.
- Debe proporcionar el nombre del transportista y el número de seguimiento del envío a nuestro centro de datos al completar la solicitud.  Cree la etiqueta de envío con la dirección del centro de datos adecuada antes de enviar la solicitud de transferencia de datos.

Siga estos pasos para enviar una solicitud de transferencia de datos.

1. Acceda a la pantalla **Servicio de transferencia de datos** del [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window}. <br/> **Nota**: esta pantalla solo está disponible para el usuario maestro de la cuenta.
2. En la parte superior de la pantalla, pulse **Pedir solicitud de transferencia de datos**.
3. Rellene los campos del apartado **Información del dispositivo** según la tabla siguiente.
<table border="1">
<caption>La primera tabla lista los nombres de los campos del formulario de solicitud a la izquierda y la descripción a la derecha.</caption> 
 <tr><th>Nombre del campo</th><th>Instrucciones</th></tr>
 <tr><td>Tipo de dispositivo</td><td>El tipo de dispositivo que se envía al destino. Si el tipo de dispositivo no está en la lista, seleccione "Otros".</td></tr>
 <tr><td>Número de serie</td><td> El número de serie del dispositivo.</td></tr><tr><td>Descripción</td><td>Una breve descripción del dispositivo. Algunos de los detalles importantes que deben incluirse podrían ser identificar factores como el color y las etiquetas o pegatinas.</td></tr>
 <tr><td>Nota</td><td>Las notas adicionales sobre el dispositivo o la transferencia.</td></tr><tr><td>Destino</td><td>El centro de datos que recibirá el dispositivo.</td></tr>
 <tr><td>Transportista</td><td>Cartero o transportista exprés utilizado para enviar el dispositivo a su destino.</td></tr>
 <tr><td>Número de seguimiento</td><td>Número de seguimiento completo del envío.</td></tr>
 </table>

4. Rellene los campos del apartado **Dirección de retorno** o marque el recuadro de selección **Dirección de la empresa** para rellenar automáticamente los campos con la dirección de la empresa en el archivo. <br/> **Nota**: No olvide incluir la etiqueta de envío de devolución prepagada ni los documentos de exportación necesarios en el paquete para que podamos devolver el paquete.
5. Después de leer el acuerdo de servicio, seleccione el recuadro de selección **He leído y acepto el Acuerdo de servicio de transferencia de datos y el Acuerdo de servicio maestro**.
6. Pulse **Enviar solicitud de servicio**.

Después de enviar la solicitud, el estado de la incidencia de la solicitud aparecerá como *Enviado a SoftLayer*. Infórmenos si un envío de importación o exportación requiere una licencia de un gobierno local y adjunte la información de licencia en la incidencia.

Una vez que se recibe el dispositivo, el estado se actualiza a *Recibido por SoftLayer* y se actualiza de nuevo a *Conectado* después de que un técnico de un centro de datos conecte el dispositivo a la red. 

El período de transferencia de datos inicial no debería durar más de dos semanas. Durante este tiempo, solo se permite que el administrador de la cuenta acceda al dispositivo. Si necesita más tiempo, puede solicitar una prórroga. Además, si desea que el dispositivo se envíe antes de dos semanas, puede solicitar la devolución. Debe enviar una notificación a {{site.data.keyword.IBM}} mediante [{{site.data.keyword.slportal}}](https://control.softlayer.com/) una vez que se complete la transferencia. A continuación, desconectaremos el dispositivo y lo devolveremos o destruiremos, según lo que haya solicitado.


## Acceso a la pantalla de envíos

La pantalla Envíos de [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} muestra todos los envíos asociados con las solicitudes de servicio de transferencia de datos. Desde esta pantalla, puede visualizar los envíos y confirmar los envíos de devolución una vez que se reciben. 

Para acceder a la pantalla de envíos:

1. Acceda al [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} utilizando sus credenciales exclusivas.
2. Seleccione **Cuenta** > **Gestionar** > **Envíos** en la barra de navegación.

En la pantalla de envíos, todas las solicitudes de envío dentro de los últimos 30 días se muestran en la lista de envíos junto con los detalles. Los envíos pueden [ordenarse o filtrarse](sort-or-filter-shipments-list.html) por estado, edad o detalles de envío concretos. Además, puede confirmar el acuse de recibo de envíos de devolución en esta pantalla. ![Pantalla de envíos](/images/DTSShipmentScreen1.png)
