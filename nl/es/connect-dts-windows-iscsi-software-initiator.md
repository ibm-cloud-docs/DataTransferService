---

copyright:
  years: 2017, 2019
lastupdated: "2019-02-05"

---


# Conexión al dispositivo DTS en Windows con software iSCSI
{: #mountingDTSWindows}

Para interactuar con un LUN iSCSI en Windows, los usuarios deben conectarse al almacenamiento mediante el iniciador de software iSCSI, una herramienta iSCSI propiedad de Microsoft. Para los usuarios de Windows Server 2008 o Windows Vista y versiones posteriores, el iniciador de software iSCSI está integrado en el sistema operativo. Los usuarios de Windows Server 2003, Windows XP y Windows 2000 deben descargar el iniciador antes de iniciar este procedimiento.

## Conexión a un LUN iSCSI

1. Desde {{site.data.keyword.slportal}}, recupere **la dirección de almacenamiento, la contraseña y el nombre de usuario de iSCSI** del dispositivo de almacenamiento que desea conectar.
2. Inicie el iniciador de iSCSI.
3. En el separador **Configuración**, actualice el nombre del iniciador para los datos IQN de {{site.data.keyword.slportal}}.
4. Pulse **Descubrimiento**.
5. En la sección **Portales de destino**, pulse **Añadir**.
6. En el campo **Dirección IP o nombre de DNS**, especifique la **dirección IP iSCSI**.
7. Pulse **Avanzado**.
8. Actualice la información de inicio de sesión iSCSI.
   - Seleccione el recuadro de selección **información de inicio de sesión CHAP** para habilitar el inicio de sesión CHAP.
   - Especifique el nombre de usuario iSCSI en el campo **nombre de usuario**.
   - Especifique la contraseña iSCSI en el campo **secreto de destino**.
   - Pulse **Aceptar** dos veces.
9. Pulse **Destinos**
10. Seleccione el iSCSI recién añadido de la lista **Destinos**.
11. Pulse **Iniciar sesión**. Aparecerá la ventana **Iniciar sesión en destino**.
12. Seleccione **Restaurar automáticamente la conexión al arrancar el sistema** para que la conexión se mantenga entre reinicios.
13. Pulse **Avanzado**.
14. Actualice la información de inicio de sesión iSCSI.
    - Seleccione el recuadro de selección **información de inicio de sesión CHAP** para habilitar el inicio de sesión CHAP.
    - Especifique el nombre de usuario iSCSI en el campo **nombre de usuario**.
    - Especifique la contraseña iSCSI en el campo **secreto de destino**.
    - Pulse **Aceptar** dos veces.
15. Verifique que el destino iSCSI nuevo se muestre como Conectado en el separador Destinos.
    - Si su destino iSCSI se muestra como **Conectado**, pulse **Aceptar**. El LUN iSCSI está conectado
    - Si su destino iSCSI no se muestra como **Conectado**, repita todos los pasos anteriores para reiniciar la conexión.
