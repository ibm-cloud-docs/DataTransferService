---

copyright:
  years: 2017, 2019
lastupdated: "2019-02-05"

---
{:new_window: target="_blank"}

# Introduzindo o serviço de transferência de dados de mídia
{: #mediaDTS}

Com o serviço de transferência de dados, é possível enviar um dispositivo compatível com USB 2.0 ou 3.0, CDs e DVDs
para um data center do {{site.data.keyword.BluSoftlayer_full}} para serem conectados diretamente à sua rede. O dispositivo é hospedado em um rack dedicado e é montado como um destino iSCSI. Unidades de formato avançado agora também são suportadas.

## Requisitos de hardware
1.    O dispositivo deve ter uma fonte de alimentação compatível com 208 v/220 v
2.    O dispositivo deve ter um plugue de energia que se ajuste a um soquete padrão de 120 v (NEMA 5-15P)
3.    O dispositivo deve ser compatível com USB 2.0 (3.0 agora também é suportado)
4.    O dispositivo deve vir com cabo USB com conector Macho USB A (plug padrão que se ajusta à maioria dos computadores)
5.    CDS/DVDS
      - Devem estar em porta-CDs, caixas ou alguma forma de contêiner. É possível colocá-los todos juntos em um contêiner (um porta-CDs, por exemplo). Cada disco deve ser rotulado de forma exclusiva.
      - Os discos são girados mediante a solicitação do cliente por meio do chamado.

## Custo para você
1.    Solicitação inicial para serviço = $0
2.    Primeiras duas semanas de transferência de dados = US$ 0 **Nota**: são cobrados US$ 25 por semana por
extensão.
3.    Custo do frete de e para o data center da {{site.data.keyword.IBM}}, incluindo o pagamento de taxas e impostos.

** Nota **: o cliente é responsável por
- Assegurar que nenhuma licença de importação ou de exportação seja necessária para enviar o dispositivo para o data center
da {{site.data.keyword.IBM}} ou para retorná-lo ao Cliente (se aplicável).
- Assegurar que o Cliente ou qualquer usuário do Cliente cujos dados estejam incluídos no conteúdo não esteja sujeito a nenhuma
norma governamental dos EUA que revogue ou negue os seus privilégios de exportação nos EUA. Notifique
a {{site.data.keyword.IBM}} imediatamente se o Cliente ou qualquer usuário se tornar sujeito a qualquer norma desse tipo.
- Obter todo o licenciamento, a remessa e a liberação da alfândega para o dispositivo. As responsabilidades do cliente incluem
o pagamento de quaisquer taxas, impostos e custos do frete para o data center da {{site.data.keyword.IBM}} ou dele (se
aplicável).
- Estar em conformidade com todas as leis aplicáveis associadas à entrega e ao retorno do dispositivo
e à transferência de conteúdo para o data center da {{site.data.keyword.IBM}}. Esse requisito inclui as leis de privacidade,
de importação e de exportação.
- Ter contratos adequados em vigor com o usuário do Cliente e obter todas as permissões necessárias dele para quaisquer dados
do usuário que o Cliente desejar transferir para o hardware.

## Fazendo uma solicitação
É possível enviar uma solicitação por meio do [{{site.data.keyword.slportal}} ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/){:new_window}

1. Clique em  ** Armazenamento **  >  ** Migração de Dados **  >  ** Transferência de Dados **.
2. Clique em  ** Pedir solicitação de transferência de dados **.

![Fazendo uma solicitação de transferência de dados](/images/DTS.png)

Conclua o formulário com estas informações do dispositivo
1. Número de série
2. Tipo
3. Uma descrição simples do dispositivo
4. O data center para o qual você deseja enviar o dispositivo
5. O número de rastreamento que é usado para rastrear a remessa
6. O serviço da transportadora que é usado
7. O endereço de retorno de onde você deseja que o dispositivo seja enviado após a conclusão da transferência de dados.

Essa solicitação cria um chamado de suporte para alertar os técnicos do {{site.data.keyword.BluSoftlayer}} de que
o dispositivo está sendo enviado e permite que eles rastreiem a entrega. Quando o {{site.data.keyword.BluSoftlayer}} recebe
o dispositivo, os técnicos o conectam ao rack dedicado. Quando o dispositivo é conectado, o chamado é atualizado para fornecer um
link para as suas credenciais de logon para o destino iSCSI.

## Solicitando uma Devolução
Se você forneceu um endereço de retorno e incluiu a etiqueta de remessa pré-paga no pacote, será possível
solicitar que o dispositivo seja enviado de volta a qualquer momento durante o período de transferência de duas semanas. É possível enviar a solicitação por meio do [{{site.data.keyword.slportal}} ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/){:new_window}.

1. Selecione  ** Armazenamento **  >  ** Migração de Dados **  >  ** Transferência de Dados **.
2. No menu **Ação** do dispositivo, selecione **Solicitação de retorno**.

Essa atualização alerta os técnicos do {{site.data.keyword.BluSoftlayer}} de que você deseja que o dispositivo
seja desconectado e enviado de volta.

## Solicitando uma Extensão
Após seu período gratuito de duas semanas, se você ainda requerer o uso de seu dispositivo, deverá solicitar uma extensão por meio do [{{site.data.keyword.slportal}} ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/){:new_window}. Essa atualização
alerta os técnicos do {{site.data.keyword.BluSoftlayer}} de que você deseja estender o tempo de conexão do dispositivo.

1. Selecione  ** Armazenamento **  >  ** Migração de Dados **  >  ** Transferência de Dados **
2. No menu **Ação** para o dispositivo, selecione **Solicitação de extensão**.

Cada semana extra incorre em uma taxa de serviço de $ 25 que deve ser paga. A solicitação de extensão pode ser negada
dependendo do espaço disponível no data center. Quando a solicitação é concedida, o chamado é atualizado.

## Desconectando o Dispositivo
Após o período de duas semanas, o dispositivo é automaticamente desconectado do data center. Se você solicitou um retorno, então seu dispositivo é retornado para você pela transportadora escolhida e para o endereço de retorno especificado na solicitação inicial. O chamado é atualizado indicando que o dispositivo foi desconectado. Se você não solicitou o retorno de seu dispositivo, então ele é destruído no local.
