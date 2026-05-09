# Plano de Melhoria Sugerido

Com base na auditoria realizada e na observação de que as ferramentas de gestão (como Milestones) já existem no repositório, mas carecem de uso sistemático, as duas ações prioritárias para atingir a conformidade com o **MPS.BR Nível G** são as seguintes:

## 1. Institucionalização da Gestão de Milestones e Cronogramas
A auditoria constatou que, embora a aba de Milestones não esteja vazia, ela não apresenta maturidade e não há um planeamento com prazos definidos ou estimativas de esforço. O uso atual é esporádico e não serve como ferramenta de controle administrativo.

A melhoria proposta consiste em adotar uma rotina obrigatória de planejamento, em que cada ciclo de desenvolvimento, como as versões v0.8.5 e v0.9.0, esteja vinculado a um milestone com data de entrega definida e estimativa de esforço.

Essa ação está alinhada ao MPS.BR, na área de Gerência de Projetos (GPR), que prevê a definição de cronograma e do esforço necessário para a execução das tarefas. Com isso, os milestones passam a ser utilizados para acompanhar o progresso do projeto em relação ao planejamento, e não apenas para agrupar issues concluídas.

Como aplicação prática, nenhuma issue deve ser movida para “In Progress” sem estar associada a um milestone ativo no GitHub com prazo definido.

## 2. Formalização da Trilha de Rastreabilidade via Processo de RFC
A auditoria de Engenharia de Requisitos identificou que o projeto não possui um processo formal de *Request for Comments* (RFC) ou documentação de *design* prévia. As mudanças são feitas diretamente via Pull Requests, o que compromete a rastreabilidade de decisões arquiteturais.

A ação proposta consiste em instituir um processo formal de RFC (Request for Comments) para mudanças significativas no projeto, utilizando um modelo padrão para registrar a necessidade da alteração, a solução técnica proposta e a aprovação dos mantenedores antes do início da codificação.

Essa prática está alinhada ao MPS.BR, especialmente nos processos de Gerência de Requisitos (GRE) e Planejamento do Projeto (PJR), pois contribui para o controle das mudanças nos requisitos e para a manutenção da consistência entre os requisitos e os produtos desenvolvidos.

Como implementação prática, sugere-se a criação de um diretório /rfcs no repositório, de modo que decisões arquiteturais importantes passem por esse fluxo antes da criação de issues técnicas ou do desenvolvimento do código, garantindo o registro formal da intenção da mudança.

## 3. Reforço nos Testes e na Validação das Saídas com IA

Na parte de Verificação e Validação, foi observado que o Crawl4AI já possui testes automatizados, exemplos de uso e revisão por Pull Requests. Esses pontos ajudam a verificar se o projeto funciona corretamente e mostram uma preocupação com a qualidade do código.

Apesar disso, não ficou claro se todos os Pull Requests passam obrigatoriamente por testes antes de serem integrados ao projeto. Os workflows encontrados estão mais ligados a release, Docker e notificações, e não a uma verificação completa de cada alteração feita no código.

Como melhoria, seria importante criar um fluxo obrigatório de testes para Pull Requests. Esse fluxo poderia executar os testes automatizados, verificar se o projeto compila corretamente, analisar a formatação do código e indicar a cobertura dos testes. Com isso, o projeto teria mais segurança antes de aceitar novas mudanças.

Outro ponto importante é a validação das saídas geradas com apoio de LLMs. O projeto já usa recursos como schemas, JSON, CSS/XPath, regex e filtros de conteúdo, que ajudam a deixar a extração mais controlada. Mesmo assim, seria interessante adicionar testes que comparem a saída gerada com uma saída esperada, para verificar se o conteúdo extraído está realmente fiel à página original.

Dessa forma, o projeto teria mais segurança tanto na revisão do código quanto na qualidade das informações entregues ao usuário.

