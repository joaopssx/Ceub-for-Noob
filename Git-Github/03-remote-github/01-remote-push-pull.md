# 01 - Remote com GitHub (push e pull)

## Objetivo

Conectar repositorio local ao GitHub e sincronizar codigo.

## Explicacao curta

Local sozinho nao basta.
Remote no GitHub garante backup e colaboracao.

## Codigo completo

```bash
git remote add origin https://github.com/SEU-USUARIO/SEU-REPO.git
git branch -M main
git push -u origin main

git pull origin main
```

## Como executar

1. Crie repo vazio no GitHub.
2. Copie URL HTTPS.
3. Rode `git remote add origin ...`.
4. Envie com `git push -u origin main`.
5. Depois use `git push` e `git pull` no dia a dia.

## Saida esperada (exemplo)

```text
branch 'main' set up to track 'origin/main'.
Everything up-to-date
```

## Erros comuns + como resolver

### `remote origin already exists`

Voce ja cadastrou remote.
Troca URL com:

```bash
git remote set-url origin NOVA_URL
```

### erro de autenticacao no GitHub

GitHub nao aceita senha comum no terminal.
Use token (PAT) ou `gh auth login`.

### `rejected` no push

Remote tem commit que local nao tem.
Faz pull antes:

```bash
git pull --rebase origin main
```

## Exercicios

### Faceis (3)

1. Criar repo no GitHub.
2. Conectar remote `origin`.
3. Enviar primeiro push.

### Medios (2)

1. Fazer alteracao no GitHub e puxar com `git pull`.
2. Fazer alteracao local e subir com `git push`.

### Desafio (1)

1. Clonar repo novo em outra pasta e manter sincronizado com pull/push.
