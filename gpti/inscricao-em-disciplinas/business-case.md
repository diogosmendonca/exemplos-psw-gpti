# Business Case — Módulo de Inscrição em Disciplinas

**Versão:** 1.1 — iniciação; a seção 12.1 registra a revisão feita no planejamento  
**Data:** 28/09/2026

## 1. Resumo executivo

Propõe-se desenvolver um protótipo acadêmico de módulo digital de inscrição em disciplinas para demonstrar uma alternativa ao processo hoje realizado com planilhas e documentos em papel. O processo atual exige trabalho manual e retrabalho e oferece pouca automação. Neste escopo, os endpoints do sistema acadêmico serão simulados com `json-server` e o login institucional será demonstrado por mock OAuth; não haverá integração efetiva nem implantação em produção. A integração institucional e a realização dos benefícios operacionais poderão ser avaliadas em uma etapa futura.

A iniciativa busca demonstrar como inscrições poderiam ser organizadas digitalmente, reduzindo tarefas repetitivas e melhorando o acompanhamento do processo. A viabilidade de uso institucional e dos benefícios financeiros dependerá de validação, integração e implantação em etapa futura.

## 2. Problema e oportunidade

O processo atual de inscrição depende de planilhas e papel. Esse modelo pode exigir transcrição e conferência manual de informações, dificultar o acompanhamento das solicitações e aumentar o risco de inconsistências. Além disso, a falta de automação gera retrabalho para estudantes e equipes responsáveis.

A digitalização do processo é uma oportunidade para centralizar as inscrições, automatizar etapas adequadas e oferecer um fluxo mais claro aos envolvidos.

## 3. Objetivos

Estes são os objetivos da iniciativa. O protótipo de 12 semanas demonstra o caminho; os objetivos só se realizam em uma implantação futura, que não faz parte deste projeto. Os objetivos do protótipo estão no termo de abertura.

- Disponibilizar um canal digital para inscrição em disciplinas.
- Demonstrar o fluxo de login por mock OAuth e consumir endpoints acadêmicos simulados, deixando a integração institucional efetiva para escopo futuro.
- Reduzir a necessidade de controles paralelos em papel e planilhas.
- Diminuir tarefas manuais e retrabalho no processamento das inscrições.
- Melhorar a visibilidade do status das inscrições para estudantes e equipes responsáveis.

## 4. Solução proposta

Desenvolver um protótipo que permita ao estudante demonstrativo consultar opções de inscrição, registrar sua solicitação e acompanhar seu status. Os dados acadêmicos serão fornecidos por endpoints simulados com `json-server`, e a autenticação será mockada. O sistema demonstrará fluxos de consulta e processamento conforme regras provisórias elaboradas pela equipe.

O desenho poderá considerar a futura integração com o OAuth e o sistema acadêmico existentes, mas nenhum endpoint real, credencial ou dado institucional será acessado neste projeto. Contratos, permissões e viabilidade de integração precisam ser tratados com a instituição em etapa posterior.

## 5. Escopo inicial

### Incluído

- Fluxo digital de inscrição em disciplinas.
- Demonstração de autenticação por mock OAuth e consumo de endpoints acadêmicos simulados com `json-server`.
- Consulta e acompanhamento do status da solicitação.
- Visão operacional para as equipes responsáveis, a definir durante o levantamento de requisitos.
- Registro das informações necessárias para processar as inscrições, conforme regras provisórias definidas para o protótipo e ainda não aprovadas pela instituição.

### Fora do escopo inicial

- Integração efetiva com o provedor OAuth institucional e com o sistema acadêmico existente (etapa futura).
- Alteração de regras acadêmicas ou de oferta de disciplinas.
- Migração ampla de dados históricos, salvo necessidade identificada e aprovada.
- Uso de credenciais ou dados reais e implantação em produção.

## 6. Benefícios esperados

