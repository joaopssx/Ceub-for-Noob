# 01 - init, add e commit

## Objetivo

Criar seu primeiro repositorio local e fazer commit da forma certa.

## Explicacao curta

Fluxo base do Git:

- `git init` cria repositorio
- `git add` prepara arquivo
- `git commit` salva snapshot

Sem esse trio, nada anda.

## Codigo completo

```bash
mkdir aula-git
cd aula-git

git init

echo "# Projeto Aula Git" > README.md

git status
git add README.md
git commit -m "chore: cria README inicial"

git log --oneline
```

## Como executar

1. Crie pasta e entre nela.
2. Rode `git init`.
3. Crie arquivo.
4. Rode `git add`.
5. Rode `git commit`.
6. Veja historico com `git log --oneline`.

## Saida esperada (exemplo)

```text
[main (root-commit) a1b2c3d] chore: cria README inicial
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
```

## Erros comuns + como resolver

### `fatal: not a git repository`

Voce nao esta dentro da pasta com `.git`.
Entra na pasta certa ou roda `git init`.

### `nothing to commit`

Voce tentou commit sem mudar arquivo.
Rode `git status` pra confirmar.

### commit com mensagem ruim tipo "update"

Evita mensagem generica. Fala o que fez de verdade.

## Exercicios

### Faceis (3)

1. Criar repositorio local vazio.
2. Criar `README.md` e commitar.
3. Rodar `git log --oneline`.

### Medios (2)

1. Fazer segundo commit alterando README.
2. Criar arquivo `anotacoes.txt` e commitar separado.

### Desafio (1)

1. Fazer 3 commits pequenos com mensagens claras, cada um com uma mudanca.
