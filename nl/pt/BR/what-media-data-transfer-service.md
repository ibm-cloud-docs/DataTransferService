---

copyright:
  years: 2017
lastupdated: "2017-12-18"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# O que é Media Data Transfer Service?
 
O Data Transfer Service é um serviço que permite enviar um dispositivo compatível com USB 2.0 ou USB 3.0 e/ou CDs e DVDs para um data center do {{site.data.keyword.BluSoftlayer_full}} para serem conectados diretamente à sua rede. O dispositivo é hospedado em um rack dedicado localizado no data center à sua escolha e será montado como um destino iSCSI. Unidades de formato avançado agora também são suportadas.

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
2.    Primeiras 2 semanas de Transferência de dados: US$ 0
**Nota**: será cobrado US$ 25 por semana para extensão
3.    Custo do frete de e para o data center da {{site.data.keyword.IBM}}, incluindo o pagamento de taxas e impostos.

**Nota**: o cliente é responsável por:  
- assegurar-se de que nenhuma licença de importação ou exportação seja necessária para enviar o Dispositivo para o data center da {{site.data.keyword.IBM}} ou para retorná-lo para o Cliente (se aplicável); 
- assegurar-se de que nem o Cliente nem qualquer usuário final do Cliente cujos dados estejam incluídos no Conteúdo estejam sujeitos a qualquer ordem do governo dos Estados Unidos que revogue ou negue seus privilégios de exportação dos EUA. O Cliente concorda em notificar a {{site.data.keyword.IBM}} imediatamente se o Cliente ou qualquer usuário final do Cliente se tornar sujeito a qualquer ordem desse tipo;  
- obter todo o licenciamento, envio e liberação da alfândega para o Dispositivo, incluindo o pagamento de taxas, impostos e custos de frete de e para (se aplicável) o data center da {{site.data.keyword.IBM}}.   
- obedecer todas as leis aplicáveis, incluindo privacidade, importação e exportação, associados à entrega e retorno do Dispositivo, além da transferência de Conteúdo para o data center da {{site.data.keyword.IBM}}; e 
- ter contratos adequados em vigor e obter todas as permissões necessárias com o usuário final do Cliente para qualquer Cliente de dados do usuário final transferidas para o Hardware.

## Fazendo uma solicitação
Isso é feito em **Armazenamento** > **Migração de dados** > **Transferência de dados** e, em seguida, clicando no link **Pedir solicitação de transferência de dados** na parte superior direita da página.

![Fazendo uma solicitação de transferência de dados](/images/DTS.png)
 

Preencha este formulário com os dispositivos
1. Número de série
2. Tipo
3. Uma descrição simples do dispositivo
4. O data center para o qual você gostaria que o dispositivo fosse
5. O número de rastreamento usado para rastrear a remessa
6. O serviço da transportadora usado
7. O endereço de retorno para o qual você gostaria que o dispositivo fosse enviado na conclusão.

Depois de preenchido, isso criará automaticamente um chamado de suporte para alertar nossos técnicos de que o dispositivo está sendo enviado para nós, permitindo a eles a capacidade de rastrear a entrega. Depois de recebermos o dispositivo, continuaremos a conectá-lo ao nosso rack dedicado. Quando tivermos conectado o dispositivo, o chamado será atualizado, fornecendo um link para suas credenciais de logon para o destino iSCSI.

## Solicitar retorno
Se você tiver fornecido um endereço de retorno e tiver incluído a etiqueta de remessa pré-paga no pacote, será possível solicitar que o dispositivo seja enviado de volta para você a qualquer momento durante o período de transferência de 2 semanas. Isso é feito por meio do [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} selecionando **Armazenamento** > **Migração de dados** > **Transferência de dados** e na lista suspensa **Ação** de seu dispositivo, você seleciona **solicitar retorno**. Isso alertará nossos técnicos que você gostaria que o dispositivo fosse desconectado e enviado de volta para você.

## Solicitar extensão
Após seu período de 2 semanas grátis, se você ainda requer o uso do dispositivo USB, deve-se solicitar uma extensão que alertará nossos técnicos que você gostaria de ampliar o tempo de conexão do dispositivo. Isso é feito da mesma maneira que você solicitaria o retorno de seu dispositivo selecionando **Armazenamento** > **Migração de dados** > **Transferência de dados** e na lista suspensa **Ação** do dispositivo, selecionaria **solicitar extensão**. Cada semana além das duas primeiras haverá uma taxa de serviço de 25 dólares que deverá ser paga. Além disso, dependendo do espaço disponível no data center para seu dispositivo, sua solicitação poderá ser negada. Se a solicitação for concedida, o chamado será atualizado, indicando que você recebeu a semana extra.

## Desconectar
Após o período de duas semanas, o dispositivo será desconectado automaticamente do nosso data center e retornado a você pela transportadora escolhida e para o endereço de retorno especificado na solicitação inicial. O chamado será atualizado, indicando que o dispositivo foi desconectado. Se você não tiver solicitado o retorno do dispositivo, ele será destruído no local.
