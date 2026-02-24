# 01 - Pull Request (colaboracao real)

## Objetivo

Criar branch, subir para GitHub e abrir Pull Request com descricao decente.

## Explicacao curta

PR e o caminho certo pra colaborar em time.
Nada de commitar direto na `main` sem revisao.

## Codigo completo

```bash
git checkout -b feat/login-page

git add .
git commit -m "feat: adiciona estrutura inicial de login"
git push -u origin feat/login-page
```

Depois disso, o PR e aberto no GitHub pela interface web.

## Como executar

1. Crie branch da tarefa.
2. Faca commits pequenos.
3. Suba branch com push.
4. Abra PR no GitHub para `main`.
5. Peca revisao.
6. Aplique feedback e atualize PR.

## Saida esperada (exemplo)

```text
remote:
remote: Create a pull request for 'feat/login-page' on GitHub by visiting:
remote:      https://github.com/.../pull/new/feat/login-page
```

## Erros comuns + como resolver

### PR gigante com 200 arquivos

Quebra em PR menor. Facilita revisao e evita dor de cabeca.

### descricao vazia no PR

Coloca pelo menos:

- o que mudou
- por que mudou
- como testar

### commit sem contexto

Mensagem ruim atrapalha revisao.
Escreve como se outro dev fosse ler sem voce do lado.

## Exercicios

### Faceis (3)

1. Criar branch de feature.
2. Fazer commit nessa branch.
3. Subir branch no GitHub.

### Medios (2)

1. Abrir PR com descricao curta.
2. Atualizar PR com novo commit.

### Desafio (1)

1. Simular revisao: comentar o PR de um colega e sugerir ajuste.
