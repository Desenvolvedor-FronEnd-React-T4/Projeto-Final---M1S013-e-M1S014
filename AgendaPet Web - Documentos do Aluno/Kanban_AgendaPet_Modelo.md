# Kanban da Sprint — AgendaPet Web (modelo)

Este é o **ponto de partida** do seu quadro. Os 12 cartões (um por história) já estão listados; **a estimativa em pontos, a meta da sprint, a branch e o link do Pull Request são com você** (Sprint Planning, dia 16/10).

> O arquivo `Kanban_AgendaPet_Modelo.csv` tem os mesmos cartões em formato de planilha (abre no Excel/Google Planilhas e pode ser importado no Notion).

> Primeira vez montando um quadro? Veja o [passo a passo](Kanban_PassoAPasso.md) e a imagem de exemplo `Kanban_AgendaPet_Exemplo.png`.

## 1. Meta da sprint

Escreva em **uma frase** o que a sprint precisa entregar:

> _______________________________________________

## 2. Colunas

| Coluna | Significado |
|---|---|
| **Backlog** | Todos os 12 cartões começam aqui |
| **A Fazer** | Cartão estimado, com critérios de aceite lidos, escolhido para a sprint |
| **Em Andamento** | Você está trabalhando nele agora, na sua branch (um por vez) |
| **Em Revisão** _(recomendada)_ | Pull Request aberto, aguardando a sua revisão |
| **Concluído** | Pull Request integrado à `main` e Definição de Pronto cumprida |

## 3. Cartões

| Ticket | História | Prioridade | Pontos (1, 2, 3, 5 ou 8) | Branch | Pull Request |
|---|---|---|---|---|---|
| US01 | Estrutura semântica e acessível da página | Alta | | | |
| US02 | Catálogo de serviços | Alta | | | |
| US03 | Formulário de novo agendamento | Alta | | | |
| US04 | Endereço automático por CEP | Média | | | |
| US05 | Alerta de feriados | Média | | | |
| US06 | Agenda do dia: lista, busca, filtros e atalhos | Alta | | | |
| US07 | Regras de negócio e fechamento do dia | Alta | | | |
| US08 | Persistência e exportação dos dados | Alta | | | |
| US09 | Relógio e lembretes de atendimento | Média | | | |
| US10 | Layout responsivo e identidade visual | Alta | | | |
| US11 | Projeto Node.js e relatório de fechamento | Alta | | | |
| US12 | Depuração e relatório de bug | Média | | | |

Os critérios de aceite de cada história estão no item 5.1 do enunciado (.docx).

## 4. Como montar o quadro

**Trello:** crie um quadro, adicione as colunas acima e um cartão por ticket (título `US03 · Formulário de novo agendamento`). Use a descrição do cartão para a branch e o link do PR.

**GitHub Projects:** na aba *Projects* do repositório, crie um projeto com o template *Board*, ajuste as colunas e adicione um item por ticket. Vale também usar Issues, uma por ticket.

**Notion:** importe o `.csv` como tabela e mude a visualização para *Board*, agrupando pela propriedade de coluna/status.

**Sem ferramenta externa:** é permitido um quadro simples no README, uma planilha ou a imagem do quadro em `docs/kanban.png`.

O **link do quadro precisa estar acessível a quem corrige** (público ou compartilhado).

## 5. Regras do quadro

- **Definição de Pronto para Iniciar** (cartão que sai do Backlog para A Fazer): história lida e critérios de aceite entendidos; ticket estimado em pontos; branch criada no padrão `tipo/US##-descricao` (ex.: `feat/US03-formulario`).
- **Cada cartão cita a branch e o link do Pull Request.**
- **Movimente os cartões ao longo das duas semanas.** Nunca deixe tudo em Concluído só no último dia: o histórico de movimentação faz parte da avaliação.
- Um cartão só vai para **Concluído** com o PR integrado e a Definição de Pronto cumprida (item 5.1 do enunciado).
- Registre também, em `planejamento/sprint-planning.md`: meta da sprint, ordem de execução e por quê, estimativa de cada ticket, riscos (ex.: API fora do ar) e o que seria cortado se faltasse tempo.
