# Termo de Abertura do Projeto

## Módulo de Inscrição em Disciplinas

| Campo | Informação |
|---|---|
| **Versão** | 1.6 — marcos na semana letiva seguinte à aula prática extra |
| **Data** | 28/09/2026 |
| **Patrocinador** | Prof. Diogo Mendonça |
| **Gerente do projeto** | GPTI-1, aluno da disciplina de GPTI (Gerência de Projetos de TI). Presta contas do plano inteiro ao patrocinador. |
| **Equipe de gestão** | GPTI-1 a GPTI-4 |
| **Duração estimada** | 3 meses |
| **Equipe prevista** | 8 alunos: 4 da disciplina de Programação Web (PSW) e 4 da disciplina de GPTI; dedicação estimada de 5 horas semanais por pessoa |

## 1. Propósito e justificativa

Este termo autoriza o início de um projeto acadêmico de desenvolvimento de um protótipo de módulo digital para inscrição em disciplinas. Segundo o processo conhecido pelos alunos, as inscrições são apoiadas por planilhas e documentos em papel, o que demanda trabalho manual, gera retrabalho e limita a automação. A solução pretende centralizar as solicitações, permitir que estudantes façam a inscrição online e apoiar, futuramente, as equipes administrativas no acompanhamento do processo. O diagnóstico e as regras ainda não foram validados oficialmente pela instituição.

O projeto será também uma experiência de aprendizagem prática: os quatro alunos de PSW definirão e desenvolverão o escopo inicial do produto e os quatro alunos de GPTI validarão esse escopo e conduzirão a gestão do projeto. Os oito participantes são alunos da instituição e conhecem o processo de matrícula por vivência própria. Desenvolverão conhecimentos em **React e JavaScript no frontend** e **JavaScript, Express e MongoDB no backend**, aplicando-os em um protótipo pensado para um uso institucional futuro. A dimensão pedagógica deve ser considerada no planejamento, nas revisões técnicas e na definição realista das entregas.

O produto futuro deverá prever autenticação de alunos por meio do provedor OAuth da instituição e consulta a dados do sistema acadêmico. **A integração efetiva com esses sistemas não faz parte deste escopo.** Para o protótipo, a equipe fornecerá endpoints acadêmicos simulados com `json-server` (incluindo dados fictícios de ingresso, CR e disciplinas concluídas) e testará o fluxo de login somente por mock OAuth, sem credenciais ou dados reais. A integração efetiva será considerada em uma etapa/projeto futuro, sujeito a autorização institucional.

## 2. Objetivos do projeto

Os objetivos abaixo são do protótipo. Quem mede é a equipe GPTI, com ciência do patrocinador, na demonstração da semana 12. A redução de posto administrativo do caso de negócio é hipótese de uma implantação futura, não critério de sucesso deste termo.

- Um aluno fictício consulta a oferta, monta o pedido, submete e vê o status, sem formulário em papel. O status separa pedido de inscrição efetivada.
- Nos casos documentados no dicionário da EAP, a vaga sai na ordem período correto, ingresso mais antigo, CR maior e identificador. Pré-requisito ausente não gera efetivação. Vaga efetivada na fase anterior permanece nas fases seguintes.
- A AV1, com termo, caso de negócio e plano, é aceita na semana 8. O termo de encerramento e as lições aprendidas são aceitos na semana 12.
- O login é demonstrado por mock e os dados acadêmicos saem do `json-server`. Nenhuma chamada ao provedor ou ao sistema acadêmico real ocorre na demonstração.

## 3. Escopo de alto nível

### Incluído

- Levantamento e validação das regras necessárias para o fluxo inicial de inscrição.
- Interface frontend construída com React e JavaScript.
- Backend em JavaScript com Express e persistência em MongoDB.
- Uso de `json-server` como backend simulado para a demonstração integrada do frontend no primeiro marco.
- Integração do frontend com a API do backend próprio, Express/MongoDB, no marco final.
- Endpoints simulados do sistema acadêmico fornecidos pela equipe via `json-server`, incluindo data de ingresso, CR e histórico de disciplinas concluídas.
- Demonstração de autenticação por mock OAuth, sem conexão ao provedor institucional.
- Fluxos de consulta, envio e acompanhamento de inscrições dentro do escopo validado.
- Testes funcionais, documentação técnica essencial e demonstração das entregas.

