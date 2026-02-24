# 01 - Configuracao inicial do Git

## Objetivo

Configurar nome, email e editor padrao no Git, e fazer primeira validacao.

## Explicacao curta

Se voce nao configura nome/email, seu commit fica quebrado.
Esse passo evita o erro classico: `Please tell me who you are`.

## Codigo completo

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@exemplo.com"
git config --global init.defaultBranch main
git config --global core.editor "code --wait"

git config --global --list
```

## Como executar

1. Abra terminal.
2. Rode os comandos acima (troque nome/email).
3. Confira com `git config --global --list`.

## Saida esperada (exemplo)

```text
user.name=Joao Silva
user.email=joao@email.com
init.defaultbranch=main
core.editor=code --wait
```

## Erros comuns + como resolver

### `Please tell me who you are`

Faltou configurar `user.name` e `user.email`.

### `code --wait` nao funciona

No VS Code, rode `Shell Command: Install 'code' command in PATH`.
Ou usa outro editor no `core.editor`.

### email errado no commit

Ajusta com:

```bash
git config --global user.email "email_correto@exemplo.com"
```

## Exercicios

### Faceis (3)

1. Configurar nome.
2. Configurar email.
3. Validar com `git config --global --list`.

### Medios (2)

1. Trocar editor padrao pra outro editor que voce use.
2. Configurar branch inicial como `main`.

### Desafio (1)

1. Explicar a diferenca entre configuracao `--global` e local (por repo).
