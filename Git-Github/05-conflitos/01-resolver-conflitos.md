# 01 - Resolvendo conflitos

## Objetivo

Entender conflito de merge e resolver sem quebrar o projeto.

## Explicacao curta

Conflito acontece quando duas pessoas editam a mesma parte do arquivo.
Nao e erro grave, e rotina de time.

## Codigo completo

```bash
# em main
git checkout main

# em branch A
git checkout -b feat/a
# editar README.md
git add README.md
git commit -m "feat: altera linha A"

# volta main e cria branch B
git checkout main
git checkout -b feat/b
# editar a mesma linha de README.md
git add README.md
git commit -m "feat: altera linha B"

# tenta merge que gera conflito
git checkout main
git merge feat/a
git merge feat/b
```

Quando conflitar, o arquivo fica com marcadores:

```text
<<<<<<< HEAD
conteudo atual
=======
conteudo da outra branch
>>>>>>> feat/b
```

Resolucao:

```bash
# editar arquivo e remover marcadores
git add README.md
git commit -m "fix: resolve conflito no README"
```

## Como executar

1. Gere conflito controlado (como acima).
2. Abra arquivo e decida versao final.
3. Remova marcadores.
4. Faca `add` e commit de resolucao.

## Saida esperada (exemplo)

```text
CONFLICT (content): Merge conflict in README.md
Automatic merge failed; fix conflicts and then commit the result.
```

## Erros comuns + como resolver

### esquecer de remover marcador `<<<<<<<`

Se commitar assim, arquivo quebra e equipe xinga.
Confere arquivo antes de commit.

### resolver conflito no susto

Le as duas versoes e decide com calma.
Nao sai apagando tudo.

### `git status` ignorado

`git status` mostra exatamente o que falta resolver.
Usa ele sempre.

## Exercicios

### Faceis (3)

1. Gerar conflito em arquivo de teste.
2. Resolver conflito e commitar.
3. Ver historico com `git log --oneline --graph`.

### Medios (2)

1. Simular conflito em branch de feature real.
2. Resolver mantendo parte de cada lado.

### Desafio (1)

1. Explicar em texto curto para colega como resolver conflito sem perder codigo.
