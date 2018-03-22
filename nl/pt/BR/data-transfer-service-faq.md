---

copyright:
  years: 1994, 2017
lastupdated: "2017-12-18"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Perguntas mais frequentes do Data Transfer Service

## O que é Data Transfer?

A transferência de dados permite que os usuários autorizados (geralmente administrador da conta) enviem os dispositivos compatíveis com um dos nossos data centers para serem conectados diretamente à rede da conta. O dispositivo é hospedado em um rack dedicado no data center selecionado e montado como um destino iscsi por um período de duas (2) semanas. Durante esse período, o administrador pode acessar o dispositivo na rede para usá-lo com outros dispositivos e/ou serviços na conta. Após o período de duas semanas, uma extensão poderá ser solicitada para manter o dispositivo conectado à rede. Caso contrário, o dispositivo será retornado para a parte especificada na seção de endereço de retorno quando a solicitação foi criada ou o dispositivo será destruído no local se o retorno não tiver sido solicitado.


## Posso enviar um Dispositivo para transferência de dados internacionalmente?

Hardware e discos podem ser enviados tanto interna como internacionalmente para qualquer um de nossos data centers; entretanto, você como Cliente é responsável por:

- assegurar-se de que nenhuma licença de importação ou exportação seja necessária para enviar o Dispositivo para o data center da {{site.data.keyword.IBM}} ou para retorná-lo para o Cliente (se aplicável);
- assegurar-se de que nem o Cliente nem qualquer usuário final do Cliente cujos dados estejam incluídos no Conteúdo estejam sujeitos a qualquer ordem do governo dos Estados Unidos que revogue ou negue seus privilégios de exportação dos EUA. O Cliente concorda em notificar a {{site.data.keyword.IBM}} imediatamente se o Cliente ou qualquer usuário final do Cliente se tornar sujeito a qualquer ordem desse tipo;
- obter todo o licenciamento, envio e liberação da alfândega para o Dispositivo, incluindo o pagamento de taxas, impostos e custos de frete de e para (se aplicável) o data center da {{site.data.keyword.IBM}};
- obedecer todas as leis aplicáveis, incluindo privacidade, importação e exportação, associados à entrega e retorno do Dispositivo, além da transferência de Conteúdo para o data center da {{site.data.keyword.IBM}}; e
- ter contratos adequados em vigor e obter todas as permissões necessárias com o usuário final do Cliente para qualquer Cliente de dados do usuário final transferidas para o Hardware.

Inclua uma etiqueta de envio de retorno pré-paga e todos os documentos de exportação apropriados com sua remessa e empacotaremos os dispositivos para retorno usando a etiqueta e os documentos fornecidos. Se o retorno não tiver sido solicitado, o dispositivo será destruído.


## Que tipos de dispositivos posso enviar com uma Solicitação de transferência de dados?
Use as diretrizes a seguir ao selecionar um dispositivo ou um disco (CD ou DVD) para enviar para a transferência de dados:

- Requisitos de hardware:
   - A fonte de alimentação deve ser compatível com 208 v/220 v.

   - O plugue de energia deve ajustar-se a um soquete padrão de 120 v (NEMA 5-15P).

   - O dispositivo deve ser compatível com USB 2.0 ou USB 3.0.

   - Forneça um conector Macho USB A (plug USB padrão que se ajusta à maioria dos computadores).
 
- Requisitos de CD/DVD:

   - Os discos devem ser enviados em livros CD, caixas ou contêineres semelhantes. Se for enviar múltiplos discos, armazene os discos juntos em uma única caixa ou livro CD.

   - Cada disco deve ter uma etiqueta clara e exclusiva (por exemplo, Disco A, Disco B, Disco C etc.).
   
## Posso obter meu dispositivo mais cedo ou deixá-lo lá além de duas semanas durante o processo de transferência de dados? 

Sim, seu hardware ou discos poderão ser retornados a qualquer momento ou poderão ficar conectados mais tempo, se necessário. Para solicitar um retorno ou uma extensão, inclua um comentário no chamado original da Solicitação de transferência de dados com a solicitação apropriada. Se estiver solicitando um retorno, desconectaremos e retornaremos o hardware ou os discos para o endereço de entrega de retorno fornecido na solicitação original usando as etiquetas de remessa pré-pagas e o pacote fornecidos. 

Se estiver solicitando uma extensão, a solicitação de extensão será processada o mais rápido possível. É importante observar que cada solicitação de extensão amplia o tempo que o dispositivo está conectado em uma semana e pode estar sujeita a uma taxa de extensão. Detalhes adicionais serão incluídos quando um membro de nossa equipe responder à solicitação no chamado original.
   
## O que cada status em meu chamado de transferência de dados significa?

Cada status no chamado de transferência de dados indica a fase do processo de transferência do hardware ou discos enviados para o data center. Consulte a tabela abaixo para obter detalhes específicos sobre cada status:

|Status 	| Definição |
|---------| -----------|
|Enviado para o SoftLayer |A Solicitação de transferência de dados foi enviada pelo usuário e o hardware ou os discos estão sendo enviados para o data center selecionado.|
|Recebido pelo SoftLayer |	A remessa foi recebida pelo data center, foi designada a uma série e foi escaneada em nosso sistema.|
|Conectar |	O hardware ou o disco foi conectado ao dispositivo.|
|Conectado |	Um destino iscsi foi criado para o dispositivo.|
|Solicitação de extensão |	O usuário solicitou uma extensão no tempo de conexão de duas (2) semanas.|
|Solicitação de retorno | O usuário solicitou o retorno do hardware ou dos discos.|
|Desconectar |	A desconexão do hardware ou dos discos foi iniciada.|
|Desconectado |	O destino foi removido com segurança pelos Sistemas de informações.|
|Destruído | O dispositivo foi destruído no local depois de nosso procedimento de destruição de HDD.|
|Retornar pelo SoftLayer |	O hardware ou os discos foram empacotados e enviados para o endereço de retorno fornecido na solicitação original.|
