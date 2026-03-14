Use este prompt completo como mensagem inicial no Claude Code, em um repositório vazio:

Quero inicializar neste repositório vazio uma estrutura completa de governança para Claude Code.

Objetivo central
Inicialize este repositório para que a governança se torne o sistema operacional persistente de todas as futuras solicitações em linguagem natural.

Importante
- Este repositório se tornará um projeto específico, com arquitetura, decisões tecnológicas, convenções de nomenclatura, organização de pastas, regras de negócio, comportamentos esperados, contratos e instruções próprias.
- Apenas esta mensagem inicial de bootstrap deve ser genérica, para que eu possa reutilizá-la em outros repositórios.
- Não assuma domínio, stack, framework, linguagem de programação, estilo arquitetural ou modelo de negócio durante o bootstrap.
- Depois do bootstrap, este repositório deve evoluir com base no seu próprio contexto acumulado e na sua própria governança persistida.
- Não crie uma estrutura decorativa.
- Crie um sistema de governança funcional.
- Escreva conteúdo operacional dentro dos arquivos criados para que eles orientem ativamente o comportamento futuro neste repositório.
- O comportamento operacional futuro deve ficar definido dentro dos arquivos criados agora, e não depender de prompts operacionais futuros do usuário.

Objetivo do bootstrap
Criar uma estrutura persistente de governança para que toda mensagem futura do usuário, escrita em linguagem natural, seja suficiente para que o Claude:
- interprete a mensagem corretamente
- normalize semanticamente a intenção
- classifique o tipo de solicitação
- identifique o contexto relevante dentro do repositório
- consulte a governança acumulada
- atualize instruções e definições quando necessário
- propague impactos entre arquivos relacionados
- implemente mudanças no repositório quando aplicável
- revise alinhamento entre implementação e governança quando aplicável
- faça tudo isso com base no conteúdo persistido nos arquivos criados neste bootstrap

Modelo operacional permanente
Trate toda mensagem futura do usuário neste repositório como entrada operacional suficiente.

Não exija que o usuário forneça instruções adicionais de processo como:
- classifique isso
- normalize isso
- atualize a governança primeiro
- consulte as regras
- consulte a arquitetura
- use contratos
- use BDD
- alinhe a implementação com a governança
- propague mudanças relacionadas
- confirme se o trecho de código é exemplo ou obrigatório quando isso já estiver explicitamente dito pelo usuário

Esses comportamentos devem ser escritos na governança do repositório e tratados como comportamento operacional persistente.

Tratamento de linguagem natural
O usuário pode escrever ou ditar em linguagem natural.
A entrada do usuário pode conter:
- erros de português
- frases incompletas
- autocorreções
- repetições
- ambiguidades
- padrões de fala
- pensamento não linear
- reformulações dentro da mesma mensagem
- solicitações imperativas curtas com pouco contexto explícito

Antes de executar qualquer ação, sempre:
1. interprete semanticamente a mensagem
2. normalize a intenção do usuário
3. resolva problemas óbvios de escrita em português apenas para fins de entendimento
4. preserve a intenção, não a formulação imperfeita
5. converta o significado em linguagem técnica clara antes de persistir qualquer conteúdo

Nunca:
- exija que o usuário reescreva uma mensagem apenas porque ela foi informal, ditada, fragmentada ou imperfeita
- copie erros brutos de escrita para arquivos de governança, instruções, contratos, BDD, código ou artefatos declarativos
- invente regras de domínio ausentes
- invente restrições técnicas ausentes
- invente comportamento de negócio ausente apenas para preencher lacunas

Quando o contexto estiver incompleto:
- consulte primeiro a governança do repositório
- prefira a menor interpretação coerente compatível com o contexto já existente
- use premissas conservadoras
- registre premissas relevantes quando elas afetarem comportamento, design ou consistência futura

Política de dúvidas, ambiguidades e resolução
Escreva na governança do repositório uma política explícita para tratamento de dúvidas, ambiguidades, lacunas e conflitos de interpretação.

Essa política deve determinar que:
- se houver ambiguidade material, dúvida relevante ou lacuna de informação que possa comprometer a implementação correta, o Claude não deve sair executando imediatamente
- antes de implementar, o Claude deve registrar a dúvida ou ambiguidade nos arquivos apropriados do repositório
- o Claude deve responder no prompt com as dúvidas encontradas, o impacto delas e o que precisa ser confirmado
- o Claude só deve implementar sem confirmação do usuário quando a governança existente já permitir uma premissa mínima, conservadora e coerente
- toda premissa relevante usada sem confirmação explícita deve ser registrada
- quando a dúvida for resolvida pelo usuário em mensagem posterior, o Claude deve atualizar a governança afetada, a implementação correspondente e os arquivos de dúvidas e premissas
- dúvidas resolvidas não devem permanecer como pendências abertas
- premissas resolvidas não devem permanecer como premissas ativas
- arquivos ativos de dúvidas e premissas devem conter apenas itens ainda pendentes ou ainda válidos
- quando uma dúvida for resolvida, o Claude deve remover a dúvida da lista ativa e refletir a resolução nos arquivos definitivos do repositório
- quando uma premissa for confirmada ou invalidada, o Claude deve atualizar ou remover essa premissa do log ativo e refletir o resultado nos arquivos definitivos do repositório
- se for importante manter rastreabilidade, o Claude pode registrar a resolução em local apropriado de histórico, mas não deve manter o item como aberto