### Fora do escopo inicial

- Substituição ou reescrita do sistema institucional de autenticação.
- Integração efetiva com o provedor OAuth institucional ou com o sistema acadêmico existente; ambas ficam para escopo futuro.
- Alteração das regras acadêmicas, da oferta de disciplinas ou dos critérios de matrícula.
- Migração abrangente de dados históricos.
- Integrações com outros sistemas não identificados e priorizados.
- Garantia de implantação em produção ao fim do terceiro mês: o projeto visa entregar uma versão integrada e demonstrável; produção depende de aprovação institucional, segurança, infraestrutura, operação e aceite das áreas responsáveis.

## 4. Abordagem técnica e de aprendizagem

O desenvolvimento será incremental, com evolução do protótipo integrado à implementação completa:

1. **Frontend:** React e JavaScript, inicialmente consumindo endpoints simulados por `json-server`.
2. **Backend:** API em JavaScript com Express, regras de negócio e acesso a MongoDB.
3. **Integração:** substituição do serviço simulado pela API real, testes de contrato e de fluxo completo.
4. **Serviços externos simulados:** endpoints acadêmicos fornecidos por `json-server` para dados fictícios e fluxo OAuth inteiramente mockado. Não haverá integração efetiva com os sistemas institucionais durante este projeto. A integração futura exigirá levantamento e autorização próprios.

Como a equipe está aprendendo as tecnologias, o plano deve reservar tempo para capacitação, pareamento, revisão de código e correção de defeitos. A equipe deve priorizar uma fatia funcional pequena e segura; funcionalidades secundárias poderão ser reduzidas ou postergadas se o aprendizado ou as dependências externas pressionarem o prazo.

## 5. Marcos e entregas

| Marco | Prazo previsto | Entregáveis e critérios de aceite preliminares |
|---|---:|---|
| **M1 — Frontend dos fluxos priorizados, com serviços simulados** | Semana letiva 8: GPTI em 05/10/2026 e PSW em 06/10/2026 | Escopo inicial definido pelos alunos de PSW e validado pelos alunos de GPTI; fluxos de frontend priorizados implementados em React; navegação e validações básicas demonstráveis; integração com `json-server` para dados acadêmicos simulados; autenticação demonstrada por mock OAuth; limitações dos mocks documentadas. O aceite do marco será registrado pela equipe de GPTI com ciência do patrocinador. |
| **M2 — Sistema integrado ao backend próprio** | Semana letiva 12: PSW em 10/11/2026; aceite de GPTI em 30/11/2026 | Frontend conectado à API Express desenvolvida pelo projeto; persistência em MongoDB; endpoints acadêmicos permanecem simulados via `json-server` e OAuth permanece mockado; fluxos prioritários executados de ponta a ponta; testes, documentação e demonstração final. Não haverá integração efetiva com sistemas institucionais. O aceite do marco será registrado pela equipe de GPTI com ciência do patrocinador. |

Os marcos acima são os da iniciação, com a data corrigida no planejamento. A aula de 28/09 e 29/09 foi prática extra e não conta como semana do projeto. Cada marco andou uma semana letiva. O esforço não mudou. As datas, a folga e o caminho crítico estão na linha de base de prazo do plano.

## 6. Requisitos de alto nível e critérios gerais de sucesso

