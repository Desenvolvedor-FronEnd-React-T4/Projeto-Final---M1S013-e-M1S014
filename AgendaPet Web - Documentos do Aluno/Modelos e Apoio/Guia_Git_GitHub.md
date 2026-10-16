# Guia rápido de Git e GitHub para o projeto

O projeto exige: **repositório público**, **uma branch e um Pull Request (PR) por ticket**, **commits padronizados** e a `main` sempre funcionando.

**Mínimos exigidos:** 12 commits ao longo das duas semanas · 5 branches além da `main` · 5 PRs integrados.

> Prefere interface gráfica? O **GitHub Desktop** faz o mesmo (Clone, Current Branch → New Branch, Commit, Push origin, Create Pull Request). Abaixo, os comandos do terminal.

## 1. Primeira vez: criar o repositório

1. No GitHub: **New repository** → nome `agendapet-web` → **Public** → crie sem README.
2. No terminal, dentro da pasta do projeto:

```bash
git init
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/agendapet-web.git
```

3. Primeiro commit (na `main`, só a base do projeto: `.gitignore`, modelo de PR, estrutura):

```bash
git add .
git commit -m "chore: inicia projeto"
git push -u origin main
```

`.gitignore` mínimo:

```
node_modules/
```

## 2. Para cada ticket

```bash
git checkout main
git pull                                  # traz a main atualizada
git checkout -b feat/US03-formulario      # cria a branch do ticket

# ... programe ...

git add .
git commit -m "feat(US03): adiciona validação de data e horário"
git push -u origin feat/US03-formulario   # na primeira vez da branch
```

Faça **vários commits pequenos** por branch (não um só no final).

## 3. Abrir e integrar o Pull Request

1. No GitHub, aparecerá **Compare & pull request** → clique.
2. O modelo de `.github/pull_request_template.md` aparece sozinho: preencha **o que mudou**, **ticket**, **como testar**, **evidência (print ou GIF)** e marque o checklist.
3. Revise o seu próprio PR na aba **Files changed**, comente o que verificou e **aprove/mescle** (**Merge pull request**).
4. Volte ao terminal e atualize:

```bash
git checkout main
git pull
```

5. Mova o cartão do Kanban para **Concluído** com o link do PR.

## 4. Padrões

**Branches** (`tipo/US##-descricao`, sem acentos e em minúsculas):

```
feat/US03-formulario
fix/US07-faturamento-concluidos
chore/setup-projeto
docs/readme
```

**Commits** (Conventional Commits, no imperativo, citando o ticket): `tipo(ticket): descrição`

| Tipo | Quando usar | Exemplo |
|---|---|---|
| `feat` | Funcionalidade nova | `feat(US04): preenche endereço pelo CEP` |
| `fix` | Correção de bug | `fix(US07): soma só atendimentos concluídos` |
| `docs` | Documentação | `docs: descreve a regra da taxa domiciliar` |
| `style` | Formatação/CSS sem mudar lógica | `style(US10): ajusta espaçamentos no celular` |
| `refactor` | Reorganizar sem mudar comportamento | `refactor(US07): move regras para js/dominio` |
| `test` | Testes | `test(US07): testa fechamento do dia` |
| `chore` | Configuração e tarefas gerais | `chore: adiciona .gitignore` |

## 5. Problemas comuns

| Situação | O que fazer |
|---|---|
| Esqueci de criar a branch e já mexi na `main` | `git checkout -b feat/US0X-nome` (leva as mudanças junto) e commite na nova branch |
| `git push` pede para definir upstream | `git push -u origin nome-da-branch` |
| Commitei a pasta `node_modules` | Adicione `node_modules/` ao `.gitignore` e rode `git rm -r --cached node_modules` e faça um novo commit |
| Subi uma chave ou dado pessoal por engano | Remova o dado, troque a chave e avise o mentor (não basta apagar no commit seguinte) |
| Conflito ao mesclar | Abra o arquivo, escolha o trecho correto, remova os marcadores `<<<<<<<`, `=======` e `>>>>>>>`, depois `git add` e `git commit` |
| Quero ver o histórico | `git log --oneline` |

## 6. Antes de entregar

- [ ] Repositório **público** (teste abrindo o link em uma janela anônima)
- [ ] 12 ou mais commits, 5 ou mais branches e 5 ou mais PRs integrados
- [ ] `node_modules/` fora do repositório e nenhum segredo versionado
- [ ] Clone em outra pasta: `npm install` e `npm start` funcionam apenas seguindo o README