Crie uma estrutura específica para isso com pelo menos:
- open-questions.md
- assumptions-log.md

E crie uma rule específica para isso:
- .claude/rules/ambiguity-handling.md

Tratamento obrigatório de ambiguidades
Escreva explicitamente que:
- dúvidas pequenas que não alteram comportamento, arquitetura, contrato, segurança, persistência, mensageria, nomenclatura relevante ou experiência do usuário podem ser resolvidas com premissas mínimas conservadoras
- dúvidas que afetem comportamento funcional, regra de negócio, contratos, BDD, arquitetura, segurança, integração, mensageria, persistência, modelagem de dados ou impacto estrutural devem ser registradas e reportadas antes da implementação
- quando existir dúvida relevante, o Claude deve preferir pausar a implementação e pedir esclarecimento, em vez de inventar uma resposta forte demais
- se parte da solicitação puder ser executada com segurança e outra parte depender de esclarecimento, o Claude deve deixar essa divisão explícita
- quando o esclarecimento chegar, o Claude deve remover a dúvida da lista ativa, atualizar as premissas relacionadas e consolidar a resposta correta na governança definitiva

Política para trechos de código, snippets e artefatos fornecidos pelo usuário
Escreva na governança do repositório uma política explícita para tratamento de trechos de código, snippets, configurações, contratos, artefatos declarativos, templates, YAML, JSON, SQL, Terraform, Helm, políticas IAM, definições de mensageria, schemas, migrations e qualquer outro fragmento técnico enviado pelo usuário.

Essa política deve determinar que todo trecho fornecido pelo usuário deve ser classificado em uma destas categorias:
- snippet normativo
- exemplo ilustrativo
- padrão preferencial
- referência técnica contextual

Definições obrigatórias dessas categorias:
- snippet normativo:
  - o usuário deixa explícito que aquele trecho deve ser incluído, copiado, preservado, usado na íntegra, mantido exatamente, aplicado literalmente, inserido sem reescrita, tratado como canônico ou equivalente
- exemplo ilustrativo:
  - o usuário deixa explícito que o trecho é apenas exemplo, referência, inspiração, base, direção ou algo “nessa linha”
- padrão preferencial:
  - o usuário indica que quer seguir aquela abordagem, mas sem exigir cópia literal
- referência técnica contextual:
  - o trecho serve para mostrar intenção técnica, esclarecer comportamento ou contextualizar um requisito

Regras obrigatórias para snippets normativos
Escreva explicitamente que:
- se o usuário disser de forma explícita que quer que o trecho seja incluído na íntegra, copiado integralmente, preservado exatamente ou aplicado literalmente, o Claude deve tratar esse trecho como snippet normativo
- snippets normativos devem ser copiados na íntegra para o local apropriado do projeto, respeitando apenas os ajustes estritamente necessários de encaixe estrutural do arquivo de destino quando isso for inevitável
- o conteúdo lógico do snippet normativo não deve ser reescrito livremente
- o Claude não deve “melhorar”, “otimizar”, “refatorar”, “embelezar” ou reinterpretar livremente um snippet normativo
- se houver necessidade técnica real de adaptação mínima para compatibilidade, essa adaptação deve ser:
  - mínima
  - explícita
  - justificada
  - reportada no resumo final
- se o snippet normativo conflitar com a estrutura existente, com regras de segurança, com contratos ativos ou com limitações técnicas relevantes, o Claude deve:
  - registrar a dúvida ou conflito
  - explicar o impacto no prompt
  - não substituir silenciosamente o trecho por outra implementação
- snippets normativos devem poder ser persistidos como referência canônica do repositório quando fizer sentido para governança futura

Regras obrigatórias para exemplos ilustrativos
Escreva explicitamente que:
- se o usuário disser que o trecho é exemplo, referência, base, inspiração, “algo assim” ou equivalente, o Claude deve tratar esse trecho como exemplo ilustrativo
- exemplos ilustrativos não devem ser copiados literalmente por obrigação
- exemplos ilustrativos devem ser interpretados à luz do contexto do projeto
- o Claude pode adaptar, reestruturar, renomear ou reescrever exemplos ilustrativos para encaixar melhor na governança, arquitetura e estilo do repositório
- o Claude deve preservar a intenção técnica do exemplo, não necessariamente sua literalidade

Regras obrigatórias para padrões preferenciais
Escreva explicitamente que:
- padrões preferenciais devem influenciar a solução, mas não obrigam preservação literal
- o Claude deve tentar manter a abordagem, estrutura e filosofia do trecho
- adaptações são permitidas desde que a intenção principal permaneça reconhecível
- divergências relevantes devem ser reportadas

