# 01 - Branch e merge

## Objetivo

Trabalhar em branch separada e juntar no `main` com merge.

## Explicacao curta

Branch e uma linha paralela de trabalho.
Voce desenvolve sem quebrar o que ja esta funcionando na `main`.

## Codigo completo

```bash
git checkout -b feat/menu

echo "Menu inicial" >> README.md
git add README.md
git commit -m "feat: adiciona menu inicial"

git checkout main
git merge feat/menu

git log --oneline --graph --all
```

## Como executar

1. Crie branch com `git checkout -b`.
2. Faca alteracao e commit.
3. Volte pra `main`.
4. Rode `git merge nome-da-branch`.

## Saida esperada (exemplo)

```text
Updating a1b2c3d..e4f5g6h
Fast-forward
 README.md | 1 +
 1 file changed, 1 insertion(+)
```

## Erros comuns + como resolver

### commit na branch errada

Rode `git branch` antes de commitar.
A branch atual vem com `*`.

### `Already up to date`

Significa que nao tinha nada novo pra mergear.

### branch vira bagunca

Cria branch por tarefa curta. Nao mistura 5 coisas num mesmo branch.

## Exercicios

### Faceis (3)

1. Criar branch `feat/teste`.
2. Alterar um arquivo e commitar.
3. Voltar para `main`.

### Medios (2)

1. Fazer merge de branch na `main`.
2. Deletar branch local depois do merge.

### Desafio (1)

1. Criar duas branches (`feat/a` e `feat/b`), commitar em ambas e mergear em ordem.
