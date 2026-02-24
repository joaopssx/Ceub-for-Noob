# Lista 01 - Git + GitHub

## Objetivo

Fixar o fluxo basico de versionamento local e remoto.

## Explicacao curta

Faz na ordem.
No Git, ordem de comando importa muito.

## Codigo completo

Nao existe um codigo unico.
Cada exercicio e um fluxo de comandos no terminal.

## Como executar

Use um repositorio de treino e rode os comandos da atividade.

Comandos que voce mais vai usar:

```bash
git status
git add .
git commit -m "mensagem"
git log --oneline
```

## Saida esperada (exemplo)

```text
On branch main
nothing to commit, working tree clean
```

## Erros comuns + como resolver

- pular `git status` e se perder
- commitar na branch errada
- tentar push sem configurar remote

## Exercicios

### Faceis (3)

1. Criar repositorio local com `git init`.
2. Criar `README.md`, adicionar e commitar.
3. Ver historico com `git log --oneline`.

### Medios (2)

1. Criar branch `feat/teste`, alterar arquivo e commitar.
2. Voltar pra `main` e mergear branch.

### Desafio (1)

1. Conectar no GitHub e subir projeto com `git push`.

## Extras (mais 6)

7. Fazer `git pull` depois de alterar arquivo direto no GitHub.
8. Abrir PR de branch de feature.
9. Atualizar PR com mais um commit.
10. Simular conflito e resolver.
11. Ajustar URL de remote com `git remote set-url`.
12. Clonar repo em outra pasta e sincronizar com push/pull.
