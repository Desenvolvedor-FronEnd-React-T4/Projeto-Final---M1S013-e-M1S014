<!--
  pull_request_template.md — MODELO AUTOMÁTICO DE PULL REQUEST   (fluxo Git, todos os tickets)

  O QUE É: o GitHub lê este arquivo (precisa estar na pasta .github/) e já
  preenche a descrição de TODO Pull Request novo com o texto dele.

  O QUE FAZER: copie o modelo oficial de "Modelos e Apoio/pull_request_template.md"
  para cá. Você pode adaptar, mas mantenha:
    - uma seção "O que mudou" curta (2 ou 3 linhas);
    - o número do ticket (Fecha **US__**);
    - os passos para testar;
    - uma evidência (print ou GIF);
    - o checklist da Definição de Pronto.

  EXEMPLO GENÉRICO DE SEÇÕES:

    ## O que mudou
    Adiciona a validação de telefone no formulário.

    ## Ticket
    Fecha **US03** – Formulário de novo agendamento

    ## Como testar
    1. `npm install` e `npm start`
    2. Tente salvar o formulário sem preencher nada
    3. Veja as mensagens de erro em cada campo

    ## Definição de Pronto
    - [ ] Os cenários de aceite da história passam
    - [ ] Sem erros no console do navegador

  REGRA DO FLUXO: UMA branch e UM Pull Request por ticket, com commits no
  padrão  tipo(US__): descrição no imperativo   (ex.: feat(US03): validar telefone).
-->
