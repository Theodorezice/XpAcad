# C31 – Download da imagem do selo

**Issue:** #32 · **Prioridade:** Could · **Estimativa:** 6h

## História de usuário

Como aluno, quero baixar a imagem do selo que conquistei, para compartilhá-la em outros lugares.

## Objetivo

Permitir que o aluno baixe uma cópia da imagem de um selo já conquistado, facilitando o compartilhamento da conquista sem expor informações pessoais ou indicadores individuais de desempenho.

## Regras de negócio

- A opção de download deve aparecer somente para selos conquistados pelo aluno autenticado.
- Selos ainda não conquistados não devem disponibilizar a ação de download.
- A imagem deve ser fornecida em um formato comum. Como proposta inicial, recomenda-se PNG.
- O arquivo deve conter somente a arte e a identificação pública do selo, sem nome do aluno, matrícula, turma, quantidade de XP, nível, posição em ranking ou outros dados individuais.
- O download não deve alterar o XP, o nível, o histórico ou o estado de conquista do selo.
- O aluno só pode baixar imagens dos selos que conquistou.

## Fluxo principal

1. O aluno acessa a área em que seus selos conquistados são exibidos.
2. O sistema apresenta a opção de download nos selos conquistados.
3. O aluno seleciona a opção de baixar a imagem.
4. O sistema disponibiliza o arquivo da imagem em formato PNG.
5. O dispositivo realiza o download do arquivo.

## Critérios de aceitação

- [ ] A imagem do selo é baixada em um formato comum (proposta: PNG).
- [ ] O arquivo não contém dados pessoais ou informações individuais de desempenho do aluno.
- [ ] A opção de download está disponível somente para selos conquistados pelo próprio aluno.
- [ ] O download não altera XP, nível, histórico ou estado de conquista do selo.

## Observações

A definição de PNG é uma proposta para concretizar o requisito de formato comum e pode ser validada pela equipe. Esta issue trata da especificação funcional; não pressupõe implementação de código nesta contribuição.