Regras obrigatórias para referência técnica contextual
Escreva explicitamente que:
- referências contextuais servem para orientar entendimento
- elas não exigem cópia literal
- elas podem influenciar classificação, desenho, validação ou implementação
- elas devem ser usadas como contexto complementar

Persistência de snippets normativos
Crie uma estrutura específica para persistir snippets normativos quando eles forem relevantes para o comportamento futuro do repositório, com pelo menos:
- Instructions/snippets/
- Instructions/snippets/README.md
- Instructions/snippets/canonical-snippets.md

Escreva explicitamente que:
- snippets normativos fornecidos pelo usuário podem ser registrados nessa área como referências canônicas
- trechos persistidos como canônicos devem ser respeitados em futuras implementações
- o Claude não deve reescrever livremente referências canônicas já registradas
- qualquer alteração futura em snippet canônico deve exigir nova instrução explícita do usuário ou conflito técnico devidamente reportado

Tratamento de classificação de trechos
Escreva explicitamente que:
- se o usuário indicar claramente a natureza do trecho, o Claude deve respeitar essa classificação sem reinterpretá-la arbitrariamente
- se o usuário não indicar claramente a natureza do trecho, o Claude deve inferir com cautela com base na formulação usada
- se ainda houver dúvida material sobre tratar o trecho como normativo ou ilustrativo, o Claude deve registrar a ambiguidade antes de implementar de forma irreversível
- na ausência de sinal claro de literalidade obrigatória, o Claude deve assumir que o trecho é ilustrativo ou preferencial, não normativo

Pipeline obrigatório de execução
Escreva no repositório que o assistente deve seguir internamente esta sequência para toda mensagem do usuário:

1. Interpretar semanticamente a mensagem
2. Normalizar a intenção do usuário
3. Classificar a solicitação em uma ou mais categorias
4. Identificar os arquivos de governança relevantes
5. Ler a governança relevante antes de agir
6. Verificar se há ambiguidades, dúvidas materiais ou lacunas
7. Verificar se há trechos técnicos enviados pelo usuário e classificar cada trecho como normativo, ilustrativo, preferencial ou contextual
8. Registrar dúvidas e premissas quando necessário
9. Atualizar ou remover dúvidas e premissas que tenham sido resolvidas pela nova mensagem do usuário
10. Atualizar a governança primeiro sempre que a mensagem introduzir ou alterar qualquer definição durável
11. Propagar impactos entre artefatos relacionados quando necessário
12. Só então implementar, alterar, remover ou revisar mudanças no repositório
13. Informar:
   - intenção interpretada
   - arquivos consultados
   - arquivos alterados
   - trechos classificados como normativos, ilustrativos, preferenciais ou contextuais
   - premissas adotadas
   - conflitos encontrados
   - dúvidas registradas
   - dúvidas removidas ou resolvidas
   - o que passa a valer como fonte de verdade ativa

Definição de nova definição
Escreva explicitamente na governança que “nova definição” inclui qualquer adição ou mudança durável, como:
- nova regra de negócio
- alteração de regra de negócio existente
- nova restrição
- nova exceção
- novo fluxo
- novo conceito de domínio
- novo invariante
- novo contrato
- alteração de contrato
- novo cenário BDD
- mudança no comportamento esperado do sistema
- nova convenção de nomenclatura
- alteração de nomenclatura
- nova regra de organização de pastas
- mudança estrutural de organização
- nova regra arquitetural
- novo princípio técnico
- nova decisão técnica
- ambiguidade resolvida que deva persistir como conhecimento do repositório
- snippet canônico ou fragmento normativo que deva passar a governar futuras implementações

Política de atualização da governança
Sempre atualize a governança primeiro e só depois implemente.

Escreva isso explicitamente:
- Se a mensagem do usuário introduzir ou alterar uma definição durável, a governança deve ser atualizada antes de qualquer mudança de código, infraestrutura declarativa, contratos, artefatos de mensageria, banco como código ou outros artefatos do repositório.
- Se a implementação depender de uma nova interpretação, essa interpretação deve ser persistida primeiro.
- Se a solicitação já estiver totalmente coberta pela governança existente, o assistente pode implementar diretamente, mas ainda deve validar se a governança continua alinhada após a implementação.

Política de conhecimento durável
Escreva regras explícitas dizendo:
- persista conhecimento durável
- não promova detalhes transitórios de implementação para a governança, a menos que eles afetem decisões futuras
- a governança armazena regras, decisões, restrições, terminologia, comportamentos, padrões de interpretação e snippets canônicos duráveis
- a governança não é um log bruto de atividade
- a governança não é um despejo de toda escolha incidental de codificação
- persista apenas o que deve continuar guiando trabalho futuro

Prioridade entre fontes de verdade
Escreva regras explícitas de prioridade:
1. Contratos executáveis, artefatos formais equivalentes e snippets normativos explicitamente declarados como canônicos pelo usuário
2. BDD
3. Regras de negócio estruturadas
4. Arquitetura e padrões técnicos
5. Convenções de nomenclatura, estilo e organização

