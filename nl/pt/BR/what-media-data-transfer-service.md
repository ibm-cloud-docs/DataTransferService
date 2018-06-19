---

copyright:
  years: 2017, 2018
lastupdated: "2018-05-22"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# O que é serviço de transferência de dados de mídia?
 
O serviço de transferência de dados permite enviar um dispositivo compatível com USB 2.0 ou 3.0, CDs e DVDs para um data center do {{site.data.keyword.BluSoftlayer_full}} para ser conectado diretamente à sua rede. O dispositivo é hospedado em um rack dedicado e é montado como um destino iSCSI. Unidades de formato avançado agora também são suportadas.

## Requisitos de hardware
1.    O dispositivo deve ter uma fonte de alimentação compatível com 208 v/220 v
2.    O dispositivo deve ter um plugue de energia que se ajuste a um soquete padrão de 120 v (NEMA 5-15P)
3.    O dispositivo deve ser compatível com USB 2.0 (3.0 agora também é suportado)
4.    O dispositivo deve vir com cabo USB com conector Macho USB A (plug padrão que se ajusta à maioria dos computadores)
5.    CDS/DVDS
      1.    Deve estar em livros CD, caixas ou alguma forma de contêiner e de preferência todos juntos em um contêiner (Um livro CD, por exemplo) e cada disco deve ter uma etiqueta exclusiva.
      2.    Os discos serão girados por solicitação do cliente por meio do chamado

## Custo para você
1.    Solicitação inicial de serviço: US$ 0
2.    Primeiras 2 semanas de Transferência de dados: $ 0
**Nota**: será cobrado $ 25 por semana para extensão
3.    Custo do frete de e para o data center da {{site.data.keyword.IBM}}, incluindo o pagamento de taxas e impostos.

**Nota**: o cliente é responsável por:  
- assegurar-se de que nenhuma licença de importação ou exportação seja necessária para enviar o Dispositivo para o data center da {{site.data.keyword.IBM}} ou para retorná-lo para o Cliente (se aplicável); 
- assegurar que o Cliente ou qualquer usuário do Cliente cujos dados estejam incluídos no Conteúdo não esteja sujeito a nenhuma ordem do governo dos EUA que revogue ou negue seus privilégios de exportação dos EUA. Notifique a {{site.data.keyword.IBM}} imediatamente se o Cliente ou qualquer usuário se tornar sujeito a qualquer ordem desse tipo;  
- obter todo o licenciamento, envio e liberação da alfândega para o Dispositivo. As responsabilidades do Cliente incluem o pagamento de taxas, impostos e custos de frete para/de (se aplicável) o data center da {{site.data.keyword.IBM}}.   
- obedecer a todas as leis aplicáveis que estão associadas à entrega e ao retorno do Dispositivo, além da transferência de Conteúdo para o data center da {{site.data.keyword.IBM}}. Isso inclui leis de privacidade, importação e exportação.
- ter contratos adequados em vigor e obter todas as permissões necessárias do usuário do Cliente para quaisquer dados do usuário que o Cliente deseja transferir para o Hardware.

## Fazendo uma solicitação
Isso é feito por meio de **Armazenamento** > **Migração de dados** > **Transferência de dados**, em seguida, clique em **Pedir solicitação de transferência de dados** no canto superior direito.

![Fazendo uma solicitação de transferência de dados](/images/DTS.png)

Conclua o formulário com estas informações do dispositivo
1. Número de série
2. Tipo
3. Uma descrição simples do dispositivo
4. O data center para o qual você gostaria que o dispositivo fosse
5. O número de rastreamento que é usado para rastrear a remessa
6. O serviço da transportadora que é usado
7. O endereço de retorno para o qual você gostaria que o dispositivo fosse enviado na conclusão.

Essa solicitação cria um chamado de suporte para alertar nossos técnicos de que o dispositivo está sendo enviado para nós e permite que eles rastreiem a entrega. Quando recebermos o dispositivo, nós o conectamos ao nosso rack dedicado. Depois que conectamos o dispositivo, o chamado é atualizado para fornecer a você um link para suas credenciais de logon para o destino iSCSI.

## Solicitar retorno
Se você forneceu um endereço de retorno e incluiu a etiqueta de remessa pré-paga no pacote, é possível solicitar que o dispositivo seja enviado de volta a qualquer momento durante o período de transferência de duas semanas. Isso pode ser feito por meio do [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window}. Selecione **Armazenamento** > **Migração de dados** > **Transferência de dados** e, no menu **Ação** de seu dispositivo, selecione **Solicitar retorno**. Isso alerta nossos técnicos que você deseja que o dispositivo seja desconectado e enviado de volta.

## Solicitar extensão
Após seu período de duas semanas grátis, se você ainda requer o uso do dispositivo, deve-se solicitar uma extensão. Isso alerta nossos técnicos que você deseja estender o tempo que o dispositivo está conectado. É possível fazer isso da mesma maneira que solicitaria que seu dispositivo fosse retornado para você. Selecione **Armazenamento** > **Migração de dados** > **Transferência de dados** e, no menu **Ação** para o dispositivo, selecione **Solicitar extensão**. Cada semana extra incorre em uma taxa de serviço de $ 25 que deve ser paga. Observe que sua solicitação de extensão pode ser negada dependendo do espaço disponível no data center. Quando a solicitação é concedida, o chamado é atualizado de acordo.

## Desconectar
Após o período de duas semanas, o dispositivo é desconectado automaticamente do nosso data center. Se você solicitou um retorno, então seu dispositivo é retornado para você pela transportadora escolhida e para o endereço de retorno especificado na solicitação inicial. O chamado é atualizado indicando que o dispositivo foi desconectado. Se você não solicitou o retorno de seu dispositivo, então ele é destruído no local.