- O protótipo deve permitir demonstrar o acesso simulado, consultar opções provisórias de inscrição, enviar uma solicitação e apresentar um status compreensível.
- Os dados persistidos devem ser validados e acessados pelo backend; o frontend não deve conectar diretamente ao MongoDB.
- A primeira entrega deve demonstrar os fluxos do frontend sem depender do backend definitivo, usando dados simulados pelo `json-server`.
- A entrega final deve substituir o mock do backend próprio pela API Express/MongoDB do projeto; os endpoints acadêmicos e o OAuth permanecerão simulados. Deve demonstrar persistência e tratamento dos principais erros dos fluxos implementados.
- O aceite de cada pacote está no dicionário da EAP. As regras continuam hipóteses do protótipo: a secretaria acadêmica não as valida nesta fase.
- O êxito do projeto será avaliado pela entrega dos marcos, pelo atendimento aos fluxos priorizados, pelo aceite interno da equipe de GPTI e pelo aprendizado técnico documentado. A validação com usuários e áreas institucionais fica para uma etapa posterior.

### Critérios de encerramento e cancelamento

O projeto termina na semana 12, quando a equipe GPTI registra o aceite do M2 ou a lista do que não passou, e o patrocinador dá ciência. Encerrar com limitação conhecida é término, não fracasso escondido.

O patrocinador cancela o projeto, ou o encerra antes do M2, se ocorrer uma destas condições:

- A demonstração da regra de alocação não cabe nas 24 h de programação reservadas e o patrocinador não aprova um corte de escopo.
- O patrocinador retira a autorização.
- Uma premissa essencial cai e não há substituto dentro do prazo, por exemplo a equipe deixar de ter ambiente para executar o protótipo.

Cancelar cedo, nesse caso, é decisão de governança. Não é meta do projeto.

## 7. Premissas e restrições

### Premissas

- Os oito participantes são alunos da instituição e conhecem o processo de matrícula; esse conhecimento será usado para elaborar hipóteses iniciais de requisitos.
- O patrocinador, Prof. Diogo Mendonça, acompanhará o projeto e receberá as demonstrações dos marcos.
- Os participantes terão acesso às ferramentas, repositório e ambiente de desenvolvimento necessários.
- As regras de inscrição da primeira versão poderão ser reduzidas a um conjunto prioritário que caiba no prazo.
- Serão usados dados fictícios criados pela equipe; não se presume fornecimento de dados ou recursos institucionais.

### Restrições

- Duração-alvo de três meses e dedicação parcial prevista de cinco horas semanais por participante.
- A equipe estará em processo de aprendizagem de React, JavaScript, Express e MongoDB; produtividade inicial pode ser inferior à de uma equipe experiente.
- `json-server` é exclusivamente uma solução de simulação dos endpoints acadêmicos e, no primeiro marco, do backend do frontend; não deverá ser tratado como backend de produção.
- Não haverá envolvimento da secretaria acadêmica nem de outras áreas da instituição na definição ou validação inicial do escopo; os alunos de PSW elaboram o escopo e os alunos de GPTI fazem sua validação interna.
- A equipe não está autorizada, por este termo, a acessar sistemas, credenciais, dados ou infraestrutura institucional; a integração efetiva com OAuth e sistema acadêmico está explicitamente fora deste escopo.
- A implantação real depende de revisão de segurança, privacidade, infraestrutura, acessibilidade, operação e aprovação institucional, podendo ficar fora do prazo deste projeto.
- Endpoints de dados acadêmicos serão simulados com `json-server`, e OAuth será mockado. O protocolo, os contratos e as permissões dos serviços reais só serão levantados em uma etapa futura de integração.

## 8. Governança e responsabilidades

### Stakeholders

