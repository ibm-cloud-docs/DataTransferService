---

copyright:
  years: 2017, 2018
lastupdated: "2018-05-22"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Conectando-se ao dispositivo DTS no Windows com o Inicializador de software iSCSI

Para interagir com uma LUN iSCSI no Windows, os usuários devem se conectar ao armazenamento usando o Inicializador de software iSCSI, ferramenta iSCSI de propriedade da Microsoft. Para usuários do Windows Server 2008 ou Windows Vista e acima, o Inicializador de software iSCSI é construído no sistema operacional. Os usuários do Windows Server 2003, Windows XP e Windows 2000 devem fazer download do Inicializador antes de iniciar este procedimento.

## Conecte-se a um LUN iSCSI

1. No {{site.data.keyword.slportal}}, recupere o **Nome do usuário, senha e endereço de armazenamento do iSCSI** para o dispositivo de armazenamento que você deseja conectar.
2. Inicie o Inicializador iSCSI.
3. Na guia **Configuração**, atualize o nome do inicializador para os dados do IQN no {{site.data.keyword.slportal}}.
4. Clique em **Descoberta**.
5. Na seção **Portais de destino**, clique em **Incluir**.
6. No campo **Endereço IP ou nome do DNS**, insira o **Endereço IP do iSCSI**.
7. Clique em **Avançado**.
8. Atualize as informações de logon de iSCSI.
   - Marque a caixa de seleção **Informações de logon do CHAP** para permitir o logon do CHAP.
   - Insira o nome do usuário do iSCSI no campo **Nome do usuário**.
   - Digite a senha do iSCSI no campo **Segredo de destino**.
   - Clique em **OK** duas vezes.
9. Clique em **Destinos**
10. Selecione o iSCSI recém-incluído na lista **Destinos**.
11. Clique em **Efetuar logon**. A janela **Efetuar logon no destino** aparece.
12. Marque a caixa de seleção **Restaurar automaticamente esta conexão quando o sistema for inicializado** para configurar a conexão para que persista entre as reinicializações.
13. Clique em **Avançado**.
14. Atualize as informações de logon de iSCSI.
    - Marque a caixa de seleção **Informações de logon do CHAP** para permitir o logon do CHAP.
    - Insira o nome do usuário do iSCSI no campo **Nome do usuário**.
    - Digite a senha do iSCSI no campo **Segredo de destino**.
    - Clique em **OK** duas vezes.
15. Verifique se o novo destino iscsi é exibido como Conectado na guia Destinos.
    - Se o seu destino iSCSI for exibido como **Conectado**, clique em **OK**. Seu LUN iSCSI está agora conectado
    - Se o seu destino iSCSI não for exibido como **Conectado**, repita todas as etapas anteriores para reconfigurar a conexão.
