# Relatório de bug — BUG-01

<!-- Copie para docs/bug-report.md. O bug deve ser um defeito REAL encontrado por você.
     Se nenhum surgir, crie uma branch, introduza um erro controlado (por exemplo, o fechamento somar
     cancelados ou agendados), reproduza, depure, corrija e documente como o encontrou. -->

| Campo | Valor |
|---|---|
| **Título** | [descreva o defeito em uma frase] |
| **Ticket relacionado** | US__ – [título] |
| **Onde apareceu** | [tela, comando ou arquivo] |
| **Branch da correção** | [ex.: `fix/US07-...`] (PR #__) |
| **Gravidade** | [Baixa / Média / Alta] — [por quê] |

## Passos para reproduzir

1. [ ]
2. [ ]
3. [ ]

## Resultado esperado × obtido

| | Esperado | Obtido (com o bug) |
|---|---|---|
| [o que você conferiu] | [valor] | [valor] |

## Investigação com o depurador

Configuração usada: **"[nome no launch.json]"** (tecla **F5**).

1. **Breakpoint** em `[arquivo]`, linha `[ ]`.
2. Variables / Watch:

   | Expressão (Watch) | Valor |
   |---|---|
   | `[expressão]` | [valor] |

3. **Call Stack:** [funções, do topo para a base, e o que concluiu].
4. **Breakpoint condicional ou logpoint:** [condição usada e o que provou].

Evidência: [depuracao.png](depuracao.png)

## Causa raiz

[Explique por que o erro aconteceu (a causa, não o sintoma). Mostre o código antes e depois.]

```js
// ANTES (bug)

// DEPOIS (correto)
```

## Correção

- Commit ou Pull Request: [`fix(US__): ...`] / [#__]
- Como confirmar que foi corrigido: [comando ou passo]

## Como evitar de novo

- [ ]