- Menos trabalho manual e menor necessidade de redigitação de dados.
- Redução de retrabalho e de inconsistências causadas por controles descentralizados.
- Processo mais simples e rastreável para estudantes e equipes.
- Possibilidade de realizar a inscrição online sem deslocamento até a instituição, economizando tempo e custos de transporte para os estudantes.
- Menor dependência de formulários físicos e de entregas presenciais, com potencial para reduzir filas, dúvidas sobre documentação e inscrições refeitas.
- Mais clareza para consultar as informações e acompanhar o andamento da solicitação, conforme as funcionalidades definidas para o módulo.
- Melhor disponibilidade de informações sobre o andamento das inscrições.
- Base para futuras melhorias e automações do processo acadêmico.

Os benefícios são expectativas a validar após o levantamento do processo atual e a definição de indicadores e metas.

## 7. Alternativas consideradas

1. **Manter o processo atual:** não requer desenvolvimento imediato, mas mantém as limitações, o esforço manual e o retrabalho existentes.
2. **Melhorar planilhas e formulários:** pode organizar parte do fluxo com menor mudança inicial, mas tende a manter controles fragmentados e limitações de automação e rastreabilidade.
3. **Desenvolver o protótipo proposto:** requer esforço de análise e desenvolvimento acadêmico e demonstra a possibilidade de centralizar e automatizar o processo. Não substitui a decisão nem o investimento futuro para integração, implantação e operação institucional.

A recomendação nesta etapa é desenvolver o protótipo. Uma decisão sobre solução institucional dependerá de validação com as áreas responsáveis e de análise separada de viabilidade técnica, operacional e financeira.

## 8. Custos e recursos

Há uma estimativa econômica simulada de mão de obra na seção 12, relativa ao protótipo. Não é orçamento aprovado nem custo de uma solução pronta para operação. Uma futura integração e implantação deverá considerar, no mínimo:

- Levantamento e validação dos processos e regras acadêmicas.
- Desenvolvimento do protótipo com serviços simulados; uma integração institucional futura precisará de estimativa própria.
- Infraestrutura, segurança, testes e implantação.
- Treinamento, comunicação e suporte aos usuários.
- Manutenção e evolução após a implantação.

A estimativa dependerá da equipe disponível, das tecnologias adotadas e da complexidade das regras e da integração.

## 9. Riscos e dependências

| Risco ou dependência | Possível impacto | Ação inicial |
|---|---|---|
| Regras de inscrição incompletas ou divergentes | Escopo inadequado ou necessidade de retrabalho | Registrar as regras do protótipo como hipóteses; validar com as áreas acadêmicas em etapa futura, antes de qualquer uso real |
| Contratos dos mocks divergirem dos sistemas institucionais reais | Retrabalho em uma etapa futura | Documentar endpoints e payloads simulados; validar contratos com os responsáveis institucionais antes de uma integração futura |
| Baixa adesão de estudantes ou equipes | Manutenção de processos paralelos | Na etapa de implantação, envolver representantes dos usuários, testar o fluxo e planejar comunicação e capacitação. Neste projeto, só demonstração com dados fictícios |
| Requisitos de segurança e privacidade não identificados | Exposição indevida de dados ou bloqueio da implantação | Usar só dados fictícios neste projeto; envolver as áreas responsáveis antes de qualquer implantação |
| Dados inconsistentes nos controles atuais | Dificuldade de transição e conferência | Definir se haverá carga de dados e estabelecer critérios de validação, se necessário |

## 10. Indicadores de sucesso

As metas devem ser definidas após a medição da situação atual. Indicadores possíveis:

- Percentual de inscrições realizadas pelo módulo.
- Tempo médio entre solicitação e processamento da inscrição.
- Volume de correções ou solicitações refeitas.
- Quantidade de etapas ou controles manuais no processo.
- Satisfação de estudantes e equipes responsáveis.
- Disponibilidade e taxa de sucesso da integração de autenticação.