| Stakeholder | Interesse ou responsabilidade | Participação nesta etapa |
|---|---|---|
| **Prof. Diogo Mendonça — patrocinador** | Patrocinar o projeto acadêmico, acompanhar os marcos e decidir sobre mudanças relevantes de escopo e prazo | Ativo: recebe as demonstrações e dá ciência dos aceites internos |
| **4 alunos de GPTI — Gerência de Projetos de TI** | Planejar e acompanhar o projeto, validar internamente o escopo proposto por PSW e registrar decisões e aceites | Ativos: equipe de gestão |
| **4 alunos de PSW — Programação Web** | Definir o escopo funcional inicial e desenvolver a solução como atividade de aprendizagem | Ativos: equipe de produto e desenvolvimento |
| **Estudantes da instituição — usuários finais potenciais** | Realizar inscrições online e consultar o status; são beneficiários pretendidos do módulo | Não serão consultados formalmente nesta fase; os alunos da equipe usarão sua experiência para elaborar hipóteses de requisitos |
| **Secretaria acadêmica — responsável pelo processo atual** | Conhece e opera o processo oficial de matrícula; deverá validar regras e adequação operacional antes de eventual uso real | Sem participação inicial; stakeholder externo ao trabalho desta etapa, a envolver em fase futura |
| **Responsável institucional pelo provedor OAuth / equipe de TI** | Administrar o serviço de identidade e informar documentação, ambiente de teste, fluxo OAuth/OIDC, escopos, claims e requisitos de integração | Sem participação inicial; dependência técnica e stakeholder a envolver antes de integração real |
| **Instituição — proprietária do processo, dos dados e da infraestrutura** | Avaliar segurança, privacidade, operação, infraestrutura e autorização para eventual implantação | Sem participação inicial; deverá aprovar separadamente qualquer acesso a sistemas/dados e uso em produção |

Os stakeholders identificados como sem participação inicial não foram consultados nem aprovaram os requisitos. A lista registra partes interessadas potenciais e dependências para uma etapa futura; não implica compromisso de disponibilidade ou autorização.

### Papéis e responsabilidades

| Papel | Responsabilidades principais | Designação |
|---|---|---|
| Patrocinador | Patrocinar o projeto, acompanhar demonstrações e decidir sobre mudanças relevantes de escopo ou prazo | Prof. Diogo Mendonça |
| Gerente do projeto | Prestar contas do plano ao patrocinador; conferir pedidos de mudança contra a EAP; coordenar a equipe de gestão | GPTI-1 |
| Equipe de gestão (GPTI) | Planejar e acompanhar prazo, escopo, riscos, comunicação e marcos; validar o escopo proposto por PSW; registrar aceite interno das entregas | 4 alunos de GPTI — Gerência de Projetos de TI |
| Equipe de produto e desenvolvimento (PSW) | Propor o escopo funcional inicial e implementar frontend, backend, testes e documentação conforme prioridades acordadas | 4 alunos de Programação Web |
| Equipe total do projeto | Participar das atividades do projeto com dedicação estimada de 5 h/semana por aluno | 8 alunos, já incluindo os quatro de GPTI e os quatro de PSW |

Os alunos de PSW elaborarão a proposta inicial de escopo com base no conhecimento que têm do processo de matrícula. Os alunos de GPTI revisarão e validarão essa proposta para fins do projeto. A validação é interna e acadêmica, não representa aprovação oficial da secretaria ou da instituição. A equipe de GPTI manterá a lista priorizada de trabalho, riscos, decisões e demonstrações; mudanças relevantes serão submetidas ao patrocinador.

## 9. Riscos iniciais e respostas

| Risco | Impacto potencial | Resposta inicial |
|---|---|---|
| Curva de aprendizagem maior que a prevista | Atraso ou redução de funcionalidades | Reservar tempo para estudo e revisão; priorizar o fluxo mínimo viável; revisar o plano a cada demonstração |
| Regras de inscrição inferidas sem validação oficial | Implementação divergente do processo institucional e retrabalho futuro | Registrar as regras como hipóteses; basear o protótipo na experiência dos alunos; submeter a validação institucional em etapa futura antes de uso real |
| Mocks divergentes dos contratos dos sistemas institucionais | Retrabalho em uma futura integração efetiva | Documentar payloads e contratos simulados e registrar que deverão ser revistos com as equipes institucionais em fase futura |
| Requisitos de segurança e privacidade identificados tardiamente | Retrabalho ou impedimento de implantação | Usar dados fictícios, evitar sistemas institucionais e tratar revisão de segurança/privacidade como condição para uma etapa futura de implantação |
| Baixa disponibilidade dos participantes ou dedicação diferente da prevista | Entregas incompletas | Monitorar disponibilidade semanal, dividir tarefas pequenas e ajustar o escopo antes dos marcos |
| Mock incompatível com a futura integração institucional | Retrabalho em projeto posterior | Manter contratos de mock documentados e limitar afirmações de compatibilidade até validação com os responsáveis pelos sistemas |
| Expectativa de produção ao fim do prazo | Uso prematuro de software não aprovado | Comunicar que a entrega é uma versão acadêmica demonstrável, sem validação institucional; exigir aprovações separadas para qualquer uso real |