Política de conflito
Escreva regras explícitas de conflito:
- contrato prevalece sobre texto narrativo
- BDD prevalece sobre texto narrativo
- comportamento de negócio prevalece sobre preferência arquitetural quando essa preferência invalidar o comportamento esperado
- convenções de nomenclatura, estilo e organização não podem prevalecer sobre comportamento de negócio, BDD ou contratos
- snippets normativos explicitamente declarados pelo usuário não devem ser reescritos silenciosamente
- conflitos nunca devem ser ignorados
- conflitos devem ser reportados
- conflitos devem ser refletidos nos arquivos apropriados do repositório
- a interpretação escolhida deve seguir a ordem de prioridade definida

Evolução específica do repositório
Escreva regras explícitas dizendo:
- o bootstrap é genérico apenas como mecanismo de inicialização
- este repositório deve evoluir como um contexto específico
- toda nova mensagem deve ser interpretada à luz da governança específica já acumulada neste repositório
- o assistente deve preferir o contexto do repositório a suposições genéricas
- o funcionamento futuro não deve depender de o usuário reexplicar o processo

Documento central de modelo operacional
Crie um documento central de modelo operacional que consolide o comportamento de runtime do repositório.
Esse documento deve explicar:
- como solicitações são interpretadas
- como solicitações são classificadas
- quando a governança deve ser atualizada
- por que a governança é atualizada antes da implementação
- como impactos são propagados
- como a prioridade entre fontes funciona
- como ambiguidades são tratadas
- como dúvidas são registradas
- como snippets são classificados
- quando um trecho deve ser copiado literalmente
- quando um trecho pode ser adaptado ao contexto
- como o contexto do repositório se torna específico ao longo do tempo
- como solicitações curtas em linguagem natural devem ser interpretadas com segurança

Distinção entre rules e Instructions
Deixe a estrutura explícita:
- .claude/rules/ contém comportamento operacional do assistente
- Instructions/architecture/ contém memória arquitetural e instruções técnicas do repositório
- Instructions/business/ contém memória de negócio e regras de domínio específicas do repositório
- Instructions/bdd/ contém cenários comportamentais
- Instructions/contracts/ contém artefatos formais de interface, contratos de mensagens, schemas e outros contratos relevantes
- Instructions/glossary/ contém governança terminológica
- Instructions/decisions/ contém decisões registradas e ADRs
- Instructions/snippets/ contém referências canônicas de snippets normativos quando isso for relevante
- open-questions.md contém dúvidas abertas relevantes ao repositório
- assumptions-log.md contém premissas adotadas e seu contexto
- Instructions/operating-model.md contém o modelo operacional consolidado do repositório

Política para BDD e contratos
Escreva explicitamente que BDD e contratos são importantes, mas não obrigatórios para toda mudança.
Inclua regras como:
- use BDD quando o comportamento se beneficiar de especificação por cenários
- use contratos quando interfaces, payloads, mensagens, schemas ou integrações exigirem formalização
- não force toda mudança a gerar artefatos de BDD ou contrato
- só crie ou atualize esses artefatos quando eles forem relevantes para a mudança ou necessários para consistência

Política para solicitações curtas
Escreva regras explícitas para lidar com mensagens curtas e imperativas do usuário, como:
- crie um novo item
- exclua por id
- atualize a imagem do cliente
- adicione uma nova regra
- crie BDD para esse fluxo

O assistente deve:
- consultar o contexto do repositório
- inferir de forma conservadora
- evitar assumir demais
- evitar pedir esclarecimentos desnecessários quando a governança do repositório já for suficiente
- registrar premissas relevantes quando necessário
- registrar dúvidas quando a solicitação curta não for suficiente para implementação segura

Escopo de aplicação do sistema
Escreva explicitamente que este sistema de governança deve servir para repositórios de:
- código de aplicação
- infraestrutura como código
- mensageria e contratos de eventos
- topologias com SNS, SQS, tópicos, filas e integrações
- definições de banco como código
- schemas, payloads e artefatos operacionais ou declarativos
- outros repositórios em que exista conhecimento durável que deva governar mudanças futuras

Escreva também que:
- “implementar” não se restringe a código de aplicação
- “implementar” pode significar materializar mudanças em código, infraestrutura declarativa, contratos, mensageria, banco, configuração ou documentação operacional
- “contratos” não se restringem a APIs HTTP
- “contratos” também podem incluir contratos de mensagens, schemas e interfaces operacionais relevantes ao repositório

Tarefa
Crie a estrutura completa de governança abaixo e escreva conteúdo forte, operacional e normativo dentro dos arquivos.
Não crie arquivos fracos ou meramente descritivos.
Não crie arquivos vazios.
Não crie arquivos compostos apenas por placeholders sem valor operacional.

Estrutura obrigatória
- CLAUDE.md
- .claude/rules/
- .claude/skills/
- .claude/hooks/
- Instructions/operating-model.md
- Instructions/architecture/
- Instructions/business/
- Instructions/bdd/
- Instructions/contracts/
- Instructions/glossary/
- Instructions/decisions/
- Instructions/snippets/
- open-questions.md
- assumptions-log.md
- README.md

Requisitos do CLAUDE.md
Crie um CLAUDE.md curto, mas forte.

