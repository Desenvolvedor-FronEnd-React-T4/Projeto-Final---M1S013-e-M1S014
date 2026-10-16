# AgendaPet Web — Leia-me primeiro

## O que é o sistema

**AgendaPet Web** é um painel web de agendamentos para a **Patinhas & Cia**, um pet shop de bairro (empresa fictícia). Hoje a loja marca banho, tosa, consulta e hospedagem por WhatsApp e caderno, e isso gera horários duplicados, atendimentos em feriados sem aviso, endereços errados em visitas a domicílio e nenhuma noção de quanto o dia rendeu.

Você é a pessoa desenvolvedora júnior contratada para entregar, em uma **sprint de duas semanas**, a primeira versão do painel. Com ele, a atendente consegue, pelo celular ou tablet na bancada:

- ver o catálogo de serviços (preço e duração);
- agendar atendimentos com validação (data, horário de funcionamento, telefone);
- preencher o endereço de atendimentos a domicílio só com o CEP;
- ser avisada quando a data escolhida é feriado;
- acompanhar a agenda do dia (busca, filtros, concluir/cancelar) e receber lembretes;
- ver o fechamento do dia, e a dona da loja fecha o caixa também pelo terminal, com Node.js.

O projeto é feito com **HTML, CSS e JavaScript puros** (sem frameworks) e scripts **Node.js**.

## Objetivos do projeto

1. Aplicar na prática os conteúdos do Módulo 01: HTML semântico, CSS/Flexbox/responsividade, DOM e eventos, formulários, `fetch` e `async/await`, `localStorage`, timers, classes e herança, closures, módulos (ESM e CommonJS), npm e depuração.
2. Trabalhar como em uma empresa: backlog de histórias (US01 a US12), estimativa, **Kanban**, **uma branch e um Pull Request por ticket**, commits padronizados.
3. Conseguir **explicar o próprio código** e apresentá-lo ao vivo.

## Datas e entrega

| Data | O quê |
|---|---|
| 16/10 (sex) | Liberação do projeto e Sprint Planning |
| 20, 22 e 23/10 | Mentoria — Semana 13 |
| 27 e 29/10 | Mentoria — Semana 14 |
| **30/10 (sex)** | **Apresentação em live coding no Google Meet, com a turma reunida: 15 minutos por estudante**, mostrando o código feito e a tela funcionando |
| **02/11 (seg), até as 22h** | **Prazo de entrega no AVA** |

**A entrega é dupla e obrigatória:** o projeto deve estar no **AVA** (tarefa "Módulo 01 - Mini-Projeto Avaliativo (M1.2)") **e** publicado em um **repositório público no GitHub**. No AVA, envie o link do repositório e o link do Kanban.

## O que tem nesta pasta

### Documentos para ler (nesta ordem)

| Ordem | Arquivo | Para que serve |
|---|---|---|
| 1 | `Documento_Funcional_AgendaPet` (.pdf / .html) | O **quê** e o **porquê**: regras de negócio, telas e fluxos |
| 2 | `Refinamento_Tecnico_AgendaPet` (.pdf / .html) | O **como**: arquivos, funções, contratos de dados e modelos de código |
| 3 | `Mini-Projeto Avaliativo - AgendaPet Web - Front-End React T4.docx` | **Enunciado oficial**: backlog, critérios de aceite, avaliação e checklist. Em caso de divergência entre documentos, vale o enunciado |

### Kanban

| Arquivo | Para que serve |
|---|---|
| `Kanban_PassoAPasso.md` | Passo a passo para montar o quadro (Trello, GitHub Projects ou Notion) |
| `Kanban_AgendaPet_Exemplo.png` | Imagem de um quadro modelo |
| `Kanban_AgendaPet_Modelo.md` / `.csv` | Os 12 cartões prontos (sem estimativas: essa parte é sua) |

### Modelos e Apoio (copie para o seu projeto)

Tudo o que está em `Modelos e Apoio/` é opcional, mas poupa tempo. Copie assim:

| Arquivo em `Modelos e Apoio/` | Copie para o seu projeto como | Quando |
|---|---|---|
| `Guia_Git_GitHub.md` | (só leitura) | 16/10, ao criar o repositório |
| `sprint-planning_MODELO.md` | `planejamento/sprint-planning.md` | 16/10 |
| `pull_request_template.md` | `.github/pull_request_template.md` | 16/10 |
| `dados/servicos.json` | `data/servicos.json` | US02 |
| `dados/agenda-exemplo.json` | `data/agenda-exemplo.json` | US11 |
| `dados/agenda-invalida.json` | `data/agenda-invalida.json` | US11 |
| `img/logo.svg` e `img/favicon.svg` | `img/logo.svg` e `img/favicon.svg` | US01 / US10 |
| `bug-report_MODELO.md` | `docs/bug-report.md` | US12 |
| `README_MODELO.md` | `README.md` | durante a sprint; finalize em 30/10 |
| `Roteiro_Apresentacao_Live_Coding.md` | (só leitura) | antes de 30/10 |

Os arquivos de dados seguem exatamente o formato descrito no Refinamento Técnico (seções 4.2 e 4.3). Você pode usá-los como estão ou criar os seus.

## Por onde começar (16/10)

1. Leia o Documento Funcional e o enunciado.
2. Crie o repositório no GitHub (veja o `Guia_Git_GitHub.md`).
3. Monte o Kanban (veja o `Kanban_PassoAPasso.md`).
4. Estime os cartões, escreva a meta da sprint e preencha o `sprint-planning.md`.
5. Trabalhe um ticket por vez, cada um na sua branch, com Pull Request.
