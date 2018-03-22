---

copyright:
  years: 2017
lastupdated: "2017-11-13"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Conectando-se ao dispositivo DTS no Windows com o Inicializador de software iSCSI

Para interagir com um LUN iSCSI no Windows, os usuários devem se conectar ao LUN usando o Inicializador de software iSCSI, ferramenta iSCSI de propriedade da Microsoft. Para usuários que executam o Windows Server 2008 ou o Windows Vista e acima, o Inicializador de software iSCSI é construído no sistema operacional. Os usuários que executam o Windows Server 2003, o Windows XP e o Windows 2000 devem fazer download do Inicializador antes de concluir esse procedimento. Siga as etapas abaixo para se conectar a um LUN iSCSI no Windows com o Inicializador de software iSCSI.

## Conecte-se a um LUN iSCSI

1. Recupere o **Nome do usuário, a senha e o endereço de armazenamento do iSCSI** para o iSCSI que está sendo conectado do Portal do cliente. Consulte a tela Acessar a transferência de dados.
2. Ative o Inicializador iSCSI.
3. Atualize o nome do inicializador na guia **Configuração** para os dados do IQN no portal do SoftLayer.
4. Clique na guia **Descoberta**.
5. Clique no botão **Incluir** na seção **Portais de destino** da tela.
6. Insira o **Endereço IP do iSCSI** no campo **Endereço IP ou nome do DNS**.
7. Clique na guia **Avançado**.
8. Atualize as informações de logon de iSCSI.
   - Marque a caixa de seleção **Informações de logon do CHAP** para permitir o logon do CHAP.
   - Insira o **Nome de usuário do iSCSI** no campo **Nome do usuário**.
   - Insira a **Senha do iSCSI** no campo **Segredo de destino**.
   - Clique no botão de **OK** duas vezes.
9. Clique na guia **Destinos**.
10. Selecione o iSCSI recém-incluído na lista **Destinos**.
11. Clique no botão **Logon**. O menu pop-up **Efetuar logon no destino** aparecerá.
12. Marque a caixa de seleção **Restaurar automaticamente essa conexão quando o sistema for inicializado** para configurar a conexão para que persista entre as reinicializações.
13. Clique no botão **Avançado**.
14. Atualize as informações de logon de iSCSI.
    - Marque a caixa de seleção **Informações de logon do CHAP** para permitir o logon do CHAP.
    - Insira o **Nome de usuário do iSCSI** no campo **Nome do usuário**.
    - Insira a **Senha do iSCSI** no campo **Segredo de destino**.
    - Clique no botão de **OK** duas vezes.
15. Verifique se o novo destino iscsi é exibido como Conectado na guia Destinos.

<table>
<tbody>
<tr>
<th>Se o destino iscsi…</th><th>Então...</th></tr>
<tr><td>For exibido como Conectado</td><td>Clique no botão de <strong>OK</strong>. Seu LUN iSCSI está conectado agora.</td></tr>
<tr><td>Não for exibido como Conectado</td><td>Repita as etapas acima para reconfigurar a conexão.</td></tr></tbody></table>