Ele deve instruir explicitamente que:
- toda mensagem do usuário neste repositório é entrada operacional
- o assistente deve interpretar semanticamente antes de agir
- o assistente deve ler a governança relevante antes de implementar
- o assistente deve verificar ambiguidades antes de implementar
- o assistente deve registrar dúvidas abertas e premissas quando necessário
- o assistente deve classificar trechos técnicos enviados pelo usuário antes de decidir se deve copiá-los literalmente ou adaptá-los
- o assistente deve atualizar a governança primeiro quando uma definição durável for introduzida ou alterada
- a implementação deve seguir a governança do repositório
- a prioridade entre fontes de verdade deve ser respeitada
- o contexto do repositório é específico e acumulado ao longo do tempo
- o comportamento futuro é governado pelos arquivos criados neste bootstrap
- o assistente não deve depender de o usuário repetir instruções de processo

Use @imports explícitos para os arquivos de governança mais importantes, incluindo:
- regras de normalização de linguagem natural
- regras de ingestão técnica
- regras de ingestão de negócio
- regras de prioridade entre fontes
- regras de alinhamento para implementação
- regras de tratamento de ambiguidades
- regras de evolução do contexto do repositório
- @Instructions/operating-model.md
- @Instructions/architecture/technical-overview.md
- @Instructions/business/business-rules.md
- @Instructions/bdd/conventions.md
- @Instructions/contracts/README.md
- @Instructions/glossary/ubiquitous-language.md
- @Instructions/snippets/README.md
- @Instructions/snippets/canonical-snippets.md
- @open-questions.md
- @assumptions-log.md

Rules obrigatórias em .claude/rules/
Crie todos estes arquivos em português do Brasil, com instruções explícitas de comportamento:

- architecture-governance.md
- technical-ingestion.md
- business-ingestion.md
- natural-language-normalization.md
- source-of-truth-priority.md
- implementation-alignment.md
- naming-governance.md
- folder-governance.md
- change-propagation.md
- repository-context-evolution.md
- ambiguity-handling.md
- snippet-handling.md

Escreva-os como orientação operacional normativa, não como comentário passivo.

Conteúdo mínimo obrigatório por arquivo de rule

1. architecture-governance.md
Inclua instruções explícitas para:
- identificar solicitações relacionadas à arquitetura
- registrar princípios técnicos
- registrar padrões
- registrar restrições
- separar governança técnica de governança de negócio
- atualizar arquivos em Instructions/architecture
- registrar decisões arquiteturais
- avaliar impacto arquitetural na implementação
- impedir que preferência arquitetural invalide comportamento de negócio exigido

2. technical-ingestion.md
Inclua um workflow explícito para:
- classificar entrada técnica
- decidir se a entrada pertence a arquitetura, princípios, nomenclatura, padrões, organização de pastas ou decisões
- atualizar a instrução técnica apropriada
- manter consistência entre arquivos técnicos
- preservar conhecimento técnico durável
- recusar promover detalhe incidental de implementação a governança durável

3. business-ingestion.md
Inclua um workflow explícito para:
- classificar entrada de negócio
- decidir se o conteúdo pertence a business-rules, invariants, workflows, domain-model, assumptions, BDD ou contracts
- lidar com comportamento de negócio descrito em linguagem solta
- registrar dependências
- propagar mudanças de negócio para artefatos relacionados
- preservar significado durável de negócio em forma normalizada

4. natural-language-normalization.md
Inclua regras explícitas para:
- interpretar português imperfeito
- lidar com entrada ditada ou fragmentada
- lidar com ambiguidade e autocorreção
- reconstruir semanticamente a intenção
- consultar o contexto do repositório antes de assumir
- usar a menor premissa coerente
- nunca persistir formulação bruta mal escrita
- sempre normalizar conteúdo antes de atualizar instruções ou código

5. source-of-truth-priority.md
Inclua:
- ordem explícita de prioridade
- regras de resolução de conflito
- regras para documentação de conflito
- regras para seleção da fonte prevalente
- regras para refletir a resolução nos artefatos do repositório
- regras para resumir a decisão tomada

6. implementation-alignment.md
Inclua um workflow obrigatório explícito para solicitações de implementação:
- interpretar a solicitação
- classificar a solicitação
- ler a governança relevante
- verificar ambiguidades e lacunas primeiro
- classificar snippets enviados pelo usuário
- registrar dúvidas ou premissas antes de implementar quando necessário
- atualizar a governança primeiro se qualquer definição durável for nova ou alterada
- avaliar necessidade de propagação
- implementar apenas depois que a governança estiver alinhada
- relatar fontes usadas, snippets normativos preservados, snippets adaptados, premissas e conflitos

7. naming-governance.md
Inclua:
- como convenções de nomenclatura são introduzidas
- como mudanças de nomenclatura são propagadas
- distinção entre terminologia de negócio e nomenclatura técnica
- como manter consistência terminológica entre Instructions, BDD, contratos e código
- como evitar deriva de vocabulário ambíguo

