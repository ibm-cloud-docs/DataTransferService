---

copyright:
  years: 1994, 2017
lastupdated: "2017-12-18"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Introdução ao Data Transfer Service

O Data Transfer Service do {{site.data.keyword.BluSoftlayer_full}} permite que os clientes enviem um dispositivo compatível com USB 2.0 ou USB 3.0 e/ou CDs e DVDs para um data center do {{site.data.keyword.BluSoftlayer}} para serem conectados diretamente à rede deles para controlar remotamente a transferência de dados. O dispositivo é hospedado em um rack dedicado localizado no data center dos clientes e será montado como um destino iSCSI. Nosso Data Transfer Service é ideal quando você precisa transferir grandes quantias de dados sem usar a nossa Rede privada e é um serviço oferecido gratuitamente para todos os clientes {{site.data.keyword.BluSoftlayer}}.

## Acessando a tela do Data Transfer Service

**Nota**: essa tela está disponível atualmente apenas para o usuário principal da conta.

1. Acesse o [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} usando suas credenciais exclusivas.
2. Selecione **Armazenamento** > **Migração de dados** > **Transferência de dados** na Barra de navegação para acessar a tela Data Transfer Service. <br/>

Ao acessar a tela Data Transfer Service, os usuários poderão enviar uma solicitação de transferência de dados, visualizar detalhes sobre uma solicitação, visualizar o histórico de chamado associado ao rastreamento de dispositivo para uma solicitação e cancelar uma solicitação existente.

## Enviando uma solicitação de transferência de dados

As solicitações de transferência de dados foram projetadas para permitir que as partes apropriadas em nossos data centers saibam esperar uma remessa de um cliente. As solicitações são enviadas por meio do [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window}. Ao criar uma solicitação, lembre-se das diretrizes a seguir:

- Assegure-se de que o dispositivo que está sendo enviado em associação à solicitação atenda a todos os [requisitos de hardware](/docs/infrastructure/DataTransferService/data-transfer-service-faq.html).
- Apenas um dispositivo pode ser associado a cada solicitação. Se você quiser enviar múltiplos dispositivos, crie uma nova solicitação para cada dispositivo.
- Se o dispositivo precisar ser retornado, forneça a etiqueta de remessa pré-paga e documentos de exportação, conforme necessário, no pacote para que o dispositivo possa ser retornado após o período de transferência.
- Se o envio for internacional, você será responsável por obter todo o licenciamento, envio e liberação da alfândega para o Dispositivo, incluindo o pagamento de taxas, impostos e custos de frete de e para (se aplicável) o data center da IBM.
- A transportadora e o número de rastreamento da remessa para o nosso data center devem ser fornecidos ao concluir a solicitação. Assegure-se de que a etiqueta tenha sido criada com o endereço apropriado do data center antes de concluir a solicitação.

Siga as etapas abaixo para enviar uma solicitação de transferência de dados.

1. Acesse a tela **Data Transfer Service** no [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window}. <br/> **Nota**: essa tela está disponível apenas para o usuário principal da conta.
2. Clique em **Pedir solicitação de transferência de dados** na parte superior da tela.
3. Preencha cada campo na seção **Informações sobre o dispositivo** de acordo com a tabela abaixo.
<table border="1">
<tbody>
 <tr><th>Nome de Campo</th><th>Instruções</th></tr>
 <tr><td>Tipo de dispositivo</td><td>O tipo de dispositivo que está sendo enviado para o destino. Se o tipo de dispositivo não estiver listado, selecione "Outro".</td></tr>
 <tr><td>Número de série</td><td> O número de série do dispositivo.</td></tr><tr><td>Descrição</td><td>Uma breve descrição do dispositivo. Detalhes importantes a serem incluídos podem ser fatores de identificação, como cor, etiquetas ou adesivos anexados, etc.</td></tr>
 <tr><td>Nota</td><td>Quaisquer notas adicionais sobre o dispositivo ou a transferência.</td></tr><tr><td>Destino</td><td>O data center que receberá o dispositivo.</td></tr>
 <tr><td>Transportadora</td><td>Transportadora postal ou expressa usada para enviar o dispositivo para seu destino.</td></tr>
 <tr><td>Número de rastreamento</td><td>Número de rastreamento completo para a remessa.</td></tr>
 </tbody>
 </table>

4. Preencha cada campo na seção **Endereço de retorno** ou marque a caixa de seleção **Endereço da empresa** para preencher automaticamente os campos com o endereço da empresa no arquivo. <br/> **Nota**: lembre-se de incluir a etiqueta de envio de retorno pré-paga e documentos de exportação, conforme necessário, no pacote para que o dispositivo possa ser retornado após o período de transferência.
5. Marque a caixa de seleção **Li e concordo com o Contrato de Prestação de Serviços de Transferência de Dados e o Contrato de Prestação de Serviços Principal** depois de ler cada contrato de prestação de serviços fornecido.
6. Clique em **Enviar solicitação de serviço** para enviar a solicitação. Clique em **Cancelar** para cancelar a ação.

Depois de enviar a solicitação, o status para o chamado de solicitação aparecerá como *Enviado para o SoftLayer*. Notifique-nos se alguma remessa de importação ou exportação requerer uma licença de seu governo local e anexe informações sobre licença no chamado.

Depois que o dispositivo for recebido, o status será atualizado para *Recebido pelo SoftLayer* e atualizado novamente para *Conectado* depois que um técnico do data center tiver conectado o dispositivo à nossa rede. 

O período de transferência de dados inicial deve durar no máximo duas (2) semanas. Durante esse tempo, o acesso ao dispositivo é permitido apenas ao administrador de conta. Se for necessário tempo adicional, uma extensão poderá ser solicitada. Por outro lado, se o dispositivo tiver que ser enviado antes de duas (2) semanas, poderá ser feita uma solicitação de retorno. Deve-se notificar a {{site.data.keyword.IBM}} por meio do [{{site.data.keyword.slportal}}](https://control.softlayer.com/) quando a transferência está completa. Vamos então remover o Dispositivo e retorná-lo ou destruí-lo, dependendo do que você solicitou.


## Acessando a tela Remessas

A tela Remessas dentro do [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} exibe todas as remessas associadas a solicitações do Data Transfer Service. Nessa tela, as remessas podem ser visualizadas e as remessas de retorno podem ser confirmadas no recebimento. Siga as etapas abaixo para acessar a tela Remessas.

1. Acesse o [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} usando suas credenciais exclusivas.
2. Selecione **Conta** > **Gerenciar** > **Remessas** na Barra de navegação para acessar a tela Remessas.

Ao acessar a tela Remessas, todas as solicitações de envio dos últimos 30 dias são exibidas na lista de remessas junto a detalhes sobre cada remessa. As remessas podem ser [classificadas ou filtradas](sort-or-filter-shipments-list.html) por status, idade ou detalhes específicos da remessa. Além disso, o recebimento de remessas de retorno pode ser confirmado nessa tela.
![Tela Remessas](/images/DTSShipmentScreen1.png)