## 10. Estimativa econômica e financiamento

Na iniciação, a ordem de grandeza foi **520 h** e **R$ 9.800**, com faixa esperada de −25% a +75%. O planejamento revisou esse número para **R$ 8.388,80**: 360 h de atividades, 56 h de contingência e reserva gerencial de 7%. A revisão fica 14,4% abaixo do ponto da iniciação e dentro da faixa. O detalhe da conta está no caso de negócio e no plano. O valor abaixo é a linha de base de planejamento, não uma correção retroativa do caso de negócio. A reserva utiliza as 24 h livres de PSW e 32 das 36 h livres de GPTI; 8 h do apoio GPTI às respostas técnicas cobrem preparação de dados, critérios de aceite, testes e documentação, sem substituir programação. O calendário fica com apenas 4 h livres em GPTI e nenhuma folga PSW; riscos que exijam desenvolvimento adicional acima da reserva técnica demandarão redução de escopo ou replanejamento. **Os alunos não serão remunerados pelo projeto; portanto, o desembolso efetivo previsto para pagamentos à equipe é R$ 0,00.** O calendário abaixo é uma distribuição hipotética do custo para modelagem, não uma autorização nem obrigação de pagamento. A estimativa refere-se ao protótipo com endpoints acadêmicos simulados e OAuth mockado; não contempla o custo de uma futura integração efetiva.

Para fins do exercício, o custo simulado é distribuído igualmente entre os dois marcos, associando cada parcela à entrega e ao aceite interno correspondente:

| Marco e gatilho da parcela simulada | Prazo | Parcela simulada | Desembolso efetivo com a equipe |
|---|---:|---:|---:|
| **M1 — Frontend dos fluxos priorizados com `json-server`**: após demonstração e aceite interno pela equipe de GPTI, com ciência do patrocinador | Semana letiva 8: GPTI 05/10/2026 e PSW 06/10/2026 | **R$ 4.194,40 (50%)** | **R$ 0,00 — não há pagamento aos alunos** |
| **M2 — Sistema integrado ao backend próprio Express/MongoDB**: após demonstração final e aceite interno pela equipe de GPTI, com ciência do patrocinador; serviços acadêmicos continuam mockados e OAuth permanece simulado | Semana letiva 12: PSW 10/11/2026; aceite GPTI 30/11/2026 | **R$ 4.194,40 (50%)** | **R$ 0,00 — não há pagamento aos alunos** |
| **Total do projeto** | **3 meses** | **R$ 8.388,80 (100%)** | **R$ 0,00 de pagamento à equipe** |

O rateio igual de 50% por marco é uma convenção didática de planejamento financeiro e não corresponde à distribuição exata do esforço entre as fases. A conferência do plano dá 224 h até o fim da semana 8 e 136 h nas semanas 9 a 12. Não constitui faturamento, bolsa, salário ou transferência financeira. A estimativa exclui quaisquer custos efetivos de infraestrutura, licenças, transporte, supervisão, operação ou contratação de terceiros. Como não haverá participação institucional nesta etapa inicial, nenhum desembolso institucional está solicitado ou aprovado. Se surgirem custos reais, deverão ser avaliados e autorizados separadamente pelo patrocinador e pela instituição antes de serem incorridos.

## 11. Autoridade e aprovação

A aprovação deste termo autoriza o início do planejamento detalhado, levantamento de requisitos e desenvolvimento da primeira versão dentro das premissas acima. Não autoriza o uso de dados reais em ambientes não aprovados nem a implantação em produção.

| Aprovação | Nome | Assinatura | Data |
|---|---|---|---|
| Patrocinador | Prof. Diogo Mendonça |  |  |
| Representante da equipe GPTI |  |  |  |
| Representante da equipe PSW |  |  |  |