8. folder-governance.md
Inclua:
- como regras de estrutura de pastas são registradas
- como mudanças estruturais são decididas
- como a organização do repositório é documentada
- como evitar proliferação de artefatos vazios ou desnecessários
- como mudanças de pastas afetam instruções de arquitetura e estrutura de implementação

9. change-propagation.md
Inclua regras explícitas de propagação:
- se negócio muda, avalie BDD, contratos, glossário e implementação
- se contratos mudam, avalie negócio, BDD, glossário e implementação
- se BDD muda, avalie negócio, contratos e implementação
- se arquitetura muda, avalie instruções técnicas, organização de pastas e implementação
- se nomenclatura muda, avalie todos os artefatos relacionados
- se snippet canônico muda, avalie implementações relacionadas e referências associadas
- exija pensamento transversal antes de concluir qualquer mudança

10. repository-context-evolution.md
Inclua instruções explícitas de que:
- o bootstrap é genérico apenas no momento da inicialização
- a governança do repositório se torna específica pelo uso
- decisões futuras devem preferir o histórico do repositório a suposições genéricas
- o assistente deve operar com base no contexto acumulado do repositório
- o usuário não deve precisar reapresentar o comportamento de processo

11. ambiguity-handling.md
Inclua regras explícitas para:
- detectar dúvidas materiais e ambiguidades relevantes
- distinguir ambiguidade pequena de ambiguidade que bloqueia implementação segura
- registrar dúvidas em @open-questions.md
- registrar premissas em @assumptions-log.md
- responder no prompt antes de codificar quando a dúvida for relevante
- só permitir implementação imediata quando a premissa mínima for conservadora e coerente com a governança
- atualizar os registros de dúvida e premissa quando o usuário esclarecer a questão depois
- remover das listas ativas as dúvidas resolvidas
- remover ou atualizar premissas que deixarem de valer
- consolidar a resolução nos arquivos definitivos do repositório

12. snippet-handling.md
Inclua regras explícitas para:
- classificar trechos fornecidos pelo usuário como normativos, ilustrativos, preferenciais ou contextuais
- preservar snippets normativos na íntegra quando o usuário pedir isso explicitamente
- não reescrever livremente snippets normativos
- permitir adaptação de exemplos ilustrativos conforme o contexto do projeto
- permitir adaptação moderada de padrões preferenciais
- usar referências contextuais apenas como apoio de entendimento
- registrar snippets normativos canônicos em Instructions/snippets/canonical-snippets.md quando isso for útil para governança futura
- relatar qualquer adaptação mínima feita em snippet normativo
- não substituir silenciosamente um trecho literal por outra implementação “melhor”

Skills obrigatórias em .claude/skills/
Crie uma pasta por skill, cada uma contendo um arquivo SKILL.md completo.

Todos os arquivos SKILL.md devem estar em português do Brasil e devem incluir:
- nome
- descrição
- quando usar
- entradas esperadas
- workflow interno
- saídas esperadas
- arquivos de governança relacionados

Crie estas skills:
- ingest-definition
- implement-request
- review-alignment
- evolve-governance
- resolve-ambiguity
- apply-user-snippet

Conteúdo mínimo obrigatório por skill

1. ingest-definition
Essa skill deve orientar o comportamento quando o usuário introduzir ou alterar uma definição durável.
Ela deve cobrir:
- interpretação semântica
- classificação em governança técnica ou de negócio
- atualização da governança primeiro
- propagação entre artefatos relacionados
- persistência de conhecimento durável
- normalização para linguagem técnica limpa

2. implement-request
Essa skill deve orientar o comportamento quando o usuário solicitar:
- nova funcionalidade
- alteração de comportamento
- exclusão ou remoção de comportamento
- implementação guiada por regra
- atualização com base nas definições do repositório
Ela deve cobrir:
- interpretação semântica
- consulta obrigatória à governança
- verificação de ambiguidades antes da implementação
- classificação de trechos técnicos enviados pelo usuário
- política de governança primeiro
- implementação baseada nas fontes de verdade do repositório
- relatório final com fontes, snippets normativos preservados, snippets adaptados, premissas e conflitos

3. review-alignment
Essa skill deve orientar revisão de coerência entre:
- código e artefatos declarativos
- instruções de arquitetura
- instruções de negócio
- BDD
- contratos
- glossário
- decisões
- snippets canônicos
- dúvidas abertas
- premissas registradas
Ela deve cobrir:
- detecção de inconsistência
- identificação de lacunas
- reporte de conflito
- sugestões coerentes de resolução

4. evolve-governance
Essa skill deve orientar evolução da base de instruções sem perda semântica.
Ela deve cobrir:
- consolidação de conteúdo duplicado
- reorganização de seções
- preservação de conhecimento durável
- melhoria de clareza
- manutenção da consistência entre documentos

5. resolve-ambiguity
Essa skill deve orientar o comportamento quando houver dúvida, ambiguidade ou lacuna relevante.
Ela deve cobrir:
- interpretação da dúvida
- avaliação de impacto
- distinção entre dúvida bloqueante e dúvida não bloqueante
- registro em @open-questions.md
- registro em @assumptions-log.md
- resposta no prompt com a pergunta ou com a premissa adotada
- atualização posterior dos registros quando o usuário esclarecer
- remoção das dúvidas resolvidas da lista ativa
- remoção ou atualização das premissas que deixarem de valer
- consolidação da resolução nos arquivos definitivos do repositório

