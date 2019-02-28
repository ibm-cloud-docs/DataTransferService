---

copyright:
  years: 2017, 2019
lastupdated: "2019-02-05"

---
{:new_window: target="_blank"}

# Introdução ao serviço de transferência de dados
{: #gettingstarted}

Os clientes podem usar o serviço de transferência de dados do {{site.data.keyword.BluSoftlayer_full}} para enviar um
dispositivo compatível com USB 2.0 ou USB 3.0, CDs e DVDs para um data center do {{site.data.keyword.BluSoftlayer}}. O
dispositivo dos clientes é conectado diretamente à rede deles para que possam controlar remotamente a transferência de dados. O
dispositivo é hospedado em um rack dedicado localizado no data center dos clientes e montado como um destino iSCSI. O serviço de
transferência de dados é ideal quando grandes quantias de dados precisam ser transferidas sem o uso da rede privada do
{{site.data.keyword.BluSoftlayer}}. Esse é um serviço oferecido gratuitamente a todos os clientes do {{site.data.keyword.BluSoftlayer}}.

## Acessando a tela do serviço de transferência de dados

**Nota**: essa tela está disponível apenas para o usuário principal da conta.

1. Acesse o [{{site.data.keyword.slportal}} ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/){:new_window} com suas credenciais exclusivas.
2. Selecione **Armazenamento** > **Migração de dados** > **Transferência de dados** na Barra de navegação para acessar a tela Data Transfer Service. <br/>

Na tela **Serviço de transferência de dados**, os usuários podem enviar uma solicitação de
transferência de dados, visualizar os detalhes de uma solicitação, visualizar o histórico do chamado associado ao rastreamento
do dispositivo e cancelar uma solicitação existente.

## Enviando uma solicitação de transferência de dados

As solicitações de transferência de dados foram projetadas para permitir que as partes apropriadas em nossos data centers saibam esperar uma remessa de um cliente. As solicitações são submetidas por meio do [{{site.data.keyword.slportal}} ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/){:new_window}.

Ao criar uma solicitação, lembre-se das diretrizes a seguir.

- Assegure-se de que o dispositivo que você deseja enviar atenda todos os [requisitos de hardware](/docs/infrastructure/DataTransferService/data-transfer-service-faq.html).
- Somente um dispositivo pode ser associado a uma solicitação. Se você deseja enviar múltiplos dispositivos, deve-se criar uma nova solicitação para cada dispositivo.
- Se o dispositivo precisa ser retornado, forneça uma etiqueta de remessa pré-paga e documentos de exportação, conforme necessário, no pacote para que o dispositivo possa ser retornado após o período de transferência.
- Se estiver enviando o dispositivo internacionalmente, você será responsável por obter todo o licenciamento, a remessa e
a liberação da alfândega para o dispositivo. Suas responsabilidades incluem o pagamento de taxas, impostos e custos de frete para/de (se aplicável) o data center do {{site.data.keyword.BluSoftlayer}}.
- Ao preencher a solicitação, é necessário fornecer o nome da transportadora e o número de rastreamento da remessa para o data
center.  Crie a etiqueta de remessa com o endereço do data center apropriado antes de enviar a solicitação de transferência de dados.

Siga estas etapas para enviar uma solicitação de transferência de dados.

1. Acesse a tela **Serviço de transferência de dados** no [{{site.data.keyword.slportal}} ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/){:new_window}.
2. Clique em  ** Pedir solicitação de transferência de dados **.
3. Preencha cada campo na seção **Informações do dispositivo** de acordo com a tabela 1.
<table border="1">
<caption>A Tabela 1 lista os nomes dos campos no formulário de solicitação à esquerda e a sua descrição à direita.</caption>
 <tr><th>Nome de Campo</th><th>Instruções</th></tr>
 <tr><td>Tipo de dispositivo</td><td>O tipo de dispositivo que é enviado para o destino. Se o tipo de dispositivo não estiver listado, selecione "Outro".</td></tr>
 <tr><td>Número de série</td><td> O número de série do dispositivo.</td></tr><tr><td>Descrição</td><td>Uma breve descrição do dispositivo. Os detalhes importantes a serem incluídos podem ser os fatores de identificação, como a cor, os rótulos ou os adesivos.</td></tr>
 <tr><td>Nota</td><td>Quaisquer observações adicionais sobre o dispositivo ou a transferência.</td></tr><tr><td>Destino</td><td>O
data center que receberá o dispositivo.</td></tr>
 <tr><td>Transportadora</td><td>A transportadora postal ou expressa que é usada para enviar o dispositivo para seu destino.</td></tr>
 <tr><td>Número de rastreamento</td><td>Número de rastreamento completo para a remessa.</td></tr>
 </table>

4. Preencha cada campo na seção **Endereço de retorno** ou marque a caixa de seleção **Endereço da empresa** para preencher automaticamente os campos com o endereço da empresa no arquivo. <br/> **Nota**: lembre-se de incluir o rótulo de retorno pré-pago e quaisquer documentos de
exportação necessários no pacote.
5. Depois de ler o contrato de prestação de serviços, marque a caixa de seleção **Li e concordo com o Contrato de Prestação de Serviços de Transferência de Dados e o Contrato de Prestação de Serviços Principal**.
6. Clique em **Enviar solicitação de serviço**.

Após o envio da solicitação, o status do chamado da solicitação aparecerá como `Sent to SoftLayer`. Se alguma remessa de importação ou de exportação requerer uma licença de seu governo local, notifique o
{{site.data.keyword.BluSoftlayer}} e anexe as informações sobre licença no chamado.

Depois do recebimento do dispositivo, o status é atualizado para `Received by SoftLayer`. O status do
chamado é atualizado novamente para `Connected` após um técnico do data center conectar o dispositivo à rede.

O período de transferência de dados iniciais é de duas semanas. Durante esse tempo, o acesso ao dispositivo é concedido apenas
ao administrador da conta. Se você precisar de mais tempo, será possível solicitar uma extensão. Além disso, se você desejar que o
dispositivo seja enviado de volta antes de duas semanas, será possível solicitar o retorno. Deve-se notificar a {{site.data.keyword.IBM}} por meio do [{{site.data.keyword.slportal}}](https://control.softlayer.com/) quando a transferência está completa. Em seguida, o {{site.data.keyword.BluSoftlayer}} removerá o dispositivo e o retornará ou o destruirá dependendo da sua
solicitação.


## Acessando a tela Remessas

A tela Remessas dentro do [{{site.data.keyword.slportal}} ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/){:new_window} exibe todas as remessas que estão associadas a solicitações de serviço de transferência de dados. Nessa tela, é possível visualizar remessas e confirmar remessas de retorno após o recebimento.

Para acessar a tela Remessas:

1. Acesse o [{{site.data.keyword.slportal}} ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/){:new_window} usando suas credenciais exclusivas.
2. Selecione **Conta** > **Gerenciar** > **Remessas** na Barra de Navegação.

Na tela Remessas, todas as solicitações de remessa dos últimos 30 dias são exibidas com detalhes. As remessas podem
ser [classificadas ou filtradas](sort-or-filter-shipments-list.html) por status, por idade ou por detalhes
específicos da remessa. Além disso, é possível confirmar o recebimento de remessas de retorno nessa tela.
![Tela Remessas](/images/DTSShipmentScreen1.png)
