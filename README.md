# Template para processos Upstream e Downstream

## Upstream

Estágio de concepção e definição da feature que precisa ser entregue

### Etapas

#### Discovery

Etapa de investigação e entendimento do problema ou oportunidade de produto a ser endereçado. Guiado principalmente pelo time de Produto, envolvendo os times de Design e Engenharia de acordo com o necessário. Tem como resultado a definição do problema ou oportunidade.

#### Design

Etapa de definição da solução, delimitando claramente o escopo a ser implementado. Envolve ativamente os times de Design e Engenharia, podendo conter processos de definição de UX, prototipação de telas, validação de viabilidade e custo técnicos, documentação de fluxo de negócio, definição de MVP (Minimum Viable Product) e POCs (Proofs of concept).

#### Split

Etapa de quebra da solução a ser implementada em pacotes menores de valor, como histórias de usuário. Histórias devem atender as definições DoR (Definition of Ready) e DoD (Definition of Done) acordadas pelo time. Recomendado o uso da matrix INVEST (Independent, Negotiable, Valuable, Estimable, Small, Testable) como referência para a definição das histórias.

## Downstream

Estágio de refinamento técnico, organização e execução do trabalho para entrega da feature

### Etapas

#### Refining

Sessão de definição da arquitetura macro a ser implementada ou ajustada, podendo derivar em documentação técnica, enriquecimento técnico das histórias e quebra em tarefas menores, quando apropriado. Recomendado que as tarefas tenham tamanho uniforme (esforço + complexidade) para permitir maior previsibilidade de entrega. 

#### Planning

Definição do escopo de tarefas a ser implementadas no intervalo de tempo definido (sprint).

#### Developing

Etapas Designing, Implementing, Documenting podem ocorrer comitantemente.

##### Designing

Design a nível de API e componentes do que vai ser implementado. Exemplos: definição de endpoints, design de banco de dados, componentes frontend, etc.

##### Implementing

Codificação da feature ou correção do bug.

##### Testing

Implementação de testes de unidade, integração e e2e, quando aplicáveis.

##### Documenting

Documentação de APIs (swagger), eventos (AsyncAPI), arquitetura de sistemas, quando aplicáveis.

##### Instrumenting

Configuração de ferramentas de monitoramento e observabilidade, quando aplicáveis.

##### Code Reviewing

Revisão de código realizada por um ou mais pares do time de desenvolvimento.

##### Staging

Validação a nível de negócio e técnico em ambiente pré-produtivo. Pode requerer validação de stakeholders (ex: Product Manager, Designer) antes de seguir para Releasing.

##### Releasing

Escrita de: 

Release Notes: lista em alto nível da entrega (ex: épicos, histórias, bug fixes), tem como audiência os stakeholders do produto e pode ser direcionado ao usuários finais do produto.

Changelog: lista em baixo nível da entrega (ex: tarefas), contendo detalhes técnicos das mudanças realizadas (ex: adição, remoção, refatoramento de módulos/componentes do código; detalhes sobre breaking changes)

Geração do pacote a ser feito deploy, deve seguir o versionamento semântico.

### Deploying

Aplicação da estratégia de deploy (ex: blue/green, gradual rollout, canary) para o ambiente produtivo.

### Maintaining/Monitoring

Monitoramento e manutenção em produção após o deploy. Acompanhamento de alertas sobre a saúde das aplicações e atuação para mitigar possíveis problemas.
