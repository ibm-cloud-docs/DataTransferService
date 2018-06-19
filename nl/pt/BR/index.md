---

copyright:
  years: 1994, 2018
lastupdated: "2018-05-22"

---
{:new_window: target="_blank"}

# Introdução ao serviço de transferência de dados

O serviço de transferência de dados do {{site.data.keyword.BluSoftlayer_full}} permite que os clientes enviem um dispositivo compatível com USB 2.0 ou USB 3.0, CDs e DVDs para um data center do {{site.data.keyword.BluSoftlayer}} para serem conectados diretamente às suas redes para controlar remotamente a transferência de dados. O dispositivo é hospedado em um rack dedicado localizado no data center dos clientes e montado como um destino iSCSI. Nosso serviço de transferência de dados é ideal quando você precisa transferir grandes quantias de dados sem usar a nossa rede privada e é um serviço oferecido gratuitamente para todos os clientes do {{site.data.keyword.BluSoftlayer}}.

## Acessando a tela do serviço de transferência de dados

**Nota**: essa tela está disponível atualmente apenas para o usuário principal da conta.

1. Acesse o [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} usando suas credenciais exclusivas.
2. Selecione **Armazenamento** > **Migração de dados** > **Transferência de dados** na Barra de navegação para acessar a tela Data Transfer Service. <br/>

Na tela **Serviço de transferência de dados**, os usuários podem enviar uma solicitação de transferência de dados, visualizar detalhes sobre uma solicitação, visualizar o histórico de chamado associado ao rastreamento de dispositivo para uma solicitação e cancelar uma solicitação existente.

## Enviando uma solicitação de transferência de dados

As solicitações de transferência de dados foram projetadas para permitir que as partes apropriadas em nossos data centers saibam esperar uma remessa de um cliente. As solicitações são enviadas por meio do [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window}. Ao criar uma solicitação, lembre-se das diretrizes a seguir:

- Assegure-se de que o dispositivo que você deseja enviar atenda todos os [requisitos de hardware](/docs/infrastructure/DataTransferService/data-transfer-service-faq.html).
- Somente um dispositivo pode ser associado a uma solicitação. Se você deseja enviar múltiplos dispositivos, deve-se criar uma nova solicitação para cada dispositivo.
- Se o dispositivo precisa ser retornado, forneça uma etiqueta de remessa pré-paga e documentos de exportação, conforme necessário, no pacote para que o dispositivo possa ser retornado após o período de transferência.
- Se o envio for internacional, você será responsável por obter todo o licenciamento, envio e liberação da alfândega para o Dispositivo. Suas responsabilidades incluem o pagamento de taxas, impostos e custos de frete para/de (se aplicável) o data center do {{site.data.keyword.BluSoftlayer}}.
- É necessário fornecer o nome da transportadora e o número de rastreamento da remessa para o nosso data center ao concluir a solicitação.  Crie a etiqueta de remessa com o endereço do data center apropriado antes de enviar a solicitação de transferência de dados.

Siga as etapas abaixo para enviar uma solicitação de transferência de dados.

1. Acesse a tela **Data Transfer Service** no [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window}. <br/> **Nota**: essa tela está disponível apenas para o usuário principal da conta.
2. Na parte superior da tela, clique em **Pedir solicitação de transferência de dados**.
3. Preencha cada campo na seção **Informações sobre o dispositivo** de acordo com a tabela abaixo.
<table border="1">
<caption>A Tabela 1 lista os nomes dos campos no formulário de solicitação à esquerda e suas descrições à direita.</caption> 
 <tr><th>Nome de Campo</th><th>Instruções</th></tr>
 <tr><td>Tipo de dispositivo</td><td>O tipo de dispositivo que está sendo enviado para o destino. Se o tipo de dispositivo não estiver listado, selecione "Outro".</td></tr>
 <tr><td>Número de série</td><td> O número de série do dispositivo.</td></tr><tr><td>Descrição</td><td>Uma breve descrição do dispositivo. Detalhes importantes a serem incluídos podem ser fatores de identificação, como cor, etiquetas ou adesivos.</td></tr>
 <tr><td>Nota</td><td>Quaisquer notas adicionais sobre o dispositivo ou a transferência.</td></tr><tr><td>Destino</td><td>O data center que receberá o dispositivo.</td></tr>
 <tr><td>Transportadora</td><td>A transportadora postal ou expressa que é usada para enviar o dispositivo para seu destino.</td></tr>
 <tr><td>Número de rastreamento</td><td>Número de rastreamento completo para a remessa.</td></tr>
 </table>

4. Preencha cada campo na seção **Endereço de retorno** ou marque a caixa de seleção **Endereço da empresa** para preencher automaticamente os campos com o endereço da empresa no arquivo. <br/> **Nota**: lembre-se de incluir a etiqueta de envio de retorno pré-pago e quaisquer documentos de exportação necessários no pacote para que o dispositivo possa ser retornado.
5. Depois de ler o contrato de prestação de serviços, marque a caixa de seleção **Li e concordo com o Contrato de Prestação de Serviços de Transferência de Dados e o Contrato de Prestação de Serviços Principal**.
6. Clique em **Enviar solicitação de serviço**.

Depois de enviar a solicitação, o status para o chamado de solicitação aparecerá como *Enviado para a SoftLayer*. Se alguma remessa de importação ou exportação requer uma licença de seu governo local, notifique-nos e anexe as informações sobre licença no chamado.

Depois que o dispositivo for recebido, o status será atualizado para *Recebido pela SoftLayer* e atualizado novamente para *Conectado* depois que um técnico do data center conectar o dispositivo à rede. 

O período de transferência de dados inicial deve durar no máximo duas semanas. Durante esse tempo, o acesso ao dispositivo é permitido apenas ao administrador de conta. Se você precisar de mais tempo, será possível solicitar uma extensão. Além disso, se você desejar que o dispositivo seja enviado antes de duas semanas, será possível solicitar o retorno. Deve-se notificar a {{site.data.keyword.IBM}} por meio do [{{site.data.keyword.slportal}}](https://control.softlayer.com/) quando a transferência está completa. Vamos então remover o Dispositivo e retorná-lo ou destruí-lo, dependendo do que você solicitou.


## Acessando a tela Remessas

A tela Remessas dentro do [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} exibe todas as remessas associadas a solicitações do serviço de transferência de dados. Nessa tela, é possível visualizar remessas e confirmar remessas de retorno após o recebimento. 

Para acessar a tela Remessas:

1. Acesse o [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} usando suas credenciais exclusivas.
2. Selecione **Conta** > **Gerenciar** > **Remessas** na Barra de Navegação.

Na tela Remessas, todas as solicitações de envio dos últimos 30 dias são exibidas na lista de remessas com seus detalhes. As remessas podem ser [classificadas ou filtradas](sort-or-filter-shipments-list.html) por status, idade ou detalhes específicos da remessa. Além disso, é possível confirmar o recebimento de remessas de retorno nessa tela.
![Tela Remessas](/images/DTSShipmentScreen1.png)
