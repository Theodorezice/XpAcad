# Time ágil — XP Acad

## Papéis do time
| Integrante | Papel | O que faz no projeto |
|---|---|---|
| Theodore de Sousa Dias Tredicci | Product Owner | Prioriza o backlog (MoSCoW), define e valida os critérios de aceitação e decide o que entra na sprint |
| Tatiane Millene de Souza | Scrum Master | Facilita as cerimônias, cuida do quadro e do limite de WIP e trata os impedimentos |
| Nycollas Neto Branquinho | Developer | Implementa e documenta os cartões, trabalha em dupla e revisa cartões de colegas |
| Lukas Fonseca Figueiredo Macedo | Developer | Implementa e documenta os cartões, trabalha em dupla e revisa cartões de colegas |
| Matheus Vinícius Gonçalves de Oliveira | Developer | Implementa e documenta os cartões, trabalha em dupla e revisa cartões de colegas |

## Definition of Ready
Uma issue só entra no DOING se:
- [ ] Indica o requisito de origem (RF/RNF) e o cartão correspondente
- [ ] Tem história de usuário e critérios de aceitação escritos
- [ ] Tem prioridade MoSCoW definida pelo Product Owner
- [ ] Tem estimativa em horas
- [ ] Não depende de algo externo ainda não resolvido (ou está marcada como impedida)
- [ ] Há espaço no limite de WIP do DOING

## Definition of Done
Uma issue só vai para DONE se (mesmo checklist do template de pull request):
- [ ] Nenhum dado pessoal do aluno é armazenado ou trafega sem criptografia (se aplicável)
- [ ] Testado nos dois papéis (aluno e coordenação), cada um vendo só o permitido (se aplicável)
- [ ] Revisado por outro integrante, que não implementou nem tem cartão atribuído
- [ ] Confirmado que bate com a descrição e os critérios da issue
- [ ] Issue movida para DONE no quadro

Nenhum cartão é dado como pronto por quem o escreveu sozinho.

## Matriz de stakeholders
| Quadrante | Estratégia | Stakeholders |
|---|---|---|
| Alto poder · alto interesse | Gerenciar de perto | Professor-orientador, Coordenação, Equipe de desenvolvimento |
| Alto poder · baixo interesse | Manter satisfeito | ANPD, Diretoria |
| Baixo poder · alto interesse | Manter informado | Alunos |
| Baixo poder · baixo interesse | Monitorar | Fornecedor de infraestrutura |

Justificativa de quem tem nível médio em poder ou interesse:
- **Equipe de desenvolvimento:** interesse médio na classificação inicial, mas é quem executa o trabalho e por isso fica no quadrante de alto interesse.
- **Diretoria:** interesse médio; decide a continuidade do projeto e acompanha apenas as entregas, então é mantida satisfeita nas Sprint Reviews.
- **Alunos:** poder médio; são os usuários principais e precisam ser informados de como a aplicação funciona e de suas atualizações.

## Plano de comunicação
| O que comunicar | Para quem | Evento ou canal | Frequência | Responsável |
|---|---|---|---|---|
| Meta da sprint e backlog | Equipe de desenvolvimento, Professor-orientador | Sprint Planning | A cada sprint | Product Owner / Scrum Master |
| Progresso e planejamento do dia | Equipe de desenvolvimento | Daily Scrum ([canal]) | Diária (15 minutos) | Developers / Scrum Master |
| Demonstração da entrega e coleta de feedback | Coordenação, Diretoria, Professor-orientador, Alunos | Sprint Review | Final da sprint | Product Owner / Scrum Master |
| Melhorias de processo e análise do trabalho em equipe | Equipe de desenvolvimento | Sprint Retrospective | Final da sprint, após a Review | Scrum Master / Developers |
| Estado do backlog e dos critérios de risco e de visibilidade dos dados | Coordenação | [canal combinado] | A cada sprint | Product Owner |
| Conformidade com a LGPD (dados pessoais e consentimento) | ANPD, Diretoria | Documento de privacidade no repositório | A cada mudança que envolva dados pessoais | Product Owner |
| Decisões de hospedagem e infraestrutura | Fornecedor de infraestrutura | [canal combinado] | Quando houver decisão | Scrum Master |

Planning, Daily e Retrospective são feitas apenas com o Scrum Team.

## Quadro e limite de WIP
Quadro no GitHub Projects, ligado ao repositório:

| Coluna | Limite | Justificativa |
|---|---|---|
| BACKLOG | Sem limite | Guarda todos os cartões ainda não escolhidos para a sprint |
| TO-DO | 6 | Define a meta de entregáveis da sprint, priorizando os cartões mais importantes, sem sobrecarregar o time |
| DOING | 2 | O time tem 5 pessoas e trabalha em duas duplas, enquanto o 5º integrante apoia as duas ou inicia revisões; nunca há mais cartões em execução do que pessoas disponíveis |
| REVIEW | 1 | A revisão é feita por um integrante que não fez o cartão e não tem cartão atribuído |
| DONE | Sem limite | Cartões que cumprem a Definition of Done |

Regra de bloqueio: cartão parado por dependência externa é marcado como impedido, continua contando para o WIP e é o primeiro assunto da conversa seguinte do time.

## Declaração de uso de IA
- **Claude (Sonnet 5):** usado na ideação, na categorização FURPS+ dos requisitos, na criação e divisão dos cartões do Kanban e no apoio à estruturação desta entrega (templates e este documento). O time revisou os resultados, balanceou o texto da ideação para atender também aos alunos e ajustou os textos ao projeto.
- **Google Stitch:** usado para gerar as telas do protótipo, depois refinadas pelo time com prompts de ajuste (navegação entre perfis e correção do cabeçalho).