## 11. Recomendação e próximos passos

Recomenda-se autorizar o protótipo acadêmico, com prazo de 12 semanas e a ordem de grandeza da seção 12. Orçamento e prazo de uma solução em produção ficam para decisão futura. O projeto deve:

1. Mapear o processo atual e seus principais pontos de retrabalho.
2. Levantar e validar regras, exceções e períodos de inscrição.
3. Identificar usuários, responsáveis e requisitos de acesso e privacidade.
4. Registrar que a integração efetiva com OAuth e sistema acadêmico está fora desta etapa; levantar suas condições em iniciativa futura com a instituição.
5. Definir requisitos priorizados, critérios de sucesso, estimativa de custo e cronograma.
6. Planejar validação institucional e piloto com usuários em etapa posterior, antes de qualquer implantação real.

**Decisão solicitada:** autorizar o protótipo descrito neste caso, formalizado no termo de abertura. A decisão de investimento em integração e produção é outra, posterior, e depende dos dados que este protótipo e a validação institucional produzirem.

## 12. Análise econômica preliminar (24 meses)

### 12.1 Premissas e referências de mercado

Esta é uma **simulação ilustrativa de iniciação**, em reais nominais, de 24 meses e quatro períodos semestrais. O ponto usado nos indicadores é **520 h** e **R$ 9.800**. Para uma ordem de grandeza, a faixa razoável é **−25% a +75%**: de 390 h a 910 h, ou de R$ 7.350 a R$ 17.150.

O planejamento do protótipo, em [plano-de-projeto.md](plano-de-projeto.md), revisou o esforço para **416 h** na linha de base e o orçamento total para **R$ 8.388,80**, incluída a reserva gerencial. Isso é **20% menos horas** e **14,4% menos custo** do que o ponto da iniciação. As duas diferenças cabem na faixa de −25%. Não se recalculam abaixo o VPL, a TIR, o ROI, o payback nem o índice benefício-custo: eles continuam o cenário de iniciação. Um investimento menor, mantidos os benefícios, não inverte a leitura desse cenário.

O protótipo com `json-server` e OAuth mockado não produz os benefícios financeiros modelados. Esses benefícios pressupõem uma solução integrada e em operação depois do mês 3, fora deste projeto. Valores de remuneração são referências de mercado, não proposta salarial nem custo contábil da instituição.

| Premissa | Valor adotado | Base e ressalvas |
|---|---:|---|
| Equipe de projeto | 8 alunos × 5 h/semana × 13 semanas | 520 horas no total, durante os 3 meses de desenvolvimento. São 65 h por aluno. A bolsa de estágio entra só como taxa-sombra; os alunos não são estagiários nem são pagos. |
| Bolsa de estágio em TI | R$ 2.450/mês | Média nacional publicada pelo Indeed para estagiário de TI, baseada em 117 salários informados, atualizada em 15/09/2026. Para estimar, normalizada à jornada de referência de estágio de 30 h/semana (6 h/dia) e rateada para as 5 h/semana dedicadas ao projeto. |
| Remuneração administrativa de referência | R$ 3.527/mês | Mediana mensal de remuneração total (anual ÷ 12) publicada para assistente administrativo pleno em 2026; usada apenas como proxy de salário-base para estimar o custo CLT de técnico administrativo pleno. Não é salário bruto-base confirmado e pode incluir outros componentes. A amostra tem 10 registros; substituir pelo salário-base da folha/CCT aplicável. |
| Jornada mensal produtiva administrativa | 168 h/mês | Conforme solicitado: 21 dias úteis × 8 h/dia. Usada apenas para expressar custo-hora. Não é divisor legal universal para todo contrato CLT; para o fluxo financeiro considera-se o custo mensal carregado do posto. |
| Encargos patronais estimados | 35,8% | Cenário de regime geral: INSS patronal 20% + RAT 2% (premissa média; varia de 1% a 3%) + terceiros 5,8% + FGTS 8%. Aplicados também às provisões anuais de 13º e férias. Regime tributário, FAP, CCT e natureza institucional podem alterar os encargos. |
| Provisões trabalhistas | 13,333 salários/ano | 12 salários (já incluem a remuneração do mês de férias) + 13º (1) + adicional de férias de 1/3 (0,333). Não se soma novamente um salário integral de férias, para evitar dupla contagem. Não inclui benefícios, vale-transporte, vale-refeição, provisão de multa rescisória ou custo de substituição. |
| Matrículas | 350 estudantes por semestre | Ponto médio da faixa informada de 300 a 400 alunos; assumida uma inscrição/formulário de uma folha por aluno. |
| Papel A4 | R$ 32,99 por resma de 500 folhas | Referência de preço varejista observada para papel Chamex A4; equivale a R$ 0,06598 por folha. Preço e disponibilidade variam por local e data. |
| Taxa de desconto de referência | 13,75% ao ano | Meta Selic fixada pelo Copom em 16/09/2026, conforme histórico oficial do Banco Central. Convertida para taxa mensal efetiva equivalente de aproximadamente 1,0794%. A Selic é referência macroeconômica, não substitui a taxa mínima de atratividade ou custo de capital definido pela instituição. |

