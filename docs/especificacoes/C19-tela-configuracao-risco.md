# C19 – Interface de configuração do critério de risco

**Issue:** #20 · **Prioridade:** Must · **Requisito:** RF09 · **Responsável:** Tatiane Millene de Souza

## História de usuário
Como coordenador, quero configurar o critério de risco por uma tela, para ajustá-lo sozinha, sem ajuda técnica.

## Acesso
- Menu do painel da coordenação → **Configurações → Critério de risco**.
- Somente usuários com perfil **Coordenação** veem o menu e acessam a tela. Alunos e professores que tentarem acessar o endereço direto recebem "Acesso negado".

## Campos da tela
| Campo | Tipo | Validação | Valor padrão (C18) |
|---|---|---|---|
| Frequência mínima | Percentual | 0% a 100% | 75% |
| Faltas consecutivas | Número inteiro | 1 a 20 | 3 |
| Entregas não realizadas | Número inteiro | 1 a 20 | 2 |
| Queda de XP | Percentual | 10% a 100% | 50% |
| Período de análise | Dias | 7 a 60 | 14 |
| Regra de combinação | Opção | "Basta 1" ou "Todos" | Basta 1 |

## Botões
- **Salvar:** valida os campos, grava a configuração e recalcula a classificação de risco dos alunos.
- **Restaurar padrão:** pede confirmação e volta todos os campos aos valores padrão definidos na C18.
- **Cancelar:** descarta alterações não salvas.

## Mensagens
- Sucesso: "Critério atualizado. A classificação dos alunos foi recalculada."
- Erro de validação: o campo inválido fica destacado com a faixa permitida.
- Rodapé: "Última alteração por (nome) em (data e hora)".

## Critérios de aceitação
- [ ] A tela permite alterar os parâmetros (frequência, ausências, entregas)
- [ ] Salvar recalcula a classificação dos alunos
- [ ] Apenas a coordenação acessa a tela

## Dependências
- C18 (#19) – Critério de risco de engajamento configurável
- C17 (#18) – Sinalizar alunos em risco no painel
