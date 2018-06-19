---

copyright:
  years: 1994, 2018
lastupdated: "2018-05-22"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Perguntas mais frequentes

## O que é Data Transfer?

Esse serviço permite que os usuários autorizados (geralmente o administrador da conta) enviem os dispositivos compatíveis para um dos nossos data centers para serem conectados diretamente à rede da conta. O dispositivo é hospedado em um rack dedicado e é montado como um destino iSCSI por duas semanas. Durante esse período, o administrador pode acessar o dispositivo na rede para usá-lo com outros dispositivos e serviços na conta. Após o período de duas semanas, uma extensão pode ser solicitada para manter o dispositivo conectado à rede. Caso contrário, o dispositivo é retornado para a parte especificada na solicitação ou o dispositivo é destruído no local.

## Posso enviar um dispositivo para transferência de dados internacionalmente?

O hardware e os discos podem ser enviados tanto interna como internacionalmente para qualquer um de nossos data centers. No entanto, você, como Cliente, é responsável por:

- assegurar que nenhuma licença de importação ou exportação seja necessária para enviar o Dispositivo para o data center da {{site.data.keyword.IBM}} ou para retorná-lo para o Cliente (se aplicável);
- assegurar que o Cliente ou qualquer usuário do Cliente cujos dados estejam incluídos no Conteúdo não esteja sujeito a nenhuma ordem do governo dos EUA que revogue ou negue seus privilégios de exportação dos EUA. A {{site.data.keyword.IBM}} deverá ser notificada imediatamente se sua empresa ou qualquer usuário se tornar sujeito a qualquer ordem desse tipo;
- obter todo o licenciamento, envio e liberação da alfândega para o Dispositivo, incluindo o pagamento de taxas, impostos e custos de frete de/para (se aplicável) o data center da {{site.data.keyword.IBM}}.
- obedecer a todas as leis aplicáveis, incluindo privacidade, importação e exportação, que estão associadas à entrega e ao retorno do Dispositivo, além da transferência de Conteúdo para o data center da {{site.data.keyword.IBM}} e
- ter contratos adequados em vigor e obter todas as permissões necessárias com o usuário do Cliente para quaisquer dados do usuário que o Cliente de dados transferirá para o hardware.

Inclua uma etiqueta de envio de retorno pré-pago e todos os documentos de exportação apropriados com sua remessa e empacotaremos o dispositivo para retorno usando a etiqueta e os documentos fornecidos. Se o retorno não for solicitado, o dispositivo será destruído.


## Quais tipos de dispositivos posso enviar com uma solicitação de transferência de dados?
Use as diretrizes a seguir ao selecionar um dispositivo ou um disco (CD ou DVD) para enviar para a transferência de dados:

- Requisitos de hardware:
   - A fonte de alimentação deve ser compatível com 208 v/220 v.

   - O plugue de energia deve ajustar-se a um soquete padrão de 120 v (NEMA 5-15P).

   - O dispositivo deve ser compatível com USB 2.0 ou USB 3.0.

   - Forneça um conector Macho USB A (plug USB padrão que se ajusta à maioria dos computadores).

- Requisitos de CD/DVD:

   - Os discos devem ser enviados em livros CD, caixas ou contêineres semelhantes. Se você desejar enviar múltiplos discos, armazene os discos juntos em uma única caixa ou livro CD.

   - Cada disco deve ter uma etiqueta clara e exclusiva (como Disco A, Disco B, Disco C e assim por diante).

## Posso pegar meu dispositivo de volta mais cedo ou deixar que ele fique por mais de duas semanas?

Sim, seu hardware ou discos poderão ser retornados a qualquer momento ou poderão ficar conectados mais tempo, se necessário. Para solicitar um retorno ou uma extensão, inclua um comentário no chamado da solicitação de transferência de dados original com a solicitação apropriada. Se você solicitar um retorno, desconectaremos e retornaremos o hardware ou os discos para o endereço de entrega de retorno fornecido na solicitação original usando as etiquetas de remessa pré-paga e o pacote fornecidos.

Se você solicitar uma extensão, a solicitação de extensão será processada o mais rápido possível. É importante observar que cada solicitação de extensão estende o prazo que o dispositivo está conectado em uma semana e pode estar sujeita a uma taxa de extensão. Detalhes adicionais serão incluídos quando um membro de nossa equipe responder à solicitação no chamado original.

## O que cada status em meu chamado de transferência de dados significa?

Cada status no chamado de transferência de dados indica a fase do processo de transferência do hardware ou discos enviados para o data center. Consulte a tabela abaixo para obter detalhes específicos sobre cada status:

|Status 	| Definição |
|---------| -----------|
|Enviado para o SoftLayer 	|A Solicitação de transferência de dados foi enviada pelo usuário e o hardware ou os discos estão sendo enviados para o data center selecionado.|
|Recebido pelo SoftLayer |	A remessa foi recebida pelo data center, o dispositivo foi designado a um número de série e foi escaneado em nosso sistema.|
|Conectar |	O hardware ou o disco está conectado ao dispositivo.|
|Conectado |	Um destino iSCSI foi criado para o dispositivo.|
|Solicitação de extensão | O usuário solicitou uma extensão no tempo de conexão de duas semanas.|
|Solicitação de retorno | O usuário solicitou o retorno do hardware ou dos discos.|
|Desconectar |	A desconexão do hardware ou dos discos foi iniciada.|
|Desconectado |	O destino está seguramente removido.|
|Destruído | O dispositivo foi destruído no site depois de nosso procedimento de destruição de HDD.|
|Retornar pelo SoftLayer |	O hardware ou os discos foram empacotados e enviados para o endereço de retorno fornecido na solicitação original.|