Referências consultadas em 28/09/2026: [Indeed — bolsa de estagiário de TI no Brasil](https://br.indeed.com/career/estagi%C3%A1rio-de-ti/salaries), [Lei nº 11.788/2008 — estágio](https://www.planalto.gov.br/ccivil_03/_ato2007-2010/2008/lei/l11788.htm), [Salário Transparente — assistente administrativo pleno](https://salariotransparente.com.br/salarios/assistente-administrativo/pleno), [Contabilizei — cálculo do custo CLT por regime tributário](https://www.contabilizei.com.br/contabilidade-online/quanto-custa-um-funcionario-para-empresa/) e [Banco Central — histórico da meta Selic](https://www.bcb.gov.br/controleinflacao/historicotaxasjuros). O custo do papel segue a referência varejista de R$ 32,99 por resma consultada na seção anterior.

### 12.2 Investimento estimado

O Indeed informa bolsa média de R$ 2.450 por mês para estagiário de TI, mas não padroniza essa média pela mesma jornada em todas as vagas. Para tornar a conta comparável, adota-se como referência a jornada máxima usual da Lei do Estágio (30 h/semana) e calcula-se a proporção de 5 h/semana por participante. Assim, o custo estimado por hora de estágio é:

O fator $52/12$ converte semanas em uma média mensal: considera-se aproximadamente 52 semanas no ano divididas por 12 meses, resultando em $4,33$ semanas por mês. Portanto, uma jornada de 30 h/semana corresponde a cerca de 130 h/mês ($30 \times 52/12$). Dividindo a bolsa mensal por essas horas, obtém-se o valor-hora estimado. Para cada integrante que dedica 5 h/semana, a estimativa é de $5 \times 52/12 = 21,67$ h/mês. No período do projeto, usamos 13 semanas como aproximação de três meses; assim, cada integrante contribui com 65 h e a equipe de oito pessoas totaliza 520 h. O fator é uma média de conversão, não a afirmação de que todo mês tenha exatamente 4,33 semanas.

$$
R\$\ 2.450 \div (30 \times 52/12) = R\$\ 18,846/\text{h}
$$

Assim, o custo econômico estimado do desenvolvimento é:

$$
8 \times 5\ \text{h/semana} \times 13\ \text{semanas} \times R\$\ 18,846/\text{h} = R\$\ 9.800,00
$$

Para o fluxo mensal da iniciação, o investimento de R$ 9.800 é distribuído igualmente pelos meses 1 a 3: **R$ 3.266,67 por mês**. A revisão de planejamento, R$ 8.388,80, não substitui esta série. Ela mostra que o protótipo acadêmico coube abaixo do ponto inicial, dentro da margem da fase. A bolsa de estágio é apenas referência de custo de oportunidade; os alunos não serão pagos efetivamente. A estimativa não inclui auxílio-transporte obrigatório no estágio não obrigatório, seguro contra acidentes pessoais, eventual recesso remunerado, supervisão/termo de compromisso, gestão, infraestrutura, licenças, treinamento, manutenção, suporte ou integração efetiva futura; logo, não representa o orçamento completo para uma solução em produção. A jornada de 5 h/semana é uma premissa de rateio do esforço no projeto.

### 12.3 Benefícios estimados

**Custo administrativo evitado:** o processo passaria de dois funcionários em dedicação integral durante um mês para um. A economia presumida é, portanto, o custo CLT carregado de um funcionário-mês por período de matrícula.

Para estimar um custo comparável, a remuneração total de referência de R$ 3.527 é tratada como proxy do salário-base. O custo carregado mensal é calculado anualizando 13º e o adicional de férias de 1/3 (sem somar novamente a remuneração do mês de férias, já incluída nos 12 salários) e adicionando as contribuições patronais estimadas:

$$
R\$\ 3.527 \times \frac{12+1+1/3}{12} \times (1+0,358) = R\$\ 5.321,85/\text{mês}
$$

Com o divisor produtivo solicitado de 168 horas, o custo-hora carregado aproximado é **R$ 31,68/h**. Para o fluxo de caixa, usa-se o valor de um mês carregado (**R$ 5.321,85**) e não o custo-hora.

**Papel evitado:** com 350 inscrições de uma folha por estudante, o custo estimado é:

$$
350 \times (R\$\ 32,99 \div 500) = R\$\ 23,09\ \text{por semestre}
$$

Em quatro períodos, isso representa aproximadamente R$ 92,37. A faixa de 300–400 estudantes equivale a cerca de R$ 19,79–R$ 26,39 por semestre, sob a hipótese de uma folha por inscrição. Impressão, toner, formulários adicionais, armazenamento e descarte não foram monetizados por falta de dados.

O benefício total modelado é **R$ 5.344,94 por semestre** (R$ 5.321,85 de custo CLT evitado mais R$ 23,09 de papel), ou **R$ 21.379,78 em 24 meses**.

**Benefícios intangíveis para estudantes e equipe (não monetizados):** a inscrição online pode evitar deslocamentos até a instituição, reduzir o tempo gasto com entrega e conferência de formulários e facilitar o acompanhamento do pedido. Um fluxo digital bem definido também pode diminuir erros de preenchimento, pedidos incompletos e retrabalho, além de reduzir filas e tornar o processo mais previsível. Para a equipe administrativa, a centralização das solicitações pode facilitar a consulta e o acompanhamento dos casos. Esses efeitos são benefícios esperados, não entram nos cálculos de VPL, TIR, ROI ou índice benefício-custo acima e devem ser avaliados após a implantação com dados de uso, volume de correções, tempo de atendimento e satisfação dos estudantes e servidores.

> **Distinção importante:** o custo administrativo só representa economia de caixa se a instituição realmente evitar ou reduzir esse gasto (por exemplo, vaga não reposta, contratação temporária ou hora extra). Se os dois funcionários forem mantidos e apenas realocados, o benefício de mão de obra é capacidade liberada, não redução orçamentária; nesse caso, os indicadores financeiros devem ser recalculados com a economia direta de papel e outros custos efetivamente evitados.

### 12.4 Fluxo de caixa-base

O investimento é lançado nos meses 1–3; os benefícios são lançados nos meses 6, 12, 18 e 24. Os demais meses têm fluxo incremental zero. Valores em reais.

| Mês/período | Investimento | Benefício | Fluxo líquido |
|---|---:|---:|---:|
| 1, 2 e 3 (cada mês) | -R$ 3.266,67 | R$ 0,00 | -R$ 3.266,67 |
| 6, 12, 18 e 24 (cada período) | R$ 0,00 | R$ 5.344,94 | R$ 5.344,94 |
| **Total nominal em 24 meses** | **-R$ 9.800,00** | **R$ 21.379,78** | **R$ 11.579,78** |

### 12.5 Indicadores financeiros

| Indicador | Resultado-base | Interpretação |
|---|---:|---|
| VPL, à taxa mensal equivalente da Selic | **R$ 8.654,73** | Positivo: valor presente dos benefícios estimados supera o investimento. |
| TIR | **6,996% ao mês** (aprox. **125,13% ao ano efetivo**) | Superior à taxa de desconto de referência (1,0794% ao mês, equivalente à meta Selic de 13,75% a.a.). |
| ROI simples em 24 meses | **118,16%** | Calculado sobre valores nominais: (benefícios − investimento) ÷ investimento. Não considera o valor do dinheiro no tempo. |
| Payback simples | **Mês 12** | O investimento acumulado é recuperado com o recebimento do segundo benefício semestral. |
| Payback descontado | **Mês 12** | Os fluxos descontados acumulados também se tornam positivos no segundo recebimento semestral. |
| Índice benefício-custo | **1,902** | Valor presente dos benefícios ÷ valor presente dos custos; acima de 1 indica que os benefícios descontados superam os custos. |

Fórmulas utilizadas:

$$
VPL = \sum_{t=1}^{24}\frac{FC_t}{(1+i_m)^t},\qquad
ROI = \frac{\text{benefícios nominais} - \text{custos nominais}}{\text{custos nominais}},\qquad
IBC = \frac{VP(\text{benefícios})}{VP(\text{custos})}
$$

A taxa mensal equivalente usada é $i_m=(1+0,1375)^{1/12}-1=0,0107939$, ou aproximadamente 1,0794% ao mês. A TIR é a taxa mensal que zera o VPL do fluxo de caixa. A taxa anual efetiva correspondente é calculada por $(1+\text{TIR mensal})^{12}-1$.

### 12.6 Sensibilidade e conclusão

O custo da equipe de desenvolvimento foi reduzido em relação à estimativa anterior porque agora usa bolsa de estágio de TI proporcional à dedicação de 5 h/semana, em vez de salário de desenvolvedor júnior com divisor de 200 h/mês. O cálculo é sensível à bolsa de estágio, aos benefícios obrigatórios para o estágio não obrigatório e aos encargos do empregador, que dependem do regime tributário e da situação da instituição.

Os indicadores aritméticos do cenário-base são favoráveis somente sob as hipóteses simplificadas do modelo, inclusive a realização de economia de um posto administrativo e a entrada em operação de uma solução completa. Como o escopo atual termina em protótipo com serviços simulados, esses indicadores **não representam o retorno financeiro deste projeto acadêmico**. Antes de avaliar investimento em produção, será necessário estimar separadamente o custo da integração OAuth/sistema acadêmico, infraestrutura, segurança, implantação, suporte e manutenção; validar se a instituição realmente evitará o custo de um posto administrativo; e então recalcular VPL, TIR, ROI, payback e índice benefício-custo para o escopo completo. A taxa Selic permanece apenas um benchmark, sujeito à taxa mínima de atratividade institucional.

Antes de solicitar investimento, recomenda-se validar a bolsa de estágio e a jornada de referência das vagas locais; estimar auxílio-transporte e demais obrigações de estágio; obter o salário e a composição efetiva dos encargos CLT do técnico administrativo na instituição (inclusive RAT/FAP, terceiros, benefícios e CCT); confirmar o consumo real de papel/impressão; verificar custos recorrentes e de integração; e comprovar se a capacidade liberada produzirá redução orçamentária. Os valores de mercado foram consultados em 28/09/2026 e não substituem cotações ou dados da folha institucional.
