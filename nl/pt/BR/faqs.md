---

copyright:
  years: 2017, 2019
lastupdated: "2019-02-05"

---
{:faq: data-hd-content-type='faq'}

# Perguntas frequentes

## O que é Data Transfer?
{: faq}

Esse serviço permite que os usuários autorizados (geralmente o administrador da conta) enviem dispositivos compatíveis para um
dos data centers do {{site.data.keyword.BluSoftlayer_full}} para que sejam conectados diretamente à rede da conta. O dispositivo é hospedado em um rack dedicado e é montado como um destino iSCSI por duas semanas. Durante esse período, o administrador pode acessar o dispositivo na rede para usá-lo com outros dispositivos e serviços na conta. Após o período de duas semanas, uma extensão pode ser solicitada para manter o dispositivo conectado à rede. Caso contrário, o dispositivo é retornado para a parte especificada na solicitação ou o dispositivo é destruído no local.

## Um dispositivo para a transferência de dados pode ser enviado internacionalmente?
{: faq}

O hardware e os discos podem ser enviados nacionalmente e internacionalmente para qualquer um dos data centers do
{{site.data.keyword.BluSoftlayer}}. No entanto, você, como Cliente, é responsável por:

- Assegurar que nenhuma licença de importação ou de exportação seja necessária para enviar o dispositivo para o data center
da {{site.data.keyword.IBM}} ou para retorná-lo ao Cliente (se aplicável);
- Assegurar que o Cliente ou qualquer usuário do Cliente cujos dados estejam incluídos no conteúdo não esteja sujeito a nenhuma
norma governamental dos EUA que revogue ou negue os seus privilégios de exportação nos EUA. A {{site.data.keyword.IBM}} deverá ser notificada imediatamente se sua empresa ou qualquer usuário se tornar sujeito a qualquer ordem desse tipo;
- Obter todo o licenciamento, a remessa e a liberação da alfândega para o dispositivo, incluindo o pagamento das taxas, dos
impostos e dos custos do frete para o data center da {{site.data.keyword.IBM}} e dele (se aplicável);
- Estar em conformidade com todas as leis aplicáveis, incluindo a privacidade, a importação e a exportação associadas à entrega e ao retorno do dispositivo, e à transferência de conteúdo para o data center da {{site.data.keyword.IBM}}; e
- Ter contratos adequados em vigor com o usuário do Cliente e obter todas as permissões necessárias dele para quaisquer dados
do usuário que o Cliente desejar transferir para o hardware.

Inclua na remessa um rótulo de frete de retorno pré-pago e todos os documentos de exportação apropriados. O
{{site.data.keyword.BluSoftlayer}} empacota o dispositivo para retorno usando o rótulo e os documentos fornecidos. Se o
retorno não for solicitado, o dispositivo será destruído.


## Quais os tipos de dispositivos podem ser enviados com uma solicitação de transferência de dados?
{: faq}

Use as diretrizes a seguir ao selecionar um dispositivo ou um disco (CD ou DVD) para enviar para a transferência de dados:

- **Requisitos de hardware**

   - A fonte de alimentação deve ser compatível com 208 v/220 v.

   - O plugue de energia deve ajustar-se a um soquete padrão de 120 v (NEMA 5-15P).

   - O dispositivo deve ser compatível com USB 2.0 ou USB 3.0.

   - Forneça um conector Macho USB A (plug USB padrão que se ajusta à maioria dos computadores).

- ** Requisitos de CD/DVD **

   - Os discos devem ser enviados em livros CD, caixas ou contêineres semelhantes. Se você desejar enviar múltiplos discos, armazene os discos juntos em uma única caixa ou livro CD.

   - Cada disco deve estar rotulado com clareza e de forma exclusiva.

## O dispositivo pode ser enviado de volta mais cedo ou pode ficar mais de duas semanas?
{: faq}

Sim, seu hardware ou discos poderão ser retornados a qualquer momento ou poderão ficar conectados mais tempo, se necessário. Para solicitar um retorno ou uma extensão, inclua um comentário no chamado da solicitação de transferência de dados original com a solicitação apropriada. Se você solicitar um retorno, o {{site.data.keyword.BluSoftlayer}} desconectará e retornará o hardware ou os discos para o
endereço de retorno fornecido na solicitação original usando os rótulos de remessa pré-pagos e o pacote
fornecido.

Se você solicitar uma extensão, a solicitação de extensão será processada o mais rápido possível. É importante observar que cada solicitação de extensão estende o prazo que o dispositivo está conectado em uma semana e pode estar sujeita a uma taxa de extensão. Mais detalhes serão incluídos quando um membro da equipe do {{site.data.keyword.BluSoftlayer_full}} responder à
solicitação no chamado original.

Cada status no chamado de transferência de dados indica a fase do processo de transferência para o hardware ou os discos que
foram enviados para o data center. Consulte a tabela para obter detalhes específicos sobre cada status:

|Status 	| Definição |
|---------| -----------|
|`Sent To SoftLayer` |A solicitação de transferência de dados foi enviada pelo usuário e o hardware ou os
discos estão sendo enviados para o data center selecionado.|
|`Received by SoftLayer` |	A remessa foi recebida pelo data center, um número de série foi designado ao
dispositivo e ele foi escaneado no sistema do {{site.data.keyword.BluSoftlayer}}.|
|`Connect` |	O hardware ou o disco está conectado ao dispositivo.|
|`Connected` |	Um destino iSCSI foi criado para o dispositivo.|
|`Request for Extension` | O cliente solicitou uma extensão no tempo de conexão de duas semanas.|
|`Request for Return` | O cliente solicitou o retorno do hardware ou dos discos.|
|`Disconnect` |	A desconexão do hardware ou dos discos foi iniciada.|
|`Disconnected` |	O destino está seguramente removido.|
|`Destroyed` | O dispositivo foi destruído no local seguindo o procedimento de destruição de HDD do {{site.data.keyword.BluSoftlayer}}.|
|`Return by SoftLayer` |	O hardware ou os discos foram empacotados e enviados para o endereço de retorno fornecido na solicitação original.|
