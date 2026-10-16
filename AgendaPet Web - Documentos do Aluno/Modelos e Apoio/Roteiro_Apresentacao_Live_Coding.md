# Roteiro da apresentação em live coding (Sprint Review)

**Quando:** sexta-feira, 30/10 · **Onde:** Google Meet, com a turma reunida · **Tempo:** 15 minutos por estudante · **Como:** você compartilha a tela (VS Code + navegador) e mostra o código e o sistema funcionando.

Você apresenta ao cliente (a Patinhas & Cia) e depois comenta o processo. Todos os itens do item 4.6 do enunciado precisam aparecer.

## Divisão do tempo (sugestão)

| Tempo | O que mostrar | Dica |
|---|---|---|
| 0:00 – 1:00 | **Abertura:** seu nome, o que é o AgendaPet Web e a meta da sprint | Uma frase para cada |
| 1:00 – 5:00 | **Demonstração para o cliente** com a tela e o código correspondente | Siga a ordem abaixo |
| 5:00 – 6:30 | **Como executar:** `git clone`, `npm install`, `npm start`, `npm run fechamento`, `npm run validar` | Mostre o terminal; o clone pode estar pronto |
| 6:30 – 8:00 | **Sprint Planning:** Kanban, meta, estimativas e a movimentação dos cartões | Mostre branch e PR em um cartão |
| 8:00 – 9:30 | **Branches e Pull Requests:** abra um PR e explique o que mudou, como testar e a evidência | Mostre também o histórico de commits |
| 9:30 – 11:30 | **Node.js:** onde está o ESM, onde está o CommonJS, o que você instalou localmente e o que é a instalação global | Abra `package.json`, `fechamento-dia.js` e `validar-agenda.cjs` |
| 11:30 – 13:30 | **Depuração:** VS Code pausado em um breakpoint, com variáveis, Watch e Call Stack; apresente o bug do relatório | Use F5 com o `launch.json` |
| 13:30 – 15:00 | **Retrospectiva:** o que funcionou, o que não funcionou, o que faria diferente. **Declare onde usou IA e o que validou** | Termine no tempo |

### Ordem sugerida da demonstração (1:00 – 5:00)

1. Página carregando e o catálogo de serviços (estados de carregamento e sucesso).
2. Agendamento comum, com um erro de validação antes (foco no primeiro campo inválido).
3. Agendamento **domiciliar** com CEP preenchendo o endereço.
4. **Feriado** (ex.: 25/12): aviso e "Agendar mesmo assim".
5. **Conflito de horário**.
6. Mudar status (concluir/cancelar), busca e atalhos de teclado.
7. **Fechamento do dia** (faturamento só dos concluídos).
8. **Recarregar a página** (F5): os dados continuam.
9. **Tela no celular** (DevTools em 360 px).

## Antes de entrar na chamada

- [ ] Projeto **já clonado**, com `npm install` feito e o servidor funcionando (`npm start`)
- [ ] VS Code e navegador abertos, com fonte do editor em tamanho legível (aumente o zoom com `Ctrl +`)
- [ ] Abas prontas: Kanban, repositório no GitHub, um Pull Request, `package.json`, `fechamento-dia.js`, `validar-agenda.cjs`, `docs/bug-report.md`
- [ ] Algumas informações já na agenda (ou use "dados de exemplo"), para não perder tempo digitando
- [ ] Breakpoint já colocado e o `launch.json` testado com F5
- [ ] Câmera, microfone e compartilhamento de tela testados; internet estável
- [ ] Feche notificações e abas pessoais
- [ ] **Ensaiou com cronômetro** e consegue terminar em 15 minutos

## Se algo der errado

| Problema | O que fazer |
|---|---|
| ViaCEP ou BrasilAPI fora do ar | Aproveite: mostre o tratamento de falha (preenchimento manual e aviso de feriado indisponível). Isso também vale ponto |
| Erro inesperado no console | Mantenha a calma, explique o que está vendo e siga adiante. Se souber a causa, comente |
| Estourando o tempo | Corte detalhes da demonstração, nunca os itens obrigatórios do 4.6 |
| Página não abre | Confira se o `npm start` está rodando e se usou `http://localhost:5500`, não `file://` |

## Esteja preparado(a) para explicar o código

A avaliação considera que você **explica linha a linha** o que entregou. Se o mentor pedir, esteja pronto para abrir um arquivo e mostrar, por exemplo: onde está a regra do conflito de horário, onde a taxa domiciliar é calculada, onde o protocolo sequencial é gerado e por que a herança foi usada.

Sobre IA: se usou, diga **onde** e **o que você conferiu e corrigiu**. Código que você não consegue explicar gera desconto.