6. apply-user-snippet
Essa skill deve orientar o comportamento quando o usuário fornecer trecho de código, configuração ou artefato técnico.
Ela deve cobrir:
- classificação do trecho
- distinção entre snippet normativo e exemplo ilustrativo
- cópia integral quando o usuário exigir literalidade
- adaptação contextual quando o trecho for apenas exemplo
- registro de snippets canônicos quando aplicável
- reporte explícito sobre o que foi copiado literalmente e o que foi adaptado

Comportamento importante das skills
Escreva explicitamente que essas skills:
- apoiam o comportamento persistente do repositório
- não exigem que o usuário invoque comandos especiais
- existem para reforçar o modelo operacional do repositório
- devem ser compatíveis com o contexto específico acumulado pelo repositório

Hooks obrigatórios em .claude/hooks/
Crie scripts placeholder genéricos e exemplos de configuração que reforcem o modelo operacional.
Não finja fornecer enforcement real específico de stack quando a stack ainda é desconhecida.
Documente dentro dos artefatos de hook, em português do Brasil:
- propósito
- intenção de gatilho
- qual comportamento eles reforçam
- por que são placeholders
- como devem ser adaptados quando a stack do repositório se tornar concreta

Crie artefatos de hook cobrindo:
- detecção de mudança na governança
- lembrete de governança primeiro antes de implementação
- sinalização de inconsistência entre negócio, BDD, contratos e implementação
- validação mínima de coerência após mudanças de governança
- tratamento de ambiguidade antes de implementação
- registro de dúvidas e premissas
- preservação e rastreabilidade de snippets normativos
- notas de adaptação futura para enforcement específico de stack

Requisitos do documento de modelo operacional
Crie Instructions/operating-model.md em português do Brasil com orientação consolidada forte.
Esse documento deve explicar:
- propósito do repositório
- como o assistente opera
- como mensagens são interpretadas
- como tipos de mensagem são classificados
- o que conta como nova definição
- por que a governança é atualizada primeiro
- como conhecimento durável é selecionado
- como propagação entre artefatos funciona
- como prioridade entre fontes funciona
- como ambiguidade é tratada
- como dúvidas são registradas
- como premissas são registradas
- como snippets são classificados
- quando a implementação deve esperar esclarecimento
- quando um trecho deve ser copiado literalmente
- quando um trecho pode ser adaptado
- como solicitações curtas são tratadas
- como o contexto específico do repositório evolui ao longo do tempo

Arquivos obrigatórios em Instructions/architecture/
Crie:
- technical-overview.md
- engineering-principles.md
- patterns.md
- naming-conventions.md
- folder-structure.md
- architecture-decisions.md

Todos esses arquivos devem estar em português do Brasil.
Cada arquivo deve conter estrutura durável como:
- propósito
- princípios ou decisões ativas
- restrições
- convenções
- premissas
- futuras adições
- referências cruzadas
- placeholders de histórico de mudança

Não invente detalhes técnicos específicos do projeto.
Crie estrutura forte e reutilizável para futura evolução específica do repositório.

Arquivos obrigatórios em Instructions/business/
Crie:
- business-rules.md
- invariants.md
- workflows.md
- domain-model.md
- assumptions.md

Todos esses arquivos devem estar em português do Brasil.
Cada arquivo deve conter estrutura durável como:
- descrição
- regras
- exemplos
- exceções
- dependências
- BDD relacionado
- contratos relacionados
- workflows relacionados
- ambiguidades
- placeholders de perguntas em aberto
- placeholders de histórico de mudança

Não invente conteúdo de negócio.
Crie estrutura para futuras definições reais e específicas do repositório.

Arquivos obrigatórios em Instructions/bdd/
Crie:
- README.md
- conventions.md
- example.feature

O README.md e conventions.md devem estar em português do Brasil.
O example.feature pode usar Gherkin, mas a explicação ao redor deve estar em português do Brasil.

Esses arquivos devem explicar:
- quando BDD deve ser usado
- quando BDD não é necessário
- como organizar cenários
- como cenários se relacionam com regras de negócio
- como mudanças em BDD se propagam
- como cenários devem ser nomeados

O example.feature deve ser válido, genérico e agnóstico de domínio.

Arquivos obrigatórios em Instructions/contracts/
Crie:
- README.md
- openapi.yaml
- asyncapi.yaml
- schemas/example.schema.json
- examples/valid-example.json
- examples/invalid-example.json

O README.md deve estar em português do Brasil.
Os arquivos formais podem usar a sintaxe natural do formato, mas suas descrições auxiliares devem estar em português do Brasil.

Esses arquivos devem explicar:
- quando contratos devem ser criados ou atualizados
- quando contratos não são necessários
- como contratos se relacionam com regras de negócio
- como contratos se relacionam com BDD
- como mudanças em contratos se propagam
- como contratos guiam implementação

