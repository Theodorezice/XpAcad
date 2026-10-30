# C17 – Sinalizar alunos em risco no painel

**Issue:** #18 · **Prioridade:** Should · **Requisito:** RF08 · **Responsável:** Tatiane Millene de Souza

## História de usuário
Como coordenador, quero ver sinalizados os alunos com baixo engajamento, para intervir antes que o problema se agrave.

## Como o aluno é classificado
- A classificação usa o critério parametrizado definido na C18 (#19) e ajustado pela tela da C19 (#20).
- Cada aluno recebe um de dois estados: **Em risco** ou **Regular**.
- O motivo da sinalização fica registrado (ex.: "3 faltas consecutivas", "2 entregas pendentes").

## Exibição no painel da coordenação
- Etiqueta **"Em risco"** em destaque ao lado do nome do aluno.
- Ao passar o mouse ou tocar na etiqueta, aparece o motivo da sinalização.
- Filtro **"Mostrar só alunos em risco"** e contador no topo ("X alunos em risco nesta turma").
- A sinalização não usa apenas cor: tem texto e ícone, para garantir acessibilidade.

## Atualização
- A classificação é recalculada sempre que o critério de risco é alterado (C19).
- Também é recalculada a cada novo registro de presença, participação ou entrega.

## Privacidade
- Somente o perfil **Coordenação** vê a sinalização.
- O aluno não vê a própria classificação de risco.

## Critérios de aceitação
- [ ] Os alunos são classificados de acordo com o critério de risco parametrizado
- [ ] A sinalização fica visível no painel da coordenação
- [ ] A sinalização é atualizada quando o critério muda

## Dependências
- C18 (#19) – Critério de risco de engajamento configurável
- C19 (#20) – Interface de configuração do critério de risco
- C16 (#17) – Tela do painel da coordenação
