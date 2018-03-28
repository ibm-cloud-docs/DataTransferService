---

copyright:
  years: 2017
lastupdated: "2017-11-13"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Conexión al dispositivo DTS en Windows con software iSCSI

Para interactuar con un LUN iSCSI en Windows, los usuarios deben conectarse al LUN mediante el iniciador de software, la herramienta iSCSI propiedad de Microsoft.  Para los usuarios que ejecuten Windows Server 2008 o Windows Vista y versiones superiores, el iniciador de software iSCSI está integrado en el sistema operativo.  Los usuarios que ejecuten Windows Server 2003, Windows XP y Windows 2000 deben descargar el iniciador antes de completar este procedimiento.  Siga los pasos siguientes para conectar con un LUN iSCSI en Windows con un iniciador de software iSCSI.

## Conectar a un LUN iSCSI

1. Recupere **el nombre de usuario iSCSI, la contraseña y la dirección de almacenamiento** para el iSCSI que se esté conectando desde el portal del cliente.  Consulte Acceso a la pantalla de transferencia de datos.
2. Inicie el iniciador iSCSI.
3. Actualice el nombre del iniciador en el separador **Configuración** para los datos IQN del portal de SoftLayer.
4. Haga clic en el separador **Descubrimiento**.
5. Pulse el botón **Añadir** en el apartado **Portales de destino** de la pantalla.
6. Especifique la **dirección IP iSCSI** en el campo **Dirección IP o nombre de DNS**.
7. Pulse el separador **Avanzado**.
8. Actualice la información de inicio de sesión iSCSI.
   - Seleccione el recuadro de selección **información de inicio de sesión CHAP** para habilitar el inicio de sesión CHAP.
   - Especifique el **Nombre de usuario iSCSI** en el campo **Nombre de usuario**.
   - Especifique la **Contraseña iSCSI** en el campo **Secreto de destino**.
   - Pulse el botón **Aceptar** dos veces.
9. Pulse el separador **Destinos**.
10. Seleccione el iSCSI recién añadido de la lista **Destinos**.
11. Pulse el botón **Iniciar sesión**. Aparecerá el menú emergente **Iniciar sesión en destino**.
12. Seleccione el recuadro de selección **Restaurar automáticamente la conexión cuando se reinicie el sistema** para que la conexión se mantenga entre reinicios.
13. Pulse el botón **Avanzado**.
14. Actualice la información de inicio de sesión iSCSI.
    - Seleccione el recuadro de selección **información de inicio de sesión CHAP** para habilitar el inicio de sesión CHAP.
    - Especifique el **Nombre de usuario iSCSI** en el campo **Nombre de usuario**.
    - Especifique la **Contraseña iSCSI** en el campo **Secreto de destino**.
    - Pulse el botón **Aceptar** dos veces.
15. Verifique que el destino iSCSI nuevo se muestre como Conectado en el separador Destinos.

<table>
<tbody>
<tr>
<th>Si el destino iSCSI...</th><th>Entonces...</th></tr>
<tr><td>Aparece como Conectado</td><td>Pulse el botón <strong>Aceptar</strong>. El LUN iSCSI está conectado.</td></tr>
<tr><td>No aparece como Conectado</td><td>Repita los pasos anteriores para restablecer la conexión.</td></tr></tbody></table>
