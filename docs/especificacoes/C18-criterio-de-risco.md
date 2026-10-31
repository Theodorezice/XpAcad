# C18 – Critério de risco de engajamento configurável

**Issue:** #19 · **Prioridade:** Must · **Responsável:** Tatiane Millene de Souza

## História de usuário
Como coordenador, quero que o critério de risco seja parametrizável, para ajustá-lo sem depender de alteração de código.

## Objetivo
Permitir que a coordenação pedagógica defina quando um aluno é sinalizado como "em risco de evasão", ajustando os limites conforme a realidade de cada curso ou turma.

## Parâmetros configuráveis
| Parâmetro | Descrição | Valor padrão |
|---|---|---|
| Frequência mínima | Percentual mínimo de presença no período | 75% |
| Faltas consecutivas | Nº de aulas seguidas sem presença | 3 |
| Entregas não realizadas | Nº de atividades não entregues no período | 2 |
| Queda de XP | Redução percentual do XP semanal em relação à média do aluno | 50% |
| Período de análise | Janela de tempo considerada | 14 dias |
| Regra de combinação | Basta 1 parâmetro atingido ou exige todos | Basta 1 |

## Regras de negócio
- O critério é guardado como **configuração** (banco de dados/arquivo de configuração), nunca fixo no código.
- Apenas o perfil **Coordenação** pode visualizar e alterar o critério.
- Ao salvar uma alteração, a classificação de risco dos alunos é **recalculada**.
- Existe a opção **Restaurar padrão**, que volta todos os parâmetros aos valores da tabela acima.
- Toda alteração registra quem alterou e quando.
- O aluno não vê o critério nem a própria classificação de risco.

## Critérios de aceitação
- [ ] O critério é guardado como configuração, nunca fixo no código
- [ ] Alterar o critério muda a classificação dos alunos
- [ ] É possível restaurar os valores padrão

## Dependências
- C19 (#20) – Interface de configuração do critério de risco
- C17 (#18) – Sinalizar alunos em risco no painel
