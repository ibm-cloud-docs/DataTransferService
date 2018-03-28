---

copyright:
  years: 2017
lastupdated: "2017-12-18"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# ¿Qué es un servicio de transferencia de datos multimedia?
 
El servicio de transferencia de datos es un servicio que permite enviar dispositivos compatibles con USB 2.0 o 3.0 y/o CD y DVD a un centro de datos de {{site.data.keyword.BluSoftlayer_full}} que se vaya a conectar directamente a su red. El dispositivo está alojado en un bastidor dedicado ubicado en el centro de datos elegido y se montará como destino iSCSI. También se admiten unidades de formato avanzado.

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
      **Nota**: 25 $ por semana en caso de prórroga
3.    Coste del envío al centro de datos de {{site.data.keyword.IBM}} y desde él, incluidos el pago de aranceles e impuestos.

**Nota**: el cliente es responsable de:  
- asegurarse de que no se requiera ninguna licencia de importación o exportación para enviar el dispositivo al centro de datos de {{site.data.keyword.IBM}} o devolverlo al cliente (si procede); 
- asegurarse de que ni el cliente ni ningún usuario final del cliente cuyos datos se incluyen en el contenido estén sujetos a ninguna orden del gobierno de los Estados Unidos que revoque o deniegue sus privilegios de exportación estadounidenses. El Cliente acepta notificar a {{site.data.keyword.IBM}} inmediatamente si el Cliente o cualquier usuario final queda sujeto a una orden de este tipo;  
- obtener todas las licencias, del envío y del despacho de aduanas para el dispositivo, incluidos el pago de aranceles, impuestos y gastos de envío al centro de datos de {{site.data.keyword.IBM}} y desde este (si es aplicable);   
- cumplir con todas las leyes aplicables, incluidas la de privacidad, importación y exportación, asociadas con la entrega y la devolución del dispositivo, y la transferencia de contenido al centro de datos de {{site.data.keyword.IBM}}; y 
- disponer los acuerdos adecuados en su lugar y obtener todos los permisos necesarios con el usuario final del cliente para cualquier dato de usuario final que el cliente transfiera al hardware.

## Realizar una solicitud
Esto se realiza en **Almacenamiento** > **Migración de datos** > **Transferencia de datos**, pulsando el enlace **Pedir solicitud de transferencia de datos** de la parte superior derecha de la página.

![Realización de una solicitud de transferencia de datos](/images/DTS.png)
 

Rellene este formulario con los dispositivos
1. Número de serie
2. Tipo
3. Descripción breve del dispositivo
4. El centro de datos al que desea que vaya el dispositivo
5. Número para realizar el seguimiento del envío
6. Servicio de transportista utilizado
7. Dirección de devolución donde desea que se envíe el dispositivo cuando haya terminado.

Una vez cumplimentados esos datos, se creará automáticamente una incidencia de soporte para avisar a nuestros técnicos de que se nos está enviando el dispositivo y permitirles que realicen el seguimiento de la entrega.  Una vez que recibamos el dispositivo, procederemos a conectarlo a nuestro bastidor dedicado.  Una vez que hayamos conectado el dispositivo, la incidencia se actualizará y se le proporcionará un enlace a sus credenciales de registro al destino iSCSI.

## Solicitar una devolución
Si proporcionó una dirección de devolución e incluyó la etiqueta de envío en el paquete, puede solicitar que se le devuelve el dispositivo en cualquier momento durante las dos semanas de la transferencia. Para ello, en [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} seleccione **Almacenamiento** > **Migración de datos** > **Transferencia de datos** y en el menú desplegable **Acción** de su dispositivo, seleccione **solicitar devolución**. Esto avisará a nuestros técnicos que desea que se desconecte el dispositivo y le sea enviado.

## Solicitar prórroga
Después del período de dos semanas gratuito, si todavía necesita utilizar su dispositivo USB, debe solicitar una prórroga para avisar a nuestros técnicos que desea ampliar el tiempo que el dispositivo está conectado.  Esto se hace de la misma manera que pediría una devolución de su dispositivo: debe seleccionar **Almacenamiento** > **Migración de datos** > **Transferencia de datos ** y, en el menú desplegable **Acción** del dispositivo, seleccionar **Solicitud de prórroga**.  Tras las dos primeras semanas, cada semana tiene una tarifa de servicio de 25 dólares.  Además, según el espacio disponible en el centro datos de su dispositivo, su solicitud podría ser denegada.  Si se le concede la solicitud, la incidencia se actualizará e indicará que se le ha concedido una semana adicional.

## Desconectar
Tras el período de dos semanas, el dispositivo se desconectará automáticamente desde nuestro centro de datos y le será devuelto mediante el transportista elegido a la dirección de devolución especificada en la solicitud inicial. La incidencia se actualizará e indicará que el dispositivo se ha desconectado. Si no ha solicitado la devolución del dispositivo, este se destruirá in situ.
