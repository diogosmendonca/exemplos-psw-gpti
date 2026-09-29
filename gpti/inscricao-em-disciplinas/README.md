# Módulo de inscrição em disciplinas

Exemplo de planejamento de um protótipo acadêmico. Os alunos de GPTI conduzem a gestão. Os alunos de PSW propõem o escopo funcional e desenvolvem o produto. A semana letiva 1 começou em 03/08/2026. A AV1 é na semana letiva 8.

Os identificadores PSW-1 a PSW-4 e GPTI-1 a GPTI-4 são lugares dos nomes. O produto desta fase é um protótipo: OAuth e o sistema acadêmico ficam simulados, e as regras de matrícula são hipóteses da equipe.

## Documentos

A leitura segue o processo. A iniciação autoriza o trabalho. O planejamento detalha o que foi autorizado. O dicionário fecha a linha de base do escopo.

| Documento | Para que serve |
|---|---|
| [Caso de negócio](business-case.md) | Iniciação. Problema, alternativas e ordem de grandeza. Os indicadores financeiros são da iniciativa futura, não do protótipo. |
| [Termo de abertura](termo-de-abertura.md) | Autoriza o projeto. Objetivos do protótipo, marcos, premissas e governança. |
| [Plano de projeto](plano-de-projeto.md) | Escopo, EAP, cronograma, recursos, custos, riscos e engajamento. |
| [Dicionário da EAP](dicionario-eap.md) | Aceite observável de cada pacote e quem presta contas dele. |

A linha de base do escopo é a declaração no plano, a EAP e este dicionário. Marco, recurso e custo ficam no plano.

## Estrutura de gestão

O patrocinador é o Prof. Diogo Mendonça. Ele aprova mudança, marco e cancelamento. Não presta contas de pacote da EAP.

GPTI-1 é o gerente do projeto e presta contas do plano inteiro. GPTI-4 prepara a comunicação com o patrocinador. GPTI-1 responde pelo conteúdo.

| Papel | Quem | O que faz neste projeto |
|---|---|---|
| Patrocinador | Prof. Diogo Mendonça | Acompanha as demonstrações e decide mudança relevante de escopo, prazo ou reserva gerencial. |
| Gerente do projeto | GPTI-1 | Confere pedido de mudança contra a EAP e coordena a equipe de gestão. |
| Equipe de gestão | GPTI-1 a GPTI-4 | Planeja, valida o escopo proposto por PSW e registra decisão, risco e aceite. |
| Equipe de produto | PSW-1 a PSW-4 | Propõe o escopo funcional e implementa frontend, backend, testes e documentação. |

Cada pacote de primeiro nível tem um responsável por prestar contas (A). Os demais executam (R). O detalhe de cada pacote está no [dicionário](dicionario-eap.md).

| Pacote | Presta contas |
|---|---|
| 1.1 Gestão | GPTI-1 |
| 1.2 Requisitos e desenho | GPTI-3 |
| 1.3 Ambiente | PSW-4 |
| 1.4 Frontend do marco 1 | PSW-1 |
| 1.5 Regras e API | PSW-3 |
| 1.6 Integração do marco 2 | PSW-4 |
| 1.7 Verificação e encerramento | GPTI-4 |

Secretaria, equipe de identidade e a instituição não participam desta etapa. Contato com elas só com autorização do patrocinador.

## Figuras do cronograma

O plano incorpora as figuras. No GitHub, o clique abre a imagem em outra aba. Os arquivos HTML servem para abrir no navegador e ver a dependência ao passar o mouse.

- [Gantt com dependências e esforço](cronograma-gantt-recursos.png)
- [Alocação individual](cronograma-alocacao-individual.png)
- [Gantt por aluno de PSW](cronograma-gantt-psw-individual.png)
- [Gantt por aluno de GPTI](cronograma-gantt-gpti-individual.png)