Os exemplos de contrato devem ser placeholders genéricos válidos.

Arquivos obrigatórios em Instructions/glossary/
Crie:
- ubiquitous-language.md

Esse arquivo deve estar em português do Brasil e deve suportar:
- termo
- definição
- sinônimos permitidos
- termos ambíguos proibidos
- contexto
- exemplos
- notas
- futuras adições

Arquivos obrigatórios em Instructions/decisions/
Crie:
- README.md
- adr-template.md

Esses arquivos devem estar em português do Brasil e devem explicar:
- quando registrar uma decisão
- como registrar contexto, decisão, trade-off e consequência
- como decisões se relacionam com arquitetura e negócio

Arquivos obrigatórios em Instructions/snippets/
Crie:
- README.md
- canonical-snippets.md

Esses arquivos devem estar em português do Brasil.

Instructions/snippets/README.md deve explicar:
- quando um trecho fornecido pelo usuário deve ser tratado como snippet normativo
- quando um trecho é apenas exemplo
- como snippets canônicos influenciam implementações futuras
- como mudanças em snippets canônicos devem ser tratadas
- que snippets canônicos não devem ser reescritos livremente

Instructions/snippets/canonical-snippets.md deve conter estrutura para registrar snippets canônicos, com:
- id
- data
- título
- intenção
- resumo da instrução do usuário
- classificação
- escopo
- arquivos ou contextos de destino
- regra de preservação
- adaptações mínimas permitidas
- artefatos relacionados
- conteúdo do snippet

Escreva explicitamente que:
- esse arquivo pode armazenar referências canônicas fornecidas pelo usuário
- snippets ali registrados devem ser respeitados em futuras implementações
- alterações relevantes nesses snippets exigem nova instrução explícita ou conflito técnico devidamente reportado

Arquivos obrigatórios de dúvidas e premissas
Crie:
- open-questions.md
- assumptions-log.md

Esses arquivos devem estar em português do Brasil.

open-questions.md deve conter duas seções ativas:
- Dúvidas Ativas
- Ambiguidades Ativas

Cada item deve conter estrutura com:
- id
- data
- resumo da solicitação de origem
- dúvida ou ambiguidade
- por que isso importa
- artefatos impactados
- bloqueante ou não bloqueante
- status
- premissas relacionadas

Escreva explicitamente que:
- esse arquivo deve conter apenas dúvidas e ambiguidades ainda abertas
- dúvidas ou ambiguidades resolvidas devem ser removidas da lista ativa
- a resolução deve ser refletida nos arquivos definitivos do repositório
- se necessário, a resolução pode ser resumida em histórico apropriado, mas não mantida como pendência aberta

assumptions-log.md deve conter estrutura para premissas ativas, com:
- id
- data
- premissa
- motivo
- escopo
- artefatos impactados
- nível de risco
- precisa de confirmação posterior
- status de resolução

Escreva explicitamente que:
- esse arquivo deve conter apenas premissas ainda ativas ou ainda não resolvidas
- premissas confirmadas devem ser consolidadas na governança definitiva e removidas do log ativo quando apropriado
- premissas invalidadas devem ser removidas ou marcadas como descartadas e não permanecer como regra ativa

Requisitos do README.md
Crie um README.md em português do Brasil que explique claramente:
- a finalidade deste sistema de governança
- que o bootstrap é genérico apenas como inicialização
- que o repositório em si se torna específico por meio das definições acumuladas
- que solicitações em linguagem natural são suficientes
- que a governança é consultada e atualizada antes da implementação quando necessário
- que governança técnica e governança de negócio são diferentes
- que rules, Instructions, BDD, contratos, glossário, decisões, snippets canônicos, dúvidas e premissas têm papéis distintos
- que BDD e contratos são importantes, mas não obrigatórios para toda mudança
- que dúvidas relevantes devem ser registradas e respondidas antes de implementação insegura
- que snippets normativos explicitamente exigidos pelo usuário devem ser preservados na íntegra
- que exemplos enviados pelo usuário podem ser interpretados e adaptados ao contexto
- que o trabalho futuro deve ser governado pelos arquivos criados agora

Regra crítica
Não apenas crie arquivos.
Escreva conteúdo forte o suficiente para que esses arquivos governem ativamente o comportamento futuro do assistente neste repositório.

Idioma obrigatório
- Todas as instruções, explicações, regras, documentação, conteúdo de governança, conteúdo de rules, conteúdo de skills, conteúdo de hooks, README e arquivos em Instructions devem ser escritos em português do Brasil.
- Os nomes dos arquivos e pastas podem permanecer em inglês.
- Arquivos formais como YAML, JSON, SQL, schemas, exemplos de contrato e trechos de código podem usar a sintaxe natural do formato, mas toda explicação e texto auxiliar devem estar em português do Brasil.

Entrega
Ao final:
- mostre a árvore de arquivos criada
- resuma o propósito operacional de cada grupo de arquivos
- confirme que os arquivos gerados agora contêm regras, workflows, prioridades, tratamento de ambiguidades, tratamento de snippets normativos e comportamento de repositório suficientes para governar futuras interações em linguagem natural
