---

copyright:
  years: 2017, 2018
lastupdated: "2018-05-22"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# ¿Qué es un servicio de transferencia de datos multimedia?
 
El servicio de transferencia de datos es un servicio que permite enviar dispositivos compatibles con USB 2.0 o 3.0, CD y DVD a un centro de datos de {{site.data.keyword.BluSoftlayer_full}} que se vaya a conectar directamente a su red. El dispositivo está alojado en un bastidor dedicado y montado como un destino iSCSI. También se admiten unidades de formato avanzado.

## Requisitos de hardware
1.    El dispositivo debe tener una fuente de alimentación que sea compatible con 208v/220v
2.    El dispositivo debe tener un conector que se ajuste al enchufe estándar de 120v (NEMA 5-15P)
3.    El dispositivo debe ser compatible con USB 2.0 (ahora también se admite 3.0)
4.    El dispositivo debe incluir un cable USB con un conector USB A macho (conector USB estándar que se ajusta a la mayoría de los sistemas)
5.    CD/DVD
      1.    Deben estar en estuches para CD, fundas, cajas o en algún tipo de contenedor y preferiblemente todos juntos (un estuche para varios CD, por ejemplo) y cada disco debe ser la etiqueta exclusiva.
      2.    Los discos se girarán según la solicitud del cliente mediante la incidencia

## Coste
1.    Solicitud inicial de servicio: 0 $
2.    Primeras dos semanas de transferencia de datos: 0 $
      **Nota**: 25 $ por semana en caso de prórroga.
3.    Coste del envío al centro de datos de {{site.data.keyword.IBM}} y desde él, incluidos el pago de aranceles e impuestos.

**Nota**: el cliente es responsable de:  
- asegurarse de que no se requiera ninguna licencia de importación o exportación para enviar el dispositivo al centro de datos de {{site.data.keyword.IBM}} o devolverlo al cliente (si procede); 
- asegurarse de que el cliente o cualquier usuario cliente cuyos datos se incluyen en el contenido no estén sujetos a ninguna orden del gobierno de los Estados Unidos que revoque o deniegue sus privilegios de exportación estadounidenses. Notifique a {{site.data.keyword.IBM}} inmediatamente si el Cliente o cualquier usuario queda sujeto a una orden de este tipo;  
- obtener todas las licencias, envíos y despachos de aduanas del dispositivo. Entre las responsabilidades del cliente se incluyen el pago de aranceles, impuestos y los costes de envío (si se aplica) a y desde el centro de datos de {{site.data.keyword.IBM}};   
- cumplir con todas las leyes aplicables asociadas con la entrega y la devolución del dispositivo, y la transferencia de contenido al centro de datos de {{site.data.keyword.IBM}}. Esto incluye las leyes de privacidad, importación y exportación.
- disponer los acuerdos adecuados en su lugar y obtener todos los permisos necesarios del usuario del cliente para cualquier dato de usuario que el cliente desee transferir al hardware.

## Realizar una solicitud
Esto se realiza en **Almacenamiento** > **Migración de datos** > **Transferencia de datos**, pulsando **Pedir solicitud de transferencia de datos** de la esquina superior derecha de la página.

![Realización de una solicitud de transferencia de datos](/images/DTS.png)

Complete el formulario con los siguientes datos del dispositivo
1. Número de serie
2. Tipo
3. Descripción breve del dispositivo
4. El centro de datos al que desea que vaya el dispositivo
5. Número para realizar el seguimiento del envío
6. Servicio de transportista utilizado
7. Dirección de devolución donde desea que se envíe el dispositivo cuando haya terminado.

La solicitud crea una incidencia de soporte para avisar a nuestros técnicos de que se nos está enviando el dispositivo y permitirles que realicen el seguimiento de la entrega. Una vez que recibamos el dispositivo, lo conectaremos a nuestro bastidor dedicado. Después de conectar el dispositivo, la incidencia se actualiza para proporcionarle un enlace a las credenciales de inicio de sesión del destino iSCSI.

## Solicitar una devolución
Si proporcionó una dirección de devolución e incluyó la etiqueta de envío en el paquete, puede solicitar que se le devuelva el dispositivo en cualquier momento durante las dos semanas de la transferencia. Puede hacerlo mediante el [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window}. Seleccione **Almacenamiento** > **Migración de datos** > **Transferencia de datos** y en el menú **Acción** de su dispositivo, seleccione **solicitar devolución**. Esto avisará a nuestros técnicos que desea que se desconecte el dispositivo y le sea enviado.

## Solicitar prórroga
Después del período de dos semanas gratuito, si todavía necesita utilizar su dispositivo, debe solicitar una prórroga. Esto avisará a nuestros técnicos que desea ampliar el tiempo en que el dispositivo está conectado. Puede hacerlo de la misma forma que solicita que le devuelvan el dispositivo. Seleccione **Almacenamiento** > **Migración de datos** > **Transferencia de datos** y en el menú **Acción** del dispositivo, seleccione **solicitar prórroga**. Cada semana adicional genera una tarifa de servicio de 25 $. Tenga en cuenta que su solicitud de prórroga puede ser denegada en función del espacio disponible en el centro de datos. Cuando se otorga la solicitud, la incidencia se actualiza en consecuencia.

## Desconectar
Tras un período de dos semanas, el dispositivo se desconecta automáticamente de nuestro centro de datos. Si ha solicitado una devolución, el dispositivo le será devuelto mediante el transportista elegido a la dirección de devolución especificada en la solicitud inicial. La incidencia se actualizará e indicará que se ha desconectado el servicio. Si no ha solicitado la devolución del servicio, este se destruirá in situ.
